# elwasys Portal

## Einrichten der Entwicklungsumgebung

Zum Weiterentwickeln der Software wird folgende Software benötigt:

-	Java Development Kit 8

	http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

-	Apache Maven

	https://maven.apache.org/

-	Eclipse EE

	http://www.eclipse.org/downloads/

-	Git, z.B. mit der Benutzeroberfläche SoureTree, oder GitKraken

	https://www.sourcetreeapp.com/

### Vorbereitungen in Eclipse

Damit Maven funktioniert, muss in Eclipse das installierte JDK als Ausführungs-Umgebung eingerichtet werden.

1. Window > Preferences
2. Java > Installed JREs
3. "Add..." > Pfad zum installierten JDK 8 auswählen
4. Java > Installed JREs > Execution Environments
5. JavaSE-1.8 > Haken bei "jdk1.8[...]" setzen
6. "OK" klicken

### Run-Konfiguration für den Jetty-Server einrichten

1. Run > Run Configurations...
2. "Maven Build": Rechtsklick > Neu...
3. Name: Jetty Starten
4. Base Directory: "${workspace_loc:/Waschportal}"
5. Goals: "install jetty:run"

Jetzt kann das Waschportal durck einen Klick auf den kleinen Pfeil neben dem grünen Start-Pfeil "Run As..." > "Start Jetty" gestartet werden und ist dann unter http://localhost:8080 erreichbar. Code-Änderungen werden automatisch auf den laufenden Server geladen.
