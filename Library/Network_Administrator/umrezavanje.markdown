		Umrežavanje  
		    Sadržaj :

		        1. Osnove umrežavanja



###  1.Osnove umrežavanja

Razbijenje velike mreže u više manjih zove se **segmentacija** mreže, to postižemo upotrebom rutera(router),komutatora(swich) i mostova(bridge).  
- Mogući uzroci zagušenja LAN saobraćaja su:  
  - Previše matičnih računara u emisonom domenu
  - Emisione oluje (broadcast storm)
  - Višesmerno odašiljanje (multicating)
  - Mali propusni opseg
  - Dodavanje u mrežu razvodnih uređaja radi konektivnosti
  - Veliki ARP ili IPX saobraćaj (IPX je Novellov protokol rutiranja, slićan IP-u)  

Ruteri se koriste za međusobno povezivanje mreža i usmeravanje paketa podataka iz jedne mreže u drugu.Ruteri po standardnom podešavanju, razbijaju emisioni domen(skup uređaja u mrežnom segmentu  koji osluškuju sve opšte poruke poslate u taj segment).

Ruteri u mreži:
- ne prosleđuju opšte poruke po standardnom podešavanju
- filtriraju mrežu na osnovu informacija (ip adresa npr.)

Ruteri u mreži vrše:
- komutaciju paketa (sloj 3 ili logičko adresiranje)
- filtriranje paketa
- komutacija između paketa
- odabiranje putanje
