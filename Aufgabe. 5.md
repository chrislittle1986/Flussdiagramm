ALGORITHMUS PasswortEingabeMit3Versuchen

1:  BEGINN
2:      versuche = 0
3:      versuche = versuche + 1
4:      EINGABE passwort
5:      WENN passwort = korrektes_passwort DANN 
            GEHE ZU Zeile 10
6:      WENN versuche < 3 DANN 
            GEHE ZU Zeile 8
7:      GEHE ZU Zeile 12
8:          AUSGABE "Falsches Passwort! Noch " + (3 - versuche) + " Versuche übrig"
9:          GEHE ZU Zeile 3
10:     AUSGABE "Zugriff gewährt - Willkommen!"
11:     GEHE ZU Zeile 13
12:     AUSGABE "Zugriff gesperrt - Zu viele falsche Versuche!"
13: ENDE
