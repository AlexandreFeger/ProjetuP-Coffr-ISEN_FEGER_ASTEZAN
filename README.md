# ProjetuP-Coffr-ISEN_FEGER_ASTEZAN
Fonctionnement du Code
Le programme initialise les périphériques STM32, y compris les capteurs de mouvement et environnementaux, l'interface SPI pour l'écran 7 segments, et les boutons pour l'interaction utilisateur.
Le potentiomètre est utilisé pour entrer les chiffres du code, qui sont affichés sur l'écran 7 segments. Pour faciliter la saisie, des LEDs sont placées sous chaque digit de l'écran 7 segments pour indiquer le chiffre en cours de modification. L'utilisateur peut naviguer entre les chiffres du code en utilisant les boutons BTN1 et BTN2, permettant de passer au digit suivant ou de revenir au digit précédent, respectivement.
Une fois le code complet saisi, l'utilisateur appuie sur le bouton BTN4 pour valider le code. Si le code est correct, une animation LED est déclenchée pour indiquer le succès, et l'écran affiche "COOL". Si le code est incorrect, l'écran affiche "FAIL".
En appuyant sur le bouton BTN3, le système affiche les données environnementales (pression, température, humidité) sur le terminal Teraterm. Ces données sont fournies par les capteurs intégrés au système.
Des interruptions sont utilisées pour gérer les boutons et les capteurs en temps réel, assurant ainsi une réactivité optimale du système. Cela permet de capturer les entrées utilisateur et de lire les valeurs des capteurs de manière efficace et précise.
