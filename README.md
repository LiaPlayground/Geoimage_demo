<!--
author:   Sebastian Zug; André Dietrich

email:    sebastian.zug@informatik.tu-freiberg.de

version:  0.0.4

language: de

import:   https://raw.githubusercontent.com/LiaTemplates/BeforeAndAfter/0.0.1/README.md

-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/LiaPlayground/Geoimage_demo/main/README.md)


# LiaScript meets GeoScience
<!--
persistent: true
-->

Dieses Beispiel illustriert die Verwendung von Darstellungen der [TUBAF Mediathek](https://mediathek.tu-freiberg.de) innerhalb von LiaScript-Lehrmaterialien.

> Die Webseite der Mediathek ist hier interaktiv eingefügt. Damit ließe sich zum Beispiel eine User-Story aufbauen.

??[](https://mediathek.tu-freiberg.de/#/detail/77c364e7-be1c-45bd-b348-fda8a467fb5a)


## Einbettung einzelner Bilder anhand URL

    {{0-1}}
![Beispiel 1](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/80000/80790/feeb4ee9cc5e44f2731e2a764eae56a9cf599e8f/image/png "Hier fehlt jetzt noch der Link auf die zugehörigen Metadaten in der Mediathek")

    {{1-2}}
*********************************************

![Beispiel 1](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/80000/80790/feeb4ee9cc5e44f2731e2a764eae56a9cf599e8f/image/png)<!-- style="filter: grayscale(80)" id="image" -->

Das ist ein etwas umfangreicheres Beispiel.
Hier wurden verschieden Filter über das Bild gelegt.


| Filter      | Wert                                                                                                                |
| ----------- | ------------------------------------------------------------------------------------------------------------------- |
| Grauwert    | <script input="range" value="0" input-always-active output="grayscale"> @input </script>                            |
| Helligkeit  | <script input="range" value="1" min="0" max="10" step="0.1" input-always-active output="brightness">@input</script> |
| Kontrast    | <script input="range" value="1" min="0" max="10" step="0.1" input-always-active output="contrast">@input</script>   |
| Sättigung   | <script input="range" value="1" min="0" max="10" step="0.1" input-always-active output="saturation">@input</script> |

<script input="hidden">
document.getElementById("image").style.filter = "grayscale(@input(`grayscale`)) brightness(@input(`brightness`)) contrast(@input(`contrast`)) saturate(@input(`saturation`))";
</script>

Dieser begleitende Text eingefügt und ein Quizz zum Bild integriert.


__Welche Eigenschaften lassen sich aus diesem Dünnschliff ableiten?__

- [( )] keine Ahnung
- [(X)] ziemlich "fleckig"
- [( )] mit der Belichtung stimmt was nicht

*********************************************

## Einbettung von Bildern in einer Galerie

![Beispiel 1](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/80000/80790/feeb4ee9cc5e44f2731e2a764eae56a9cf599e8f/image/png)
![Beispiel 2](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/81000/81387/2b9379093c840e6a716411ea85ac5d6ee5459188/image/png)
![Beispiel 3](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/81000/81386/688abef24196640d61aefbbe0ddb146a742add5d/image/png)
![Beispiel 4](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/81000/81388/e172db1fdcf475e5503df2f76f2c20e7ec232d9e/image/png)
![Beispiel 5](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/81000/81389/a9b0540dc27a29407adee551d5b072b1214cb41f/image/png)
![Beispiel 6](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/81000/81390/3ddbfdf3104078ca09f5ea46beeed974ee1a9a78/image/png)
![Beispiel 7](https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/81000/81391/0a540c0f7ced873bd2e847e98c0ae0c5e0b186b9/image/png)

## Überlagerung von mehreren Bildern

<!-- style="max-width: 78vh;" -->
@beforeAndAfter(https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/80000/80790/feeb4ee9cc5e44f2731e2a764eae56a9cf599e8f/image/png,https://mediathek.tu-freiberg.de/eas/partitions-inline/2/0/81000/81387/2b9379093c840e6a716411ea85ac5d6ee5459188/image/png)

## Anmerkung
<!--
persistent: true
-->

> Die Bilder können auch vorkonfiguriert lokal gespeichert werden. Die vorgestellten Mechanismen sind dann identisch.

![](./images/Q003130_002-5x-xpol.png)
![](./images/Q003233a_002-5x-xpol.png)


> oder es können auch direkt 3D-Modelle eingebettet werden:

??[3D-Modell](https://sketchfab.com/3d-models/familienschacht-freiberg-germany-7c7d30506c554385a4a4321366e2e601)