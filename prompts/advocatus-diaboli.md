# Promptvorschlag: Advocatus diaboli

**Einsatz in der KI-Werkstatt:** KI-Einsatz als externe Prüfinstanz zur Argumentationskontrolle eigener Texte (vgl. Werkstattbericht, Abschnitt IV.4). Die Studierenden erprobten das Vorgehen an einer bereits vorhandenen eigenen Falllösung.

**Konzeption:** Der Prompt soll das Modell zweistufig vorgehen lassen: Zunächst wird die Argumentationsstruktur des Textes nüchtern analysiert und die einzelnen Argumente werden herausgestellt – ohne den Text umzuschreiben, Aussagen hineinzulesen oder Quellen zu erfinden. Danach wird die erarbeitete Struktur anhand eines Katalogs anerkannter Argumentationsfiguren und geläufiger Fehler überprüft; Argumente oder Argumentationsketten dürfen dabei nicht verkürzt werden.

## Prompt

```
Agiere als kompromissloser advocatus diaboli. Greife nur meine Sicht an.
Identifiziere:
  - versteckte Prämissen,
  - fragwürdige Wertungen,
  - Stellen, an denen der Schluss nicht zwingend ist.
Prüfe meine Argumentation nicht rhetorisch, sondern analytisch und
systematisch auf:
– versteckte Prämissen
– Zirkelschlüsse
– falsche Dichotomien
– Scheinkausalitäten (Korrelation ≠ Kausalität)
– Strohmannargumente
– unzulässige Verallgemeinerungen
– Äquivokationen/Begriffsverschiebungen
– selektive Evidenz/confirmation bias
– normative Sprünge (Sein → Sollen)
– fehlende Alternativerklärungen
– unbelegte Gewichtungen
– innere Widersprüche
– empirische Schwächen
– unklare Maßstäbe
– unzulässige Analogien
– bloße Intuitionen statt Argumente
– Immunisierungsstrategien gegen Kritik
Suche aktiv nach dem stärksten Gegenargument („steelman"), nicht nach
schwachen Einwänden.
Identifiziere außerdem:
– welche Aussagen nur plausibel klingen, aber nicht begründet sind,
– welche Schlussfolgerungen nicht zwingend aus den Prämissen folgen,
– welche Begriffe mehrdeutig oder unscharf verwendet werden,
– welche Annahmen stillschweigend vorausgesetzt werden.
Arbeite präzise, knapp und ohne Schonung. Priorisiere die
schwerwiegendsten Schwächen. Wenn ein Argument tragfähig ist, erkläre
genau warum.
```

## Risiken beim Einsatz

Das Modell kann Lücken in Argumentationsketten durch Halluzination auffüllen, fehlende Prämissen erfinden oder schwache Argumente zu wohlwollend bewerten. Wird die eigene Position im Ausgangstext zu stark hervorgehoben, argumentiert das Modell möglicherweise selbst gegen Strohmänner. Die Ausgabe ist daher stets eigenständig zu prüfen.
