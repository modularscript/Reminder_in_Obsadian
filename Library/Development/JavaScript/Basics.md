

1. sloppy "normal" mode - default in scripts
2. strict mode - throws more errors, prevents pitfalls of the language { => TS 😊}  => 'use strict' to show error
3. Hoisting or scope of code accessing { dead zone } =>  before declared ....
4.  const => declaration
	1. restrictions that make code more readable and easy to understand
	2. must be initialized with value
	3. can't be reassigned after declaration
5. Block Scoping Matters
6. Template Literals improve strings simplicity
7. Data types
	1. Primitive types:
		1. -string
		2. number
		3. boolean
		4. undefined
		5. null
		6. symbol
	2.  everything else - Object type
	3. Type conversions to know
		1.  Explicit type conversion
		2.  Implicit type conversion (coercion)
			1.  truthy (true)
			2.   falsy (false)
				1. false
				2. 0
				3. ''
				4. null
				5. undefined
				6. NaN
	4. Avoid direct comparisons in conditionals

		```
		const username = null;

		if (!username) { 
		
			console.log('no user');
		
		}
		
		```

	3. Use triple equals === (strict equals operator)

		```
		
		if (null === undefined) {
		
			console.log('equals');
		
		} else {
		
		console.log('not equals');
		
		}
		```
	5. Convert to real Boolean values where needed

		```
		
		if (Boolean(NaN) === Boolean(NaN)) {
		
			console.log('equal')
		
		} else {
		
			console.log('not equals')
		
		}
		```

8. 