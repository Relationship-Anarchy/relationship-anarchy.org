---
title: Mitmachen
description: Du kannst mehr tun, als nur zu lesen...
menu: main
weight: -210
---

Oft liest man in einem Blog nur mit, kommentiert maximal die Beiträge. Dieser Blog soll anders sein. Daher ist das selber Schreiben von Beiträgen sehr willkommen und absolut erwünscht. Und um der _Anarchie_ im Titel hierbei etwas Rechnung zu tragen, wurde die entsprechende Technik verwendet.

Daher basiert dieser Blog auf [hugo](http://gohugo.io), gehostet auf [GitHub](https://github.com), basierend auf einem [öffentlichen Repo](https://github.com/relationship-anarchy/relationship-anarchy.org).

Alles klar? Super, dann mal los... Ich freue mich! - Keine Ahnung? Auch kein Problem...

hugo ist ein sog. Framework. Also unterm Strich eine einfach Art bzw. in diesem Fall ein Programm, um aus vielen Dateien, auf sehr einfache Art, so etwas wie diesen Blog zu basteln. GitHub ist ein Service der die Zusammenarbeit mit sehr vielen Menschen und dem gemeinsamen Arbeiten an verschiedenen Dateien wesentlich komfortabler macht. (Ja, stark vereinfacht dargestellt... Aber die Dienste bieten auf Ihren Seiten auch bereits wesentlich besser Erklärungen. Alternativ hilft die Suchmaschine des Vertrauens sicher weiter. Und wer die Muße hat das ganze besser zu beschreiben oder sogar einen einfacheren Weg kennt... Ich würde mich freuen!)

Solltest Du bereits ein Autor Profil angelegt haben, geht es gleich mit dem [Blog Eintrag](#blog-eintrag) weiter...

Falls dieses Vorgehen zu kompliziert sein sollte, kannst Du Deinen Text auch einfach an [mr.smith@relationship-anarchy.org](mailto:mr.smith@relationship-anarchy.org) senden. Ich kümmere mich dann gerne darum und veröffentliche diesen in Deinem Namen.

-----
##### Autor anlegen

Wenn Du das erste Mal einen Beitrag schreiben willst, benötigst Du erstmal ein Autor Profil. Dies ist jedoch kein Problem und schnell angelegt. Hierzu legen wir in [data/authors](https://github.com/relationship-anarchy/relationship-anarchy.org/tree/master/data/authors) einfache eine entsprechende Datei an. Solltest Du dies direkt über GitHub machen, klicke auf den Link und oben rechts auf **Create new file**. Sollte dieser Button grau hinterlegt sein, musst Du Dich erst einmal bei GitHub einloggen bzw. Dir einen Account erstellen. Dies ist kostenlos und anonym, unter Angabe von Nick und einer E-Mail Adresse (Ihr bekommt eine E-Mail mit Bestätigungslink, der angeklickt werden muss, bevor Änderungen erlaubt sind!) möglich.

{{< figure src="/images/add_author_1.png" >}}

Hinter _relationship-anarchy.org/data/authors/_ ins Feld _Name your file..._ kommt Dein Autor-Name gefolgt von _.toml_, also z.B. _mrsmith_**.toml**. (Bitte alles klein und ohne Leerzeichen, Bindestriche o.ä.)

In das große Feld darunter kommen die Angaben zu Deiner Person. Für mein Profil sieht dies z.B. so aus:

```
id = "mrsmith"

[email]
username = "mr.smith"
host = "relationship-anarchy.org"

[name]
display = "Mr. Smith"

[social]
email = ""
facebook = ""
twitter = ""
```

- **id** ist hierbei die ID, die Du in Deinen Beiträgen angibst, damit dieser Dir zugeordnet werden kann. Idealer Weise verwendest Du hier die gleiche Bezeichnung wie beim Dateinamen (ohne .toml).
- **username** ist der Teil einer E-Mail Adresse vor dem @.
- **host** der Teil der E-Mail Adresse nach dem @.
- **display** ist der Name, wie er bei euren Beiträgen angezeigt wird.

{{< figure src="/images/add_author_2.png" >}}


Im ersten Feld unter **Propose new file** können wir nun noch eine kurz sog. _commit message_ eingeben. Also einer Erwähnung was wir getan haben. Im Feld darunter gibt es die Möglichkeit des optionalen, ausführlicheren Erklärung.

Mit einem Klick auf den grünen **Propose new file** Button, wird diese Datei erstmal in eurem Account angelegt. Mit einem zwei Klicks auf jeweils den grünen Button **Create pull request** sendest Du die Datei dann ans eigentliche Repo.

{{< figure src="/images/add_author_3.png" >}}
{{< figure src="/images/add_author_4.png" >}}

Damit ist die Datei angelegt und wartet darauf von einem Teammitglied bestätigt zu werden. In diesem Zustand kann diese Änderung von Dir und jedem anderen natürlich noch kommentiert und diskutiert werden. Jedoch sollte eine Übernahme der Datei gewöhnlich umgehend erfolgen!

{{< figure src="/images/add_author_5.png" >}}

-----
##### Blog Eintrag

Du hast Deinen Autor Account gerade eben oder bereits in der Vergangenheit angelegt? Super! Dann geht es nun ans Schreiben eines Beitrages.

Neue Beiträge werden, ähnlich wie die Autorenprofile, ebenfalls einfach als Datei angelegt. Die gehören jedoch in [content/blog](https://github.com/relationship-anarchy/relationship-anarchy.org/tree/master/content/blog). Hier erwartet uns, nach einem Klick auf den **Create new file** Button, oben rechts, wieder das gewohnte Bild.

{{< figure src="/images/add_entry_1.png" >}}

Als Titel für den Dateinamen nehmen wir die Überschrift unseres geplanten Beitrages, Leerzeichen durch Bindestriche ersetzt und die Endung **.md** angehängt. -> _mein-erster-beitrag_**.md**

Das große Feld darunter wird mit dem Beitrag an sich gefüllt...

```
---
date: 2018-01-07T20:05:10+01:00
title: Mein erster Beitrag
authors: ["mrsmith"]
---

HIER KOMMT MEIN TEXT...

Und noch viel mehr davon... Einfach immer weiter... Wie man halt
seinen Text schreibt.
```

Zwischen den --- sind die Angaben für den Beitrag selbst.

- **date** ist das Datum eures Beitrages im Format _**2018-01-07**T**20:05:10**+01:00_ für den 07.01.2018 um 20:05 Uhr und 10 Sekunden. Einfach von hinten nach vorne gelesen. Wobei es hier auf eine halbe Stunde nicht ankommt...
- **title** ist der Titel eures Beitrages, wie dieser anzeigt werden soll.
- **authors** ist eure Autor ID, oben angelegt unter dem Punkt **ID**. Hier wäre es auch möglich mehrere Autoren anzugeben. Dies wäre dann z.B. ["**mrsmith**","**anarchist**"] für die Autoren ID's **mrsmith** und **anarchist**.

Unter den abschließenden drei Bindestrichen fangt ihr dann einfach euren Text an und speichert diesen, wie bereits beim Autor geschehen. (Grünen Button klicken, bis _Comment_ darauf steht...)

-----

Wie gesagt... Ist dieses Vorgehen zu kompliziert, gerne den Text einfach an [mr.smith@relationship-anarchy.org](mailto:mr.smith@relationship-anarchy.org). Ich veröffentliche diesen dann, in Deinem Namen. Falls bessere Vorschläge bestehen, auch diese sehr gerne! ;-)
