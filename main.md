# Zusammenfassung Datenbanken

### 1. Phasen der Entwicklung einer Datenbank

![](C:\Users\Benno\AppData\Roaming\marktext\images\2022-06-10-13-05-10-image.png)

---

#### 1.1 Externe Phase/Anforderungsanalyse

##### Anforderungsanalyse

In dieser Phase sammelt man den Informationsbedarf (IST/SOLL Analyse) und Ordnet ihn.

### 1.2 Konzptionelle Phase

In dieser Phase werden Daten mihilfe von Beziehungen und Entitätstypen strukturiert und in Diagrammen dargestellt

##### ER-Modell

Ein ER Modell wird meistens genutzt um Datenkardinalitäten zu veranschaulichen.

##### Beispiel eines ER-Modells

In jeder Tabelle stellt jede Reihe Eine Entität dar. Die Zusammenfassung von mehreren Reihen ist eine Entitätsmenge. Jede Spalte ist ein Attribut.

Tabelle Item:

Hier ist der Entitätstyp Item

| I_ID | Name                | ItemType_ID | Screenshot (als String)                                                        | IsRandomlyRolled | TierType_ID |
| ---- | ------------------- | ----------- | ------------------------------------------------------------------------------ | ---------------- | ----------- |
| 1    | Eyasluna            | 9           | ![](https://www.bungie.net/common/destiny2_content/screenshots/235827225.jpg)  | true             | 5           |
| 2    | The Time-Worn Spire | 13          | ![](https://www.bungie.net/common/destiny2_content/screenshots/4425887.jpg)    | true             | 5           |
| 3    | Edge of Intent      | 33          | ![](https://www.bungie.net/common/destiny2_content/screenshots/14194600.jpg)   | true             | 5           |
| 4    | Fighting Lion       | 23          | ![](https://www.bungie.net/common/destiny2_content/screenshots/3549153978.jpg) | false            | 6           |
| 5    | Starfire Protocol   | 28          | ![](https://www.bungie.net/common/destiny2_content/screenshots/2782999717.jpg) | false            | 6           |

Tabelle ItemType (Ausschnitt):

Hier ist der Entitätstyp ItemType

| ItemType_ID | Name             |
| ----------- | ---------------- |
| 9           | Hand Cannon      |
| 13          | Pulse Rifle      |
| 33          | Glaive           |
| 23          | Grenade Launcher |
| 28          | Chestplate       |

Tabelle TierType (Ausschnitt):

Hier ist der Entitätstyp TierType

| TierType_ID | Name      |
| ----------- | --------- |
| 5           | Legendary |
| 6           | Exotic    |

##### Kardinalitäten

![](C:\Users\Benno\AppData\Roaming\marktext\images\2022-06-20-12-41-55-image.png)

Erklärung:

Verb:

![](C:\Users\Benno\AppData\Roaming\marktext\images\2022-06-20-12-43-14-image.png)

Fahren stellt hier das "Verb" dar, als was genau die Beziehung zwischen den Tabellen darstellt. Die Striche die von der Raute in der Mitte weggehen stellen die Eigentlichen Kardinalitäten dar.

Entitätstyp:

![](C:\Users\Benno\AppData\Roaming\marktext\images\2022-06-20-12-47-39-image.png)

Hier ist der Entitätstyp ein Auto. Die "1" auf der Rechten Seite stellt die Beziehung zum anderen Entitätstyp "Fahrer". Da ein Auto von **einem** Fahrer gefahren wird ist diese Beziehung eine 1:1 Beziehung.

Attribut:

![](C:\Users\Benno\AppData\Roaming\marktext\images\2022-06-20-12-49-22-image.png)

Die Marke stellt hier ein Attribut von einem Auto dar.

![](C:\Users\Benno\AppData\Roaming\marktext\images\2022-06-20-12-51-49-image.png)

Weitere Beispiele:

M:N Beziehung:

![](C:\Users\Benno\AppData\Roaming\marktext\images\2022-06-20-12-50-54-image.png)

1:N Beziehung

![](C:\Users\Benno\AppData\Roaming\marktext\images\2022-06-20-12-51-19-image.png)
