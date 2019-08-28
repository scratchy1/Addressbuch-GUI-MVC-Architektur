# Addressbuch-GUI-MVC-Architektur
Ich demonstriere den Entwurf einer Anwendung mit GUI am Beispiel eines einfachen Adressbuchs. Als Grundlage orientiere ich mich dabei an der MVC-Architektur
• Initialisierung des Datenmodells durch Einlesen aus der Datei bzw. Erzeugen
einer neuen Instanz der Klasse AddressBookDataModel und
eines für das Laden und Speichern von Adressbuchdaten zuständigen
SerializationToFilePersistence-Objekts.
• Erzeugen eines PersonPanel-Objekts. Dabei wird diesem per Konstruktoraufruf
eine Referenz auf das Datenmodell übergeben. Damit
„kennt“ das PersonPanel-Objekt das Datenmodell.
• Erzeugen des „Neuer Eintrag“-Buttons.
• Erzeugen des Hauptfensters. Dabei werden der „Neuer Eintrag“-Button
und das PersonPanel-Objekt übergeben, da diese auf dem Hauptfenster
angezeigt werden sollen.
• Erzeugen des Controllers, Anmelden des Controllers als Beobachter
beim „Neuer Eintrag“-Button und beim Hauptfenster.
• Sichtbarmachen des Hauptfensters.
Nachdem diese Vorarbeiten erledigt sind, ist das Programm in seinem Normalzustand:
Die Daten des Adressbuchs werden angezeigt und das Programm
wartet auf Aktivitäten der Benutzerin oder des Benutzers.
