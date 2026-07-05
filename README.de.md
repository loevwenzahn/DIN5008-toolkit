<p align="center">
  <img src="logo.png" alt="Logo des DIN5008 Toolkits" width="480">
</p>

Sprache: [English](README.md) · Deutsch

# DIN5008 Toolkit

Ein fokussiertes XeLaTeX-Toolkit für Briefe, die sich an **DIN 5008 Form A oder Form B** orientieren. Briefform, Vorgabe und Sprache werden unabhängig voneinander gewählt. So führt derselbe übersichtliche Arbeitsablauf vom Bewerbungsschreiben über Geschäfts- und Behördenkorrespondenz bis zu formalen oder bewusst reduzierten persönlichen Briefen.

> Das Toolkit ist nicht DIN-zertifiziert und erhebt keinen Anspruch auf offizielle oder allgemeingültige Konformität.

## Dein Weg zum fertigen Brief

Das Toolkit führt in wenigen klaren Schritten zum fertigen Brief:

1. **Ergebnis ansehen** – die Vorschaugalerie zeigt alle fünf Vorgaben für Form A und Form B.
2. **Projekt öffnen** – in Overleaf hochladen oder direkt öffnen und XeLaTeX wählen.
3. **Form A oder B wählen**, anschließend genau eine Vorgabe aktivieren.
4. **Absender- und Empfängerdaten ersetzen**, ohne die internen Template-Dateien anzufassen.
5. **Im LetterBody schreiben**, <code>main.tex</code> kompilieren und das PDF prüfen.

Für den normalen Einstieg genügen <code>content.tex</code> und <code>data/sender-data.tex</code>.

~~~tex
\UseLetterForm{A}       % A oder B
\UsePreset{business-de} % eine von zehn Vorgaben
~~~

## Vorschaugalerie

Die Vorschauen sind kompakte einseitige Guides und keine echten Briefe. Sie zeigen die visuelle Hierarchie und ausgewählte Funktionen der jeweiligen Vorgabe mit fiktiven und neutralisierten Demo-Daten.

### Deutsch · Form A

| Bewerbung | Behörde | Geschäft | Legal / Formal | Minimal |
|---|---|---|---|---|
| [<img src="letters/png/example-de-a-application.png" alt="Deutscher Form-A-Guide Bewerbung" width="150">](letters/pdf/example-de-a-application.pdf) | [<img src="letters/png/example-de-a-authority.png" alt="Deutscher Form-A-Guide Behörde" width="150">](letters/pdf/example-de-a-authority.pdf) | [<img src="letters/png/example-de-a-business.png" alt="Deutscher Form-A-Guide Geschäft" width="150">](letters/pdf/example-de-a-business.pdf) | [<img src="letters/png/example-de-a-legal.png" alt="Deutscher Form-A-Guide Legal Formal" width="150">](letters/pdf/example-de-a-legal.pdf) | [<img src="letters/png/example-de-a-minimal.png" alt="Deutscher Form-A-Guide Minimal" width="150">](letters/pdf/example-de-a-minimal.pdf) |

### Englisch · Form B

| Application | Authority | Business | Legal / Formal | Minimal |
|---|---|---|---|---|
| [<img src="letters/png/example-en-b-application.png" alt="Englischer Form-B-Guide Application" width="150">](letters/pdf/example-en-b-application.pdf) | [<img src="letters/png/example-en-b-authority.png" alt="Englischer Form-B-Guide Authority" width="150">](letters/pdf/example-en-b-authority.pdf) | [<img src="letters/png/example-en-b-business.png" alt="Englischer Form-B-Guide Business" width="150">](letters/pdf/example-en-b-business.pdf) | [<img src="letters/png/example-en-b-legal.png" alt="Englischer Form-B-Guide Legal Formal" width="150">](letters/pdf/example-en-b-legal.pdf) | [<img src="letters/png/example-en-b-minimal.png" alt="Englischer Form-B-Guide Minimal" width="150">](letters/pdf/example-en-b-minimal.pdf) |

