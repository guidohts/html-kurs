# HTML-Kurs

Gute Quellen im Internet sind:

[W3 Schools](https://www.w3schools.com)

[Self HTML](https://wiki.selfhtml.org)

## Grundstruktur

Du findest die Grundstruktur für ein HTML Dokument in [leer.html](leer.html)

Beachte:

- Es gibt genau ein `html`
- Unterhalb von html gibt es genau **ein** `head` und **ein** `body`

- Der Titel der Seite steht im Tag `title` und darf nur im `head` vorkommen. Er wird in der in der Titelleiste des Browsers angezeigt und nicht auf der Seite selbst.

## Wichtige Tags

`<p>Das ist ein Absatz</p>`
Absätze dürfen nicht geschachtelt werden.

`<div>Das ist ein Abschnitt</div>`
Abschnitte dürfen geschachtelt werden:

`<div><div>Das ist ein Abschnitt</div></div>`

`<img src="images/puppies/puppie_1961613.png" alt="puppy">`
So kannst du ein Bild einfügen. Das Attribut `alt` ist wichtig, weil dieser Text angezeigt wird, falls das Bild nicht geladen werden kann. Wichtig ist es auch für Blinde, die Bilder nicht sehen können, aber sich den Text vorlesen lassen.

`<a href="leer.html">Leer</a>`
Ein Link zu einer andere Seite auf deiner Website. `<a>`steht für Anker.

`<a href="https://www.hochtaunusschule.de">Hochtaunusschule</a>`
Ein Link zu einer externen Seite.

```html
<table>
    <tr>
        <th>Überschrift 1</th>
        <th>Überschrift 2</th>
    </tr>
    <tr>
        <td>Zelle 1</td>
        <td>Zelle 2</td>
    </tr>
    <tr>
        <td>Zelle 3</td>
        <td>Zelle 4</td>
    </tr>
</table>
```

Eine Tabelle


## Formatierung

Du kannst deine Seite mit Cascading Style Sheets (CSS) formatieren.

Dabei gibt es verschiedene Möglichkeiten:

### Inline-Stil

`<p style="color: red;">Mein Absatz</p>`

Du kannst den Stil direkt im HTML Element mit dem Attribut `style` angeben.

Für kleine Stilangaben kann man das machen. Für umfangreichere Formatierungen wird das schnell unübersichtlich.

### `<style>`-Tag

Duu kannst innerhalb von `<head>` ein `<style>`-Tag vereinbaren, und dort alle deine Stile einbauen:

```html
<style>
    p: color: red;
</style>
```


#### Adressierungsarten

Du kannst alle HTML-Elemente desselben Typs gleichzeitig formatieren:

```html
<style>
    p: color: red;
    div: color: blue;
</style>
```

Du kannst jedes Element in deinem HTML mit einer `id` versehen, und diese `id` im CSS ansprechen. `id` muss eindeutig sein.

```html
<style>
    #absatz1: color: red;
</style>

...

<p id="absatz1">Mein Absatz</p>
```

Du kannst Klassen definieren. Diese Klassen kannst du beliebigen Elementen zuweisen. 

```html
<style>
    .rot: color: red;
</style>

...

<p class="red">Mein Absatz</p>
<div class="red">Mein Abschnitt</div>
```


## Hosting mit GitHub

Du kannst die Webseite abrufen unter [https://guidohts.github.io/html-kurs](https://guidohts.github.io/html-kurs/)
