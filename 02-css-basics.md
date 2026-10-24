# Lesson 2: CSS Basics

## CSS kya hai?

CSS ka matlab hai **Cascading Style Sheets**.

Pichle lesson me hum ne HTML se website ki **haddi** banayi thi. Ab CSS se hum us haddi par **kapray pehnayenge** — matlab rang, size, font aur style denge. HTML batata hai ke page par **kya** hai, CSS batata hai ke wo **kaisa dikhega**.

## CSS kahan likhte hain?

Sab se aasan tareeqa: HTML page ke `<head>` ke andar `<style>` tag me likhte hain:

```html
<!DOCTYPE html>
<html>
<head>
    <title>CSS Seekhna</title>
    <style>
        h1 {
            color: blue;
        }
    </style>
</head>
<body>
    <h1>Ye heading ab neeli ho jayegi!</h1>
</body>
</html>
```

Samajh lein:
- `h1` — kis cheez ko style dena hai (isko **selector** kehte hain)
- `{ }` — in brackets ke andar style likhte hain
- `color: blue;` — ye ek **property** hai (color) aur uski **value** hai (blue)
- Har line ke end par semicolon `;` lagana zaroori hai

## Rang (colors)

Rang 3 tareeqon se de sakte hain — naam se, ya code se:

```css
p {
    color: red;            /* naam se */
    background-color: #FFFF00;  /* code se (peela rang) */
}
```

Aam rangon ke naam: `red`, `blue`, `green`, `black`, `white`, `orange`, `purple`, `pink`.

## Fonts (likhayi ki shakal)

```css
h1 {
    font-family: Arial, sans-serif;
    font-size: 30px;
    text-align: center;
}
```

- `font-family` — lafzon ki shakal (Arial, Verdana waghera)
- `font-size` — lafzon ka size (px = pixels)
- `text-align` — text kidhar ho: `left`, `center` ya `right`

## Box Model (sab se zaroori concept)

Har cheez jo page par nazar aati hai, wo ek **dabba (box)** hoti hai. Us dabbe ke 4 hisse hote hain, andar se bahar ki taraf:

1. **Content** — asal cheez (text ya tasveer)
2. **Padding** — content aur border ke darmiyan khaali jagah
3. **Border** — dabbe ki deewar (line)
4. **Margin** — dabbe ke bahar ki khaali jagah (doosre dabbon se faasla)

```css
div {
    padding: 20px;              /* andar ki jagah */
    border: 2px solid black;    /* deewar */
    margin: 10px;               /* bahar ki jagah */
}
```

Seedha yaad rakhein: **padding andar ki saans hai, margin bahar ki doori hai.**

## Class aur ID

Jab aap chahein ke sirf kuch khaas cheezon ko style mile, to class ya id use karte hain:

- **Class** (`.` se shuru) — ek se zyada cheezon par lag sakti hai
- **ID** (`#` se shuru) — sirf ek cheez par lagti hai

```html
<style>
    .sabz {
        color: green;
    }
    #khaas {
        color: red;
        font-size: 25px;
    }
</style>

<p class="sabz">Ye paragraph sabz hoga.</p>
<p class="sabz">Ye bhi sabz hoga.</p>
<p id="khaas">Ye khaas paragraph surkh hoga.</p>
```

## Mukammal example: Styled page

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mera Styled Page</title>
    <style>
        body {
            background-color: lightyellow;
            font-family: Arial, sans-serif;
        }
        h1 {
            color: darkblue;
            text-align: center;
        }
        .dabba {
            background-color: white;
            padding: 20px;
            border: 2px solid darkblue;
            margin: 20px;
        }
    </style>
</head>
<body>
    <h1>Mera Khoobsurat Page</h1>
    <div class="dabba">
        <p>Ye text ek safed dabbe ke andar hai.</p>
        <p>CSS ne is page ko kitna acha bana diya!</p>
    </div>
</body>
</html>
```

## Practice exercises

1. Apne Lesson 1 wale page par CSS lagayein: heading ko apne pasandeeda rang me karein aur center me le aayein.
2. Ek paragraph ko class de kar uska rang aur font-size badlein.
3. Ek dabba (div) banayein jis me padding, border aur margin teeno hon — phir values badal kar dekhein ke kya farq parta hai.

---
**Agla lesson:** [JavaScript Basics](03-javascript-basics.md) — page ko click aur action ke saath zinda karein.
