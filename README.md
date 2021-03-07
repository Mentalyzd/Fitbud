# Fitbud: Find your fitness buddies!
Deze app is gemaakt als project voor Blok Tech. Hierbij was het de bedoeling om een dynamische webapp te maken met gebruik van Node.js, Express en MongoDB. Deze app is gemaakt voor mensen die opzoek zijn naar gym buddies. Dit kan zijn om mee te sporten of om meer ervaring op te doen.

Deze webapp is alleen voor mobiel gebruik. Met de app kan je een eigen account aanmaken, inloggen, gebruikers liken en je profiel aanpassen.

![](https://user-images.githubusercontent.com/32453774/110257911-455ab700-7fa0-11eb-9082-cf1aadaf2e96.jpg)

## Content
1. [Install App](#install-app)
2. [Install Database](#install-database)
3. [Dependencies](#dependencies)
4. [License](#license)


## Install App
### Stap 1
Installeer git
```
sudo apt update
sudo apt install git
```
Controleer of installatie gelukt is
```
git --version
Voorbeeld output: git version 2.17.1
```


### Stap 2
Clone de repo van github en ga naar de folder
```
git clone https://github.com/Mentalyzd/Fitbud.git
cd Fitbud
```


### Stap 3
Installeer npm
```
npm install
```
Controleer npm install
```
npm -v
Voorbeeld output: 7.5.3
```


### Stap 4
Run de applicatie
```
npm start
```
Succesvolle output:
```
App listening at http://localhost:2999 and on local network at http://YOU_LOCALE_IP_ADRES:8080
```

## Install Database
### Stap 1
Maak account aan voor mongoDB
```
Ga naar: https://account.mongodb.com/account/register
```
1. Zodra je ingelogd bent maak je een nieuw project aan in MongoDB Atlas.
2. Daarna maak je ook een nieuw cluster en een database aan met de naam naar keuze. **Onthoud de database naam goed!**
3. MongoDB vraagt je om een username en een wachtwoord maken voor de database connectie. **Onthoud deze ook goed!**



### Stap 2
Maak in de root van de repo een bestand aan, genaamd .env
```
touch .env
```

Open het nieuwe betand in nano
```
nano .env
```
Hierin ga je variable toevoegen als gebruikersnaam, wachtwoord en database naam:
```
DB_USER=JOUW_DATABASE_GEBRUIKERSNAAM
DB_PASS=JOUW_DATABASE_WACHTWOORD
DB_NAME=JOUW_DATABASE_NAAM
```
Sla je bestand op, type:
```
CTRL + X
```


### Stap 3
Stop de applicatie, type:
```
CTRL + C
```
Start de applicatie opnieuw
```
npm start
```
De database connectie is succesvol als het volgende in de terminal staat:
```
Connection succesfull
[]
```

## Dependencies
In dit project heb ik de volgende packaged gebruikt **NPM** : 
* [bcrypt](https://www.npmjs.com/package/bcrypt)
* [body-parser](https://www.npmjs.com/package/body-parser-json)
* [dotenv](https://www.npmjs.com/package/dotenv)
* [ejs](https://www.npmjs.com/package/ejs)
* [express](https://www.npmjs.com/package/express)
* [express-session](https://www.npmjs.com/package/express-session)
* [mongoose](https://www.npmjs.com/package/mongoose)
* [multer](https://www.npmjs.com/package/multer)
* [node](https://www.npmjs.com/package/node)
* [nodemon](https://www.npmjs.com/package/nodemon) **(Dev-dependency)**

## License
[MIT](https://github.com/Mentalyzd/Fitbud/blob/main/LICENSE) © [Christiaan Zandbergen](https://github.com/Mentalyzd)

