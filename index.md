## This a unofficial Documentation for the Orange Pi
## It is not Complete
## If you found an Issue or make changes, send me Pull request. 

![Orange Pi Plus](OPi+.PNG) 
 
1.Content   
2.Hardware       
3.Linux   
4.Android   
5.H3droid  

# Orange Pi™ ist eine eingetragene Marke der Shenzhen Xunlong Software CO., Limited  
# Hinweis:
### Der Autor übernimmt keine Haftung für Schäden und damit verbundene Verluste.
### Der Autor hat auf den Inhalt der in diesem Dokument verwiesenen Webseiten
### keinen Einfluss und übernimmt keine Haftung für die Benutzung der Webseiten.
### Die Nutzung der vorgestellten Software erfolgt auf eigene Gefahr, der Autor
### übernimmt keine Haftung für Schäden aller Art die mit der Nutzung der Software
### entstehen können., ferner übernimmt der Autor keine Haftung für
### Schäden an Hardware, Menschen und Tieren. Diese Dokumentation ist nach bestem
### wissen und gewissen geschrieben worden.  

### Inhaltsverzeichnis
1. Einführung 
2. Warum ein Orange Pi Plus ? 
3. Vor/Nachteile 
4. Wo finde ich Hilfe ? 
5. Welche Hardware brauche ich ? 
6. Welche Software brauche ich ? 
7. Welches Betriebssystem ? 
8. Community Projekte 
9. Vorbereiten einer SD-Karte 
10. Erste schritte im Umgang mit Linux 
11. Ansteuern von GIPOs 
12. Kritik 
13. Quellenangaben 
Bilder des Orange Pi Plus 

# 1.Einführung 
Die Firma „Xunlong Software“ welche ihren Sitz in Shenzhen City, China hat (Website: 
http://www.orangepi.org/ ) bringt in regelmäßigen Abständen Einplatinencomputer heraus, welche 
meistens auf auf SOCs der Firma Allwinner basieren. Darunter der H3 Prozessor der 
auf dem Orange Pi Plus und weiteren Boards verwendet wird. 

# 2.Warum ein Orange Pi Plus ? 
Im Vergleich zu einen Raspberry Pi hat der Orange Pi Plus eine bessere Hardwareausstattung, 
er verfügt über „Gigabit“ 10/100/1000 Ethernet (Raspberry Pi nur 10/100 MBit Ethernet), 
einen SATA Anschluss, 8 Gbyte emmc Speicher auf dem Android vorinstalliert ist, 1 GB DDR3 
Ram (Raspberry Pi 1GB DDR2 ). 

# 3.Vor/Nachteile
 Kommt Später 
# 4. Wo finde ich Hilfe ? 
Es gibt viele Anlaufstellen bei Fragen rund um den Orange Pi, zuerst einmal im Forum des 
Herstellers dieses ist jedoch nicht so aktiv und einige Fragen werden nicht beantwortet. Aktiver ist 
das Armbian Forum welches sehr zu empfehlen ist., ganz Professionell wird es mit Sunxi welche 
sich mit Kernel-Hacking (nicht das umgangssprachliche böse „Hacken“) und Treibern befassen, 
diskutieren kann man im #linux-sunxi Channel von freenode.net. Nicht zu vergessen und auch 
empfehlenswert ist Dietpi welches Armbian ähnelt aber „leichter“ ist.

1. Im Forum des Herstellers: (Einige Fragen werden nicht beantwortet) 
http://www.orangepi.org/orangepibbsen/forum.php 
2. Forum von Armbian: https://forum.armbian.com/ 
3. Forum von Dietpi: http://dietpi.com/phpbb/index.php 
4. Sunxi IRC (internet Relay Chat): https://webchat.freenode.net/?channels=linux-sunxi 

# 5. Welche Hardware Brauche ich ?
Allgemein:
• Den Orange Pi Plus selber
• Ein Netzteil mit 5 Volt und 2 Amphere
• Ein Adapterkabel vom USB Male Typ A zur DC Buchse
• Eine SD Karte Class 10 oder besser
• Ein Kühlkörper mit Befestigungsmaterial (Empfohlen)
• Ein SD Kartenreader (Wenn nicht schon Vorhanden)

Zusätzlich für den Desktop Betrieb:
• Eine USB Tastatur
• Eine USB Maus
• HDMI Kabel
• Monitor mit HDMI Eingang (oder endsprechende Adapter)
• Lautsprecher oder Kopfhörer mit AUX Eingang

# 6. Welche Software brauche ich ?
Die jeweilige Software die man benötigt, ist davon abhängig welches Betriebsystem man auf seinen
Rechner benutzt und welches Betriebsystem man auf dem Orange Pi Plus Laufen lassen möchte, so
benötigt ein Nutzer welcher Android nutzen möchte andere Tools&Software als ein Nutzer welcher
ein Linux benutzen möchte.

## Software für Windows:
Zum Vorbereiten einer SD Karte unter Windows:
### H2testw:
Ist ein Tool welches überprüft ob ein Speichermedieum (In diesem fall eine SD Karte)
fehlerhafte Sektoren aufweist. Also ob sie noch für den Einsatz als Speichermedium geeignet ist.
### SD Card Formatter:
Diese Software wird von der SD Association herausgegeben, um SD Karten
zu formatieren (Die Standard Windows Formatierfunktion ist dazu nicht geeignet) und sie somit
zum Brennen eines Software Images vorzubereiten. (Ist auch für Mac OS verfügbar)

### DiskImager32:
Brennt .ISO und .Img Dateien auf SD Karten, CD Roms und USB Sticks.
(Wichtig ist für uns das er Imagedateien auf SD Karten brennen kann)
### Etcher: 

Etcher ist ein Opensourche Tool welches das Brennen von .Img und .ISO Dateien
ermöglicht, ist jedoch weiterentwickelter ist als DiskImager32. (Auch verfügbar für Linux und Mac
OS) Download: https://Etcher.io (Achtung externer Link !)

![Etcher](Etcher.png "Etcher")
#### Bildlizenz: resin-io, Etcher-1.0, CC BY-SA 4.0
Quelle:https://upload.wikimedia.org/wikipedia/commons/c/c0/Etcher-1.0.png
Lizenz: https://creativecommons.org/licenses/by-sa/4.0/legalcode

Um Android unter Windows zu installieren:

### Livesuit:
Da  man Android anders installieren muss als zb: Linux sind die gängigen tools nicht in der Lage
Bootfähige Android Images auf SD karten oder auf emmc Speicher zu schreiben. Livesuit ist dazu
in der Lage.
# Software für Linux:
Zum Brennen von Linux Images:
### Etcher: 
(Siehe oben)
### dd: 
Auf Debian und Ubuntu basierten Systemen installieren via „sudo apt-get install dd“ Befehl.
Zum Brennen von Android Images:
### Livesuit: 
(Siehe oben )
