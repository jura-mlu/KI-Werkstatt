# Übung: Halluzination und Verifikation (BVerfGE 81, 310 – „Kalkar II“)

**Einsatz in der KI-Werkstatt:** Veranschaulichung der Differenz zwischen statistischer Sprachvervollständigung und inhaltlicher Richtigkeit (vgl. Werkstattbericht, Abschnitt IV.1).

**Setting:** Die Übung wurde bewusst mit einem Sprachmodell **ohne eigenständige Internetrecherche** durchgeführt (hochschuleigene KI-Anwendung, ein HAWKI-Klon), das ausschließlich auf Grundlage seiner Trainingsdaten operierte. Bei aktuellen kommerziellen Modellen mit integriertem Grounding lassen sich die Halluzinationen nicht mehr zuverlässig reproduzieren.

## Prompt

```
Fasse mir die Entscheidung BVerfGE 81, 310 zusammen
```

**Variante (Disambiguierung):**

```
Fasse mir die Entscheidung BVerfGE 81, 310 (Kalkar II) zusammen
```

## Erwartbarer Befund

Das Modell gibt der Form nach eine Urteilszusammenfassung aus – allerdings nicht zur angefragten Entscheidung. Es verwebt Inhalte bekannterer Leitentscheidungen (etwa BVerfGE 65, 1 – Volkszählung; BVerfGE 105, 252 – Glykol) zu einem Text, der den tatsächlichen Gegenstand von BVerfGE 81, 310 (Bund-Länder-Streit zu Voraussetzungen und Schranken einer Weisung nach Art. 85 III GG im Kontext des Atomrechts) verfehlt. Der Klammerzusatz „(Kalkar II)“ verbessert die Zuordnung nur in einzelnen Durchläufen; der Kurztitel ist in den Trainingsdaten auch mit der anders gelagerten „Kalkar I“-Entscheidung verknüpft.

## Gegenstrategien

- **Grounding:** Den Prompt so gestalten, dass das Modell – soweit technisch möglich – zu einem Quellenabgleich angehalten wird.
- **Disambiguierung:** Präzisieren, welche konkrete Entscheidung gemeint ist und welcher Detailgrad erwartet wird.
- **Nichtwissen einräumen lassen:** Dem Modell die Möglichkeit geben, fehlende Informationsgrundlagen offenzulegen, z. B.:

```
Falls du keine gesicherten Informationen findest, teile mir das mit.
```
