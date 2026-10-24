# Lesson 1: HTML Basics

## HTML kya hai?

HTML ka matlab hai **HyperText Markup Language**. Darna nahi, ye koi mushkil cheez nahi hai.

Aasan lafzon me: **HTML website ki haddi (skeleton) hai.** Jaise insaan ka jism haddi ke baghair khara nahi ho sakta, waise hi website HTML ke baghair nahi ban sakti. HTML batata hai ke page par kya kya hoga — heading kahan hogi, paragraph kahan hoga, tasveer kahan lagegi.

## Tag kya hota hai?

HTML **tags** se banta hai. Tag ek nishani hoti hai jo angle brackets `< >` me likhi jati hai. Har tag ka ek shuru aur ek khatma hota hai:

```html
<p>Ye ek paragraph hai.</p>
```

- `<p>` — shuru ka tag (paragraph shuru)
- `</p>` — khatme ka tag (slash `/` ka matlab hai "band karo")

## Pehli webpage ki buniyad

Har HTML page ki ye buniyadi banawat hoti hai:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Meri Pehli Website</title>
</head>
<body>
    <h1>Assalam-o-Alaikum!</h1>
    <p>Ye meri pehli webpage hai.</p>
</body>
</html>
```

Samajh lein:
- `<!DOCTYPE html>` — browser ko batata hai ke ye HTML page hai
- `<html>` — poora page iske andar hota hai
- `<head>` — wo maloomat jo nazar nahi aati (jaise page ka title)
- `<title>` — browser ke tab me jo naam nazar aata hai
- `<body>` — wo sab kuch jo screen par nazar aata hai

## Headings (surkhiyan)

Headings 6 size me hoti hain — `h1` sab se bara, `h6` sab se chhota:

```html
<h1>Ye sab se bari heading hai</h1>
<h2>Ye us se chhoti hai</h2>
<h3>Ye aur chhoti hai</h3>
```

## Paragraphs

Aam text ke liye `<p>` tag use hota hai:

```html
<p>Mera naam Tanveen hai.</p>
<p>Main coding seekh raha hoon.</p>
```

## Links (dosri page par jana)

Link banane ke liye `<a>` tag use hota hai. `href` me wo address likhte hain jahan jana hai:

```html
<a href="https://www.google.com">Google par jayein</a>
```

## Images (tasveer lagana)

Tasveer ke liye `<img>` tag use hota hai. Iska koi khatme wala tag nahi hota. `src` me tasveer ka address aur `alt` me tasveer ki wazahat likhte hain (agar tasveer na khule to ye lafz nazar aate hain):

```html
<img src="meri-tasveer.jpg" alt="Meri tasveer">
```

## Lists (fehrist)

**Bullets wali list** (ul = unordered list):

```html
<ul>
    <li>Aam</li>
    <li>Kela</li>
    <li>Angoor</li>
</ul>
```

**Number wali list** (ol = ordered list):

```html
<ol>
    <li>Pehla kaam</li>
    <li>Doosra kaam</li>
    <li>Teesra kaam</li>
</ol>
```

## Mukammal example: Meri pehli webpage

```html
<!DOCTYPE html>
<html>
<head>
    <title>Mera Taaruf</title>
</head>
<body>
    <h1>Mera Naam Tanveen Hai</h1>
    <p>Main Sukkur se hoon aur coding seekh raha hoon.</p>

    <h2>Meri Pasandeeda Cheezein</h2>
    <ul>
        <li>Coding</li>
        <li>Cricket</li>
        <li>Filmein</li>
    </ul>

    <h2>Mera Plan</h2>
    <ol>
        <li>HTML seekhna</li>
        <li>CSS seekhna</li>
        <li>Apni website banana</li>
    </ol>

    <a href="https://www.google.com">Google kholein</a>
</body>
</html>
```

Is code ko Notepad me likhein, file ka naam `index.html` rakhein, phir us par double-click karein — aap ki pehli website browser me khul jayegi!

## Practice exercises

1. Apne baare me ek page banayein: apna naam heading me, apna sheher paragraph me, aur apni 3 hobbies ki list banayein.
2. Us page me apni pasandeeda website ka link lagayein.
3. Apni page me ek tasveer lagayein (koi bhi tasveer, apne computer se ya internet se).

---
**Agla lesson:** [CSS Basics](02-css-basics.md) — is page ko khoobsurat banana seekhein.
