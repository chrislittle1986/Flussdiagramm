ALGORITHMUS PasswortValidierung

EINGABE: passwort (String)
AUSGABE: "Akzeptiert" oder "Verworfen"

BEGINN
    // Check 1: Mindestlänge prüfen
    WENN länge(passwort) < 8 DANN
        AUSGABE "Verworfen: Passwort zu kurz (mindestens 8 Zeichen)"
        ENDE
    ENDE WENN

    // Check 2: Sonderzeichen prüfen
    hatSonderzeichen = FALSCH
    FÜR jedes zeichen IN passwort TUE
        WENN zeichen IST Sonderzeichen (!@#$%^&*()_+-=[]{}|;:,.<>?) DANN
            hatSonderzeichen = WAHR
            VERLASSE Schleife
        ENDE WENN
    ENDE FÜR
    
    WENN hatSonderzeichen = FALSCH DANN
        AUSGABE "Verworfen: Kein Sonderzeichen gefunden"
        ENDE
    ENDE WENN

    // Check 3: Kleinbuchstaben prüfen
    hatKleinbuchstabe = FALSCH
    FÜR jedes zeichen IN passwort TUE
        WENN zeichen IST Kleinbuchstabe (a-z) DANN
            hatKleinbuchstabe = WAHR
            VERLASSE Schleife
        ENDE WENN
    ENDE FÜR

    // Check 4: Großbuchstaben prüfen  
    hatGroßbuchstabe = FALSCH
    FÜR jedes zeichen IN passwort TUE
        WENN zeichen IST Großbuchstabe (A-Z) DANN
            hatGroßbuchstabe = WAHR
            VERLASSE Schleife
        ENDE WENN
    ENDE FÜR

    // Finale Validierung
    WENN (hatKleinbuchstabe = FALSCH) ODER (hatGroßbuchstabe = FALSCH) DANN
        AUSGABE "Verworfen: Passwort muss Klein- und Großbuchstaben enthalten"
    SONST
        AUSGABE "Akzeptiert: Passwort erfüllt alle Anforderungen"
    ENDE WENN

ENDE

// Beispiel-Aufrufe:
// PasswortValidierung("abc123") → Verworfen: Passwort zu kurz
// PasswortValidierung("abcdefgh") → Verworfen: Kein Sonderzeichen gefunden  
// PasswortValidierung("Abcdefg!") → Akzeptiert: Passwort erfüllt alle Anforderungen
