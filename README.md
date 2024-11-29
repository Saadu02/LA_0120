# Projekt-Dokumentation


LA_0120 Carina Sutter, Sathana Suganthasri, Nicola Karrer

| Datum  | Version | Zusammenfassung                                              |
| ------ | ------- | ------------------------------------------------------------ |
| 01.11. | 0.0.1   | Informieren und Ausprobieren |
| 08.11. | 0.1.1   | Projektplanung, Aufteilung und Entscheidungen treffen |
| 15.11. | 0.1.2   | Änderungen, LEDs und Sensoren verknüpfen |
| 22.11. | 1.0.0   | Auto-Ampel und Fussgänger-Ampel fertig |
| 29.11. | 1.1.0   | Auto- und Fussgänger-Ampel miteinander verbunden |
| 06.12. | X.X.X   | - |
| 13.12. | X.X.X   | - |

## 1 Informieren

### 1.1 Ihr Projekt

Wir wollen uns an etwas neues getrauen und haben uns deshalb überlegt, ein Produkt mit Schaltkreisen zu entwickeln. Dafür hatten wir die Idee, ein Ampelsystem zu bauen mit verschiedenen LEDs und Sensoren. Dazu kommt ein selbstgeschriebenes Programm, mit dem der ganze Lichtwechsel automatisiert wird.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Beschreibung                       |
| ---- | --------------- | ---------------------------------- |
| 1    | Funktional | Als ein User möchte ich, dass die Sensor auf einem Objekt erkennen können |
| 2    | Funktional | Als ein User möchte ich, dass die LEDs am richtigen Zeitpunkt ein- oder ausgeschaltet sind. |
| 3    | Funktional | Als ein User möchte ich, dass die Ampeln automatisch die LEDs nach Sensor wechseln. |
| 4    | Funktional | Als ein User möchte ich, dass eine dass es eine Schaltfläche gibt, die ich anklicken kann, um die Fussgängerstreifen sicher zu überqueren. |
| 5    | Funktional | Als ein User möchte ich, dass nach dem Klicken der Schaltfläche die LEDs automatisch nach Überprüfung des Objekts wieder grün leuchten.|


### 1.3 Diagramme

![image](https://github.com/user-attachments/assets/189c4587-95cc-4937-9d69-6ddca6c73c70)

08.11.

![image](https://github.com/user-attachments/assets/cc304349-b940-4ddf-bf5a-21c444da5a72)

22.11.
![image](https://github.com/user-attachments/assets/fc400210-bb41-4f28-bc3f-9be6ddaffa9b)


![image](https://github.com/user-attachments/assets/90a9376e-4725-440f-9484-00f9bcebe9d9)

29.11.

## 2 Planen

| AP-№ | Frist  | Zuständig | Beschreibung | geplante Zeit |
| ---- | ------ | --------- | ------------ | ------------- |
| 0.A  | 01.11. | Alle | Informieren / Planen | 180min |
| 0.B  | 08.11. | Alle | Ampelzirkulation-Skizze und -Logik und Plattform kennen lernen | 180min |
| ~1.A~  | ~15.11.~ | ~Sathana~ | ~Sensoren verbinden~ | ~180min~ |
| ~2.A~  | ~15.11.~ | ~Nicola~ | ~LEDs verbinden~ | ~180min~ |
| ~3.A~  | ~15.11.~ | ~Carina~ | ~Zirkulation verstehen~ | ~180min~ |
| ~1.B~  | ~22.11.~ | ~Sathana~ | ~Sensoren Funktionsfähig machen und Ouput bestimmen~ | ~180min~ |
| ~2.B~  | ~22.11.~ | ~Nicola~ | ~LEDs Funktionsfähig machen und Input bestimmen~ | ~180min~ |
| ~3.B~  | ~22.11.~ | ~Carina~ | ~Input und Output verbinden~ | ~180min~ |
| 1.A  | 15.11. | Alle | Bewegungs-Sensoren definieren | 90min |
| 2.A  | 15.11. | Alle | LEDs verbinden | 90min |
| 3.A  | 22.11. | Alle | Sensoren mit LEDs verknüpfen | 90min |
| 4.a  | 22.11. | Alle | Fussgängerwechsel skizzieren und implementieren | 90min |
| 4.b  | 29.11. | Alle | Auto-Ampel und Fussgänger-Ampel verknüpfen | 180min|
| 4.c  | 06.12. | Alle | 4x Ampel für ganze Kreuzung | 180min |
| 4.c  | 13.12. | Alle | 4x Ampel für ganze Kreuzung | 180min |


## 3 Entscheiden

01.11.
Unsere Idee ist es zuerst eine per Knopfdruck funktionierende Ampel zu programmieren. Dabei benutzen wir die Programmiersprache Python und werden diese besser kennenlernen, da wir das in der Schule nicht durchgenommen haben. Dazu werden wir pi-top [4] benutzen, das Raspberry PI beinhält und die Erweiterung Electrics-Kit verwenden.

08.11.
Wir haben uns dazu entschieden Tinkercad, ein Online Arduino-Simulator, zu benutzen, damit wir auch von Zuhause aus arbeiten können. Diese ist zudem Einsteiger freundlich und wir können alle über einen geteilten Link aufs Projekt zugreifen, das sich auch in Echtzeit aktualisiert.
Eine weitere Änderung ist, dass wir jetzt C++ benutzen werden anstatt von Python, da wir die Plattform geändert haben.

15.11.
Wir haben versucht, die Schaltung mit einem PIR-Sensor zu machen, das aber nicht funktioniert hat. Nun versuchen wir, das ganze mit einem Ultraschall-Abstandssensor zu implementieren.
Ausserdem haben wir anstatt unsere Aufgaben selbstständig zu lösen, das Meiste zusammen gemacht, da wir so wie so alles miteinander verknüpft ist und wir auf dem selben Projekt arbeiten.


## 4 Realisieren

| AP-№ | Datum  | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ------ | --------- | ------------- | ----------------- |
| 0.A  | 01.11. | Alle | 180min | 180min |
| 0.B  | 08.11. | Alle | 180min | 180min |
| 1.A  | 15.11. | Alle | 90min | 150min |
| 2.A  | 15.11. | Alle | 90min | 30min |
| 3.A  | 22.11. | Alle | 150min | 90min |
| 4.A  | 22.11. | Alle | 180min | 90min |

## 5 Kontrollieren

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |
