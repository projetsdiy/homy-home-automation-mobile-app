# Homy
Homy is a mobile application for iOS and Android that allows you to drive and receive data from one (or more) Open Source home automation server or connected objects developed based on Arduino, ESP32, ESP8266.
This GitHub repository will manage bugs and requests for improvements.

[More details on the beta version of Homy by reading this article](https://diyprojects.io/homy-ios-android-home-automation-application-control-server-diy-connected-objects)

If you like **Homy**, give it a star, or contribute!

[![GitHub stars](https://img.shields.io/github/stars/projetsdiy/homy-home-automation-mobile-app.svg?style=social&label=Star)](https://github.com/projetsdiy/homy-home-automation-mobile-app)
[![donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](paypal.me/ProjetsDIYFR)

**Homy is under development, operation is not guaranteed yet**

## Principle
Homy can connect directly to a Domoticz server via HTTP, HTTPS or MQTT without an intermediary server. You have to expose the server to the internet by configuring the router

<img align="center" src="https://github.com/projetsdiy/homy-home-automation-mobile-app/blob/master/images/FR_homy_diagram_router.jpg" style="max-width:100%;">

If you do not want to expose your home automation server to the internet, you can use an online MQTT server (cloudMQTT for example) on which Homy will connect

<img align="center" src="https://github.com/projetsdiy/homy-home-automation-mobile-app/blob/master/images/FR_homy_diagram_cloud_mqtt_server.jpg" style="max-width:100%;">

All your data remains private and never passes through other servers.

## Status of Connector Development
- [X] HTTP Connector (HTTPS) Domoticz
- [X] MQTT connector with automatic detection of generic JSON objects (Arduino code / ESP8266 / ESP32)
- [X] MQTT connector with Tasmota message support 
- [ ] MQTT connector with support for Espurna messages
- [ ] MQTT connector with Cayenne message support
- [ ] Jeedom HTTP Connector
- [ ] MQTT Home Assistant Connector
- [ ] Gladys connector (format to be determined)
- [ ] MQTT Zigbee2MQTT connector (accessory support using Zigbee protocol such as Xiaomi Aqara / Mijia)

## In the study
- Blynk server
- Support for radio objects: RFLink, MySensors, Sonoff RF Bridge

## State of progress of homy functions of Homy
- [X] Messages parser (incoming / outgoing) of Domoticz equipments
- [X] Messages parser (incoming / outgoing) of Tasmota equipment 
- [X] Messages parser (in / out) of generic JSON devices
- [X] Automatic assignment of a category
- [X] Organize objects by location
- [X] Organize objects by room
- [X] Customization of the display unit (temperature, humidity, barometer, lux, distance, noise, CO2 content, electrical power, water flow)
- [X] Management of the actuators: lamp and switches (ON / OFF), LED bulb (color, brightness, ON / OFF), shutters and blinds (ON / OFF, opening rate), thermostat (set point)
- [X] Start a Domoticz scenario

## In the study
- Scenario generator
- Data logger for objects that are not connected to a home server
- Siri Shortcut shortcuts (iOS)


# Contribute
You can contribute to Homy project by

- Propose new features
- Testing new released features and report issues
- Donating to acquire hardware for testing or send sample for implementing
- Donate

[![donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](paypal.me/ProjetsDIYFR)

# Homy - version bêta
Homy est une application mobile pour iOS et Android qui permet de piloter et recevoir des données en provenance d'un (ou plusieurs) serveur domotique Open Source ou d'objects connectés développés à base d'Arduino, ESP32, ESP8266.
Ce dépôt GitHub permettra de gérer les bugs et les demandes d'améliorations. 

[Plus de détails sur la version bêta de Homy en lisant cet article](https://projetsdiy.fr/homy-application-domotique-ios-android-piloter-serveur-objets-connectes-diy/)

Si vous aimez **Homy** attribuez une étoile ou contribuez au développement

[![GitHub stars](https://img.shields.io/github/stars/projetsdiy/homy-home-automation-mobile-app.svg?style=social&label=Star)](https://github.com/projetsdiy/homy-home-automation-mobile-app)
[![donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](paypal.me/ProjetsDIYFR)

**Homy est en cours de développement, le fonctionnement n'est pas encore garanti**

## Principe 
Homy peut se connecteur directement à un serveur Domoticz via le protocole HTTP, HTTPS ou MQTT sans serveur intermédiaire. Il faut exposer le serveur à internet en configurant le routeur

<img align="center" src="https://github.com/projetsdiy/homy-home-automation-mobile-app/blob/master/images/FR_homy_diagram_router.jpg" style="max-width:100%;">

Si vous ne voulez pas exposer votre serveur domotique à internet, vous pouvez utiliser un serveur MQTT en ligne (cloudMQTT par exemple) sur lequel Homy va se connecter

<img align="center" src="https://github.com/projetsdiy/homy-home-automation-mobile-app/blob/master/images/FR_homy_diagram_cloud_mqtt_server.jpg" style="max-width:100%;">

Toutes vos données **restent privées** et ne transitent jamais par d'autres serveurs.

## Etat d'avancement du développement des connecteurs
- [X] Connecteur HTTP (HTTPS) Domoticz
- [X] Connecteur MQTT avec détection automatique d'objets JSON génériques (code Arduino / ESP8266 / ESP32)
- [X] Connecteur MQTT avec prise en charge des messages Tasmota
- [ ] Connecteur MQTT avec prise en charge des messages Espurna
- [ ] Connecteur MQTT avec prise en charge des messages Cayenne
- [ ] Connecteur HTTP Jeedom
- [ ] Connecteur MQTT Home Assistant
- [ ] Connecteur Gladys (format à déterminer)
- [ ] Connecteur MQTT Zigbee2MQTT (support des accessoires utilisant le protocole Zigbee tel que Xiaomi Aqara / Mijia)

## A l'étude
- Serveur Blynk
- Prise en charge des objets radio : RFLink, MySensors, Sonoff RF Bridge

## Etat d'avancement des fonctions domotiques de Homy
- [X] Parser les messages (entrant/sortant) des équipements Domoticz
- [X] Parser les messages (entrant/sortant) des équipements Tasmota
- [X] Parser les messages (entrant/sortant) des équipements JSON générique 
- [X] Attribution automatique d'une catégorie
- [X] Organiser les objets par lieu 
- [X] Organiser les objets par pièce
- [X] Personnalisation de l'unité d'affichage (température, humidité, baromètre, luminosité, distance, bruit, ensoleillement, teneur en CO2, puissance électrique, débit d'eau)
- [X] Gestion des actionneurs : lampe et interrupteurs (ON/OFF), ampoule à LED (couleur, luminosité, ON/OFF), volets et stores (ON/OFF, taux d'ouverture), thermostat (consigne)
- [X] Lancer un scénario Domoticz

## A l'étude
- Générateur de scénario 
- Enregistreur de données pour les objets qui ne sont pas connectés à un serveur domotique
- Raccourcis Siri Shortcut (iOS)

# Contribuer
Vous pouvez contribuer au projet Homy en

- Proposer de nouvelles fonctionnalités
- Tester les nouvelles fonctionnalités publiées et signaler les problèmes
- Faire un don pour acquérir du matériel ou envoyer du matériel
- Faire un don

[![Faire un don](https://img.shields.io/badge/donate-PayPal-blue.svg)](paypal.me/ProjetsDIYFR)

# Acknowledgment / Remerciements
- [Domoticz team and contributors](https://github.com/domoticz/domoticz)
- [Theo Arends and contributors for Tasmota firmware](https://github.com/arendst/Sonoff-Tasmota)
- [Ionic Framework](https://ionicframework.com/) and [Angular project](https://angular.io/) used for development
- [Font Awesome](https://fontawesome.com/)