## Fünf-Minuten-Schnellstart

Eine kompakte Fassung dieser Schritte für den Editor liegt in [README-OVERLEAF.md](README-OVERLEAF.md) und ist dafür gedacht, im Overleaf-Projekt selbst mitzureisen.

1. Projekt in Overleaf öffnen oder hochladen.
2. Unter **Menu → Compiler** den Compiler auf **XeLaTeX** stellen.
3. <code>main.tex</code> bei Bedarf als Hauptdatei festlegen.
4. <code>content.tex</code> öffnen.
5. Genau eine Briefform und genau eine Vorgabe aktivieren.
6. <code>data/sender-data.tex</code> anpassen.
7. Empfänger, Betreff, Referenzen und Demo-Text vollständig ersetzen.
8. <code>main.tex</code> kompilieren und das erzeugte PDF prüfen.

Nach dem Kompilieren solltest du einen einseitigen Brief sehen, der der Business-Vorschau oben entspricht.

Der Bearbeitungsweg bleibt bewusst einfach:

~~~text
Briefform wählen → Vorgabe wählen → Absender eintragen
→ Empfänger wählen → Betreff/Referenzen setzen
→ LetterBody schreiben → main.tex kompilieren
~~~

## In Overleaf öffnen

Für einen schnelleren Einstieg enthält dieser Release zwei Overleaf-fertige ZIP-Pakete. Sie können direkt in Overleaf geöffnet oder manuell heruntergeladen werden.

