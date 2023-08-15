  

```

#!/bin/sh

  

#Home

~

  

# Refresh Packages

sudo apt update

  

# Install Required packages

sudo apt install php-cli php-zip zip unzip

  

# Install CURL

sudo apt install curl

# Setups or Home Directory

  

# Download installer script

curl -sS https://getcomposer.org/installer -o composer.php

  

# Get the latest HASH

HASH=`curl -sS https://composer.github.io/installer.sig`

  

# Check the HASH

echo $HASH

  

# Output

# HASH number

  

# Verify installer script

php -r "if (hash_file('SHA384', 'composer.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"

  

# Output

#Installer verified

  
  

# Install Composer - Globally

sudo php composer.php --install-dir=/usr/local/bin --filename=composer

  

# Output

#All settings correct for using Composer

#Downloading...

#

#Composer (version 1.10.8) successfully installed to: /usr/local/bin/composer

#Use it: php /usr/local/bin/composer

#

#   ______

#  / ____/___  ____ ___  ____  ____  ________  _____

# / /   / __ \/ __ `__ \/ __ \/ __ \/ ___/ _ \/ ___/

#/ /___/ /_/ / / / / / / /_/ / /_/ (__  )  __/ /

#\____/\____/_/ /_/ /_/ .___/\____/____/\___/_/

#                    /_/

#```