# Fundraising1 - Emiel Boury, Laurens Hoste, Anas Mechkour, Michiel Beaumont

## Repository

```
├── DB              (documentatie en ontwerp van gebruikte databank)
├── diagrammen      (verschillende use-case/activiteiten diagrammen)
├── documentatie    (documentatie over onderzoek)
├── logboeken       (logboeken van de teamleden)
├── verslag         (verslagen project)
└── Project/Fundraising
    ├── app         (frontend code met react)
    └── src         (backend code met spring boot)
```

## Deploy code
Voor gedetailleerde versie met de configuratie bestanden zie het verslag (verslag/eindverslag-fundraising1.pdf) hoofdstuk 5.

Woorden die cursief staan moeten vervangen worden door eigen waarden.

1. Download de release (.zip) van de [gitlab repository](https://gitlab.stud.atlantis.ugent.be/vop2324/fundraising1/-/releases)
2. scp de release naar de server 
    - scp release.zip *user*@*server-ip*:~
3. Maak een ssh verbinding met de server
    - ssh *user*@*server-ip*
4. Unzip de release
    - sudo apt update
    - sudo apt install unzip
    - unzip release.zip
5. Ga in de release directory
    - cd release
6. De installatie maakt gebruik van duckdns, deze repository is ingesteld met volgende parameters. In het verslag wordt uitgelegd hoe deze aangepast kunnen worden:
    - https://fundraising1.duckdns.org
    - 157.193.171.39
7. Pas de configuratie bestanden en installatie scripts aan indien er andere parameters gebruikt worden
8. Maak het installatiescript uitvoerbaar
    - sudo chmod +x install.sh
    - sudo ./install.sh
## Testen
Importeer de file in fundraising1/Project/postman testen/Events.postman_collection.json in postman.
Na het importeren vind u bij collections de requests om het project te testen.

De unittesten zijn terug te vinden in Project/Fundraising/src/test/java/com/example/fundraisingDonationTests.java

## Inloggegevens voor Auth0
Voor een account met de gewone user rol, kan een account aangemaakt worden.

Er is een admin account voorzien met volgende inloggegevens:
```
    hersenletselliga.fundraising1@gmail.com
    Wachtwoord1!
```
Bij dit adminaccount hoort ook een Gmail account om mails te verzenden en ontvangen via EmailJS
```
    hersenletselliga.fundraising1@gmail.com
    Wachtwoord1
```
## Productieomgeving

De site is te vinden op [https://fundraising1.duckdns.org](https://fundraising1.duckdns.org/) 
# hersenletselliga
# hersenletsel-gift