- [Englisches Paket in Overleaf öffnen](https://www.overleaf.com/docs?snip_uri=https://github.com/loevwenzahn/DIN5008-toolkit/releases/download/v1.0.0/din5008-toolkit-overleaf-en-v1.0.0.zip&main_document=main.tex)  
  Englische Presets, englische Demo-Daten, englische Kommentare und englischer Schnellstart.  
  [ZIP herunterladen](https://github.com/loevwenzahn/DIN5008-toolkit/releases/download/v1.0.0/din5008-toolkit-overleaf-en-v1.0.0.zip)

- [Bilinguales Paket in Overleaf öffnen](https://www.overleaf.com/docs?snip_uri=https://github.com/loevwenzahn/DIN5008-toolkit/releases/download/v1.0.0/din5008-toolkit-overleaf-bilingual-v1.0.0.zip&main_document=main.tex)  
  Englische und deutsche Kommentare, Beispiele und Dokumentation.  
  [ZIP herunterladen](https://github.com/loevwenzahn/DIN5008-toolkit/releases/download/v1.0.0/din5008-toolkit-overleaf-bilingual-v1.0.0.zip)

Nach dem Öffnen in Overleaf den Compiler auf **XeLaTeX** setzen, falls Overleaf ihn nicht automatisch auswählt, und `main.tex` kompilieren.

Das vollständige Repository enthält weiterhin den kompletten Quellstand, Vorschauen, Dokumentation, Changelog und Lizenzdateien.

## Briefform, Vorgabe und Sprache wählen

### 1. Briefform

~~~tex
\UseLetterForm{A}
% \UseLetterForm{B}
~~~

| Form | Charakter |
|---|---|
| Form A | Kompakter Briefkopf und höher angeordnetes Anschriftfeld |
| Form B | Größerer Briefkopfbereich und tiefer angeordnetes Anschriftfeld |

Aktiviere die gewünschte Form ausdrücklich und lasse genau eine Auswahl aktiv.

### 2. Vorgabe und Sprache

| Zweck | Deutsch | Englisch | Zeigt |
|---|---|---|---|
| Bewerbung | <code>application-de</code> | <code>application-en</code> | Persönlicher Briefkopf, Entwurfsablauf, Anlagen |
| Geschäft | <code>business-de</code> | <code>business-en</code> | Bildlogo, Informationsblock, Unternehmensangaben im Fußbereich |
| Behörde | <code>authority-de</code> | <code>authority-en</code> | Strukturierter Referenzblock, zurückhaltender Fußbereich |
| Legal / Formal | <code>legal-de</code> | <code>legal-en</code> | Horizontale Referenzen, optionaler Sachverhaltsblock |
| Minimal | <code>minimal-de</code> | <code>minimal-en</code> | Reduzierte Gestaltung und Monogramm |

Die Endung <code>-de</code> oder <code>-en</code> steuert die sichtbare Sprache. Briefform und Sprache sind unabhängig: Form A kann auf Englisch und Form B auf Deutsch verwendet werden.

## Dateien, die normalerweise bearbeitet werden

~~~text
main.tex                    Kompilier-Einstieg; normalerweise nicht bearbeiten
content.tex                 Form, Vorgabe, Empfänger, Betreff und Brieftext
data/sender-data.tex        Absender- und Kontaktdaten
data/addressbook.tex        optionale wiederverwendbare Empfänger
logo.png                    austauschbares Standardlogo

letters/de-a/               deutsche Form-A-Guidequellen
letters/en-b/               englische Form-B-Guidequellen
letters/pdf/                erzeugte öffentliche Guide-PDFs
letters/png/                erzeugte öffentliche Guide-Vorschauen

template/form-a.tex         internes Geometrieprofil für Form A
template/form-b.tex         internes Geometrieprofil für Form B
template/                   gemeinsame interne Template-Logik
~~~

Für die normale Nutzung sollten Dateien in <code>template/</code> nicht bearbeitet werden.

## Empfänger eintragen und Brief schreiben

Am einfachsten wird der Empfänger direkt gesetzt:

~~~tex
\UseRecipientManual
\SetManualRecipient{%
Platzhalter-Empfänger\\
Platzhalter-Anschrift\\
00000 Musterort
}
~~~

Wiederverwendbare Empfänger können stattdessen aus <code>data/addressbook.tex</code> gewählt werden:

~~~tex
\UseRecipientAddressbook{generic-company}
~~~

Einen eigenen wiederverwendbaren Empfänger ergänzt du mit einer Zeile in <code>data/addressbook.tex</code> und wählst ihn über den Schlüssel:

~~~tex
\DefineRecipient{mein-buero}{Beispielbüro\\Musterstraße 1\\00000 Musterort}
% dann in content.tex: \UseRecipientAddressbook{mein-buero}
~~~

Ein unbekannter Schlüssel erzeugt einen sichtbaren Hinweis im PDF, sodass ein Tippfehler leicht auffällt. Nur eine Empfängermethode sollte aktiv sein. Der eigentliche Brief wird anschließend mit normalen Absätzen in <code>LetterBody</code> geschrieben:

~~~tex
\begin{LetterBody}

Hier steht der eigene Brieftext.

Weitere Absätze funktionieren wie gewohnt.

\end{LetterBody}
~~~

<code>LetterBody</code> verarbeitet den gewählten Empfänger, Anrede, modusspezifische Referenzen, Grußformel und Anlagen. Ersetze vor der echten Nutzung sämtliche Demo-Texte.

## Optionale Funktionen

Die kuratierte Vorgabe ist der Ausgangspunkt. Ergänze nur Funktionen, die für das konkrete Schreiben gebraucht werden.

| Funktion | Befehl | Zweck |
|---|---|---|
| Icons | <code>\UseIconstrue</code> / <code>\UseIconsfalse</code> | Kontaktsymbole, soweit unterstützt |
| Entwurfsmodus | <code>\DraftModetrue</code> | Zeigt den Entwurfshinweis und aktiviert Prüfhelfer |
| Prüfmarkierungen | <code>\TODO{...}</code>, <code>\PLACEHOLDER{...}</code>, <code>\DRAFTNOTE{...}</code> | Nur im Entwurfsmodus sichtbar |
| Rücksendezeile | <code>\UseBackaddresstrue</code> / <code>\UseBackaddressfalse</code> | Steuert die optionale Rücksendeangabe |
| Automatische Anlagen | <code>\SetAttachmentsAuto</code> | Verwendet die Anlagenliste der gewählten Vorgabe |
| Keine Anlagen | <code>\SetAttachmentsNone</code> | Unterdrückt die Anlagenliste |
| Eigene Anlagen | <code>\SetAttachmentsCustom{Dokument A\\Dokument B}</code> | Gibt eine eigene Liste aus |
| Eigenes Logo | <code>\SetHeaderLogoFile{assets/mein-logo.png}</code> | Wählt eine Bilddatei aus dem Projekt |

Lange Namen, Links, Anschriften, Referenzen und Betreffzeilen können anders umbrechen. Prüfe das fertige PDF nach jeder größeren Anpassung.

### Eigene HEX-Farben

Die Vorgaben liefern aufeinander abgestimmte Standardfarben. Einzelne Farbrollen können in `content.tex` nach `\UsePreset` überschrieben werden. Verwende genau sechs Hexadezimalzeichen ohne führendes `#`:

~~~tex
\SetAccentColor{0072CE}
\SetColorBlockColors{EAF3FA}{D5E8F5}{BFDCEC}{9FC9E2}
\SetTextDarkColor{222222}
\SetTextMidColor{666666}
\SetTextLightColor{7B7B7B}
\SetLineColor{D7D7D7}
\SetFoldmarkColor{D3D7D1}
\SetNoticeBackgroundColor{EAF3FA}
\SetLinkColors{0072CE}{0072CE}
~~~

Die vier Segmente des Farbblocks lassen sich außerdem einzeln mit `\SetColorBlockOneColor`, `\SetColorBlockTwoColor`, `\SetColorBlockThreeColor` und `\SetColorBlockFourColor` ändern. Ungültige Werte brechen den Build mit einer konkreten Fehlermeldung ab.

## Referenzen und formale Korrespondenz

Optionale Referenzfelder werden in <code>content.tex</code> gesetzt. Unterstützte leere Felder erscheinen nicht in der Ausgabe.

- Der Behördenmodus unterstützt strukturierte Referenzangaben und eine optionale Faxzeile.
- Legal / Formal unterstützt horizontale Referenzen sowie optionale Bezugszeichen- und Sachverhaltsblöcke.
- Zusätzliche Kennzeichen können leer bleiben, wenn sie nicht benötigt werden.

Der Legal/Formal-Modus ist ein Layout für formale Korrespondenz. Er bietet keine Rechtsberatung und ersetzt keine rechtliche Prüfung.

## QA und Validierung

Das Toolkit wurde mit automatisierten, visuellen und druckorientierten Prüfungen kontrolliert:

- Alle zehn öffentlichen Guides wurden mit zwei XeLaTeX-Durchläufen kompiliert.
- Alle Guide-PDFs wurden als einseitige A4-Ausgaben im Hochformat geprüft.
- Logs wurden auf LaTeX-/Paketfehler, fehlende Assets, offene Referenzen und sichtbare <code>??</code> geprüft.
- Falzmarkenkonfiguration und das zur Briefform passende Testbranding wurden getrennt kontrolliert.
- Alle **2 Formen × 5 Modi × 2 Sprachen (20 Kombinationen)** bestanden einen automatisierten Smoke-Test.
- Repräsentative zweiseitige Dokumente dienten zur Prüfung der Folgeseitenköpfe und aufgelösten Gesamtseitenzahlen.
- Repräsentative Form-A- und Form-B-Ausgaben wurden in druckorientierten Prüfungen begutachtet.

Die Guide-Ausgaben wurden vor der Veröffentlichung mit einem internen Regressionstest geprüft. Öffentliche Guide-PDFs und PNGs werden erst nach manueller Sichtprüfung aktualisiert.

## Druck und DIN-5008-Abgrenzung

Das Toolkit orientiert sich an der Geometrie von DIN 5008 Form A und Form B, darunter A4-Seitenformat, Anschriftfeld, Textachsen, Referenzbereiche, Falzmarken, Briefköpfe und Fußbereiche.

Es ist nicht DIN-zertifiziert und verspricht keine offizielle oder allgemeingültige Konformität. Druckerränder, Skalierung, installierte Schriften, Inhaltslänge, Umschläge, lokale Anforderungen und eigene Overrides können das Ergebnis beeinflussen.

Prüfe jedes PDF vor dem Versand. Wichtige Korrespondenz sollte mit dem vorgesehenen Drucker und Umschlag probeweise gedruckt werden. Für formale Schreiben können außerdem organisatorische oder rechtliche Anforderungen gelten, die nicht Gegenstand dieses Toolkits sind.

## Datenschutz und Demo-Daten

Alle enthaltenen Namen, Anschriften, Kontaktdaten, Kennzeichen und Sachverhalte sind fiktive und neutralisierte Demo-Daten.

Vor der echten Nutzung:

- Absender, Empfänger, Betreff, Brieftext, Links, Referenzen und Anlagen ersetzen;
- das erzeugte PDF prüfen, nicht nur den Quelltext;
- private Referenzen und persönliche Testmaterialien nicht in öffentlichen Repositories veröffentlichen;
- für Screenshots, Beispiele und öffentliche Issue-Berichte ausschließlich fiktive Daten verwenden.

Als Sicherheitsnetz erinnert der Build-Log bei ausgeschaltetem Entwurfsmodus und beim Kompilieren von <code>content.tex</code> daran, wenn der mitgelieferte Demo-Absendername, -Betreff oder -Empfänger noch aktiv ist. Der Hinweis erscheint nur im Log, nie im Brief. Mit <code>\CheckDemoDatafalse</code> lässt er sich abschalten, falls ein Demo-Wert legitim zu deinen Angaben passt.

## Lokaler Build

Voraussetzungen:

- eine LaTeX-Installation mit XeLaTeX;
- <code>latexmk</code>;
- die gewählten Schriften oder eine konfigurierte Ersatzschrift.

Im Projektverzeichnis:

~~~sh
latexmk -xelatex -interaction=nonstopmode -halt-on-error main.tex
~~~

Overleaf ist für den ersten Einstieg empfehlenswert, weil dadurch viele Unterschiede lokaler Installationen entfallen.

## Fehlerbehebung

- Ein `fontspec`-/Schriftfehler bedeutet meist, dass der Compiler auf pdfLaTeX steht; auf XeLaTeX umstellen.
- Wird in Overleaf das falsche Dokument kompiliert, <code>main.tex</code> als Hauptdatei festlegen.
- Unerwartetes Layout oder Fehler entstehen oft durch mehr als eine aktive Form, Vorgabe oder Empfängermethode; genau eine aktiv lassen.
- Abweichende Ergebnisse im lokalen Build sind meist schriftbedingt; siehe den Hinweis zur Ersatzschrift unter Lokaler Build.
- Erscheint noch eine Entwurfswarnung im PDF, ist der Entwurfsmodus aktiv; mit <code>\DraftModefalse</code> abschalten.

## Bekannte Grenzen

- Es wird keine offizielle DIN-Zertifizierung beansprucht.
- Der Legal/Formal-Modus bietet keine Rechtsberatung.
- Barrierefrei getaggte PDFs und PDF/A-Ausgabe werden nicht zugesichert.
- Ältere TeX-Live- oder KOMA-Script-Versionen können eine Prüfung oder Anpassung erfordern.
- Sehr lange Inhalte und umfangreiche optionale Felder benötigen eine manuelle Layoutkontrolle.
- Fortgeschrittene Kombinationen aus Typografie, Farben, Briefköpfen und ungewöhnlich langen Inhalten werden durch den Regressionstest der Vorgaben nicht vollständig abgedeckt.

## Lizenz

LaTeX-Quelltext, Template-Logik und Toolkit-Struktur stehen unter der LPPL-1.3c. Dokumentation, Beispiele und Vorschaumaterial stehen – sofern nicht anders angegeben – unter CC BY 4.0.

Siehe [LICENSE](LICENSE), [LICENSE-CC-BY-4.0](LICENSE-CC-BY-4.0) und [NOTICE](NOTICE).
