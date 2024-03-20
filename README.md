<!--
author:   Sebastian Zug, André Dietrich

email:    sebastian.zug@informatik.tu-freiberg.de

version:  0.0.3

language: en

logo:     https://github.com/SebastianZug/RoboLabVortraege/blob/main/02_LatexUndWord/images/Logo.jpg?raw=true

import:   https://raw.githubusercontent.com/LiaTemplates/BeforeAndAfter/0.0.1/README.md

comment:  

-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/SebastianZug/RoboLabVortraege/main/04_CPU_Aufbau/presentation.md#1)


# LiaScript meets GeoScience

Dieses Beispiel illustriert die Verwendung von Darstellungen der [TUBAF Mediathek](https://mediathek.tu-freiberg.de) innerhalb von LiaScript-Lehrmaterialien.

??[](https://mediathek.tu-freiberg.de/#/detail/77c364e7-be1c-45bd-b348-fda8a467fb5a)

## Einbettung einzelner Bilder anhand URL

   {{0-1}}
![Beispiel 1](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/80000/80790/feeb4ee9cc5e44f2731e2a764eae56a9cf599e8f/image/png "Hier fehlt jetzt noch der Link auf die zugehörigen Metadaten in der Mediathek")

   {{1-2}}
*********************************************

![Beispiel 1](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/80000/80790/feeb4ee9cc5e44f2731e2a764eae56a9cf599e8f/image/png)<!-- style="grayscale(80%);" -->
Das ist ein etwas umfangreicheres Beispiel. Hier wurde ein Grauwertfilter über das Bild gelegt, dieser begleitende Text eingefügt und ein Quizz zum Bild integriert.

__Welche Eigenschaften lassen sich aus diesem Dünnschliff ableiten?__

- [( )] keine Ahnung
- [(X)] ziemlich "fleckig"
- [( )] mit der Belichtung stimmt was nicht

*********************************************

## Einbettung von Bildern in einer Galerie

![Beispiel 1](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/80000/80790/feeb4ee9cc5e44f2731e2a764eae56a9cf599e8f/image/png)
![Beispiel 2](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/81000/81387/2b9379093c840e6a716411ea85ac5d6ee5459188/image/png)

## Überlagerung von mehreren Bildern

<!-- style="max-width: 78vh;" -->
@beforeAndAfter(https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/80000/80790/feeb4ee9cc5e44f2731e2a764eae56a9cf599e8f/image/png,https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/81000/81387/2b9379093c840e6a716411ea85ac5d6ee5459188/image/png)

## Anmerkung

> Die Bilder können auch vorkonfiguriert lokal gespeichert werden. Die vorgestellten Mechanismen sind dann identisch.

![](./images/Q003130_002-5x-xpol.png)
![](./images/Q003233a_002-5x-xpol.png)