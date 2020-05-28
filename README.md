# OutlookNotificationCheck

OutlookNotificationCheck überprüft ob ein Erinnerungsfenster von Outlook 2016 existiert und holt dieses in den Vordergrund.

## Erste Schritte

Mit diesen Anweisungen erhalten Sie eine Kopie der Anwendung auf ihre lokale Maschine.

### Voraussetzungen 

- .NET-Framework 4.5 oder höher

### Installation

#### 1. Führen Sie die Installationsroutine aus.

	> Wechseln Sie dazu in das Verzeichnis *[Downloadverzeichnis]/OutlookNotificationCheck/OutlookNotification_Setup/Debug/*.
	> Führen Sie hier die Installationsroutine *OutlookNotificationCheck_Setup.msi* aus und folgen Sie den Anweisungen.

#### 2. Erstellen Sie einen Autostart Eintrag.
	
	> Öffnen Sie hierzu per Tastenkombination *[WINDOWS] + [R]* das *Ausführen-Fenster* und schreiben dort *shell:startup* hinein und klicken auf die Schaltfläche *OK*.
	> In diesem Ordner erstellen Sie mit *[RECHTSKLICK]* und einem anschließenden Klick auf die Option *Neu* und einem letzen Klick auf *Verknüpfung eine Verknüpfung. Navigieren Sie zu dem Installationsverzeichnis und wählen dort die *OutlookNotificationCheck.exe* aus*.

#### 3. [OPTIONAL] Führen Sie das Programm direkt aus.
	> Klicken Sie hierzu im Installationsverzeichnis auf die ausführbare Datei *OutlookNotificationCheck.exe*.

### Überprüfung der Installation

Um die Installation zu Überprüfen, überprüfen Sie ob sich in der Taskleiste, bzw. genauer im SystemTray das Icon befindet.
Erstellen Sie in Outlook einen Termin mit einer Erinnerung. 
Führen Sie dann eine Anwendung aus, die sonst das Erinnerungsfenster unterdrückt, wie etwa eine Remotedesktopverbindung. 
Wenn das Erinnerungsfenster innerhalb von 10 Sekunden im Vordergrund landet, haben Sie den *Outlook NotificationCheck* erfolgreich installiert.

## Deployment

Öffnen Sie die *OutlookNotificationCheck.sln*-Datei in einer Entwicklungsumgebung für C#. Ich empfehle hier Microsoft Visual Studio 2015 zu nutzen, da es auch zur Entwicklung genutzt wurde.

## Entwickelt mit

- Microsoft Visual Studio 2015

## Versionierung

Wir nutzen Subversion zur Versionierung. Um die verfügbaren Versionen zu sehen, siehe *tags* in diesem Repository.

## Autoren

- **René Panke** - *Initiales Erstellen*

## Lizenz

Dieses Projekt ist lizensiert unter der MIT Lizenz - sehen Sie sich die Lizenz.md für Details an.

## Danksagungen

Die Logik basiert auf [diesem](https://stackoverflow.com/questions/23941123/how-do-you-make-an-outlook-reminder-popup-on-top-of-other-windows "stackoverflow: How do you make an outlook reminder popup on top of other windows
") Beitrag.
