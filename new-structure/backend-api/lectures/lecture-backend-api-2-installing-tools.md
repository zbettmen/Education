### 2. Backend APIs
#### Installing tools

---
#### Vi kommer använda en del mjukvaror...

Detta behöver vi:
* Pakethanterare (chocolatey, brew, apt)
* Kommandoterminal (bash)
* versionshantering (git)
* Web requests (browser, curl, wget, postman)
* json formatter (jq, online json formatter)
* Editor vscode
* node.js
* mongodb

---

#### Pakethanterare

* Motivation:
  * Installerar mjukvara som kommandon i terminalen
  * Lättare att dokumentera och mindre strul vid installation
* Installation:
  * MacOS: <a href="https://docs.brew.sh/Installation" target="blank">https://docs.brew.sh/Installation</a>
  * Windows: <a href="https://chocolatey.org/docs/installation" target="_blank">https://chocolatey.org/docs/installation</a>
  * Linux: apt or pacman

---
#### Kommandoterminal
* Motivation:
  * Enklare att dokumentera steg för att starta eller utveckla lösning
* Installation:
  * MacOS: Terminal är bash
  * Windows: choco install git
  * Linux: Duh

---
#### Versionshantering
* Motivation:
  * Enkelt att gå tillbaka till ett fungerande tillstånd när du skrivit sönder det.
  * Nödvändig branchkunskap.
* Installation:
  * Finns i alla terminaler
  * Får gärna använda GUI, men lära sig terminalen först rekommenderas

---
#### Web requests - Browser
* Motivation:
  * Kan användas för backend också
* Installation:
  * Chrome/Firefox, ni vet

---
#### Web requests - Terminalverktyg (curl)
* Motivation:
  * Enklare att dokumentera steg för att starta eller utveckla lösning
  * Mer kraftfullt än en browser, kan göra alla sorters requests
* Installation:
  * Följer med terminalerna
* Done
```
$ curl resp wget https://www.smp.se/
```			 

---
#### JSON formatter
* Motivation:
  * Enklare att läsa formaterad JSON
* Installation:
	* MacOS: ```$ brew install jq```
	* Windows: ```$ choco install jq```

* Done
```
$ curl -s https://jsonplaceholder.typicode.com/todos/1 | jq .
```			 

---
#### Postman
* Motivation:
  * Gratis 
  * Visuellt verktyg för att förstå hur requests går till
* Installation:
  * MacOS: ```$ cask install postman```		 
	* Windows: ```$ choco install postman```

---
#### Editor (VScode)
* Motivation:
  * Gratis, Bra plugins för att effektivisera utveckling
* Installation:
	* MacOS: ```$ brew install mongodb```
	* Windows: ```$ choco install mongodb```
	* Linux: <a href="https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/" target="_blank">https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/</a>

---	

#### Mongodb
* Motivation:
  * Gratis, sparar och läser JSON utan krångel
* Installation:
	* MacOS: ```$ brew install visual-studio-code```
	* Windows: ```$ choco install vscode```
* Done
  * Anslut till mongo genom att köra “mongo” och få upp en prompt.
