# Lesson 3: JavaScript Basics

## JavaScript kya hai?

JavaScript (JS) wo zubaan hai jo website ko **zinda** karti hai.

- HTML = haddi (kya hai)
- CSS = kapray (kaisa dikhega)
- JavaScript = harkat (kya karega)

Jab aap kisi button par click karte hain aur kuch hota hai — message aata hai, rang badalta hai, photo badalti hai — to uske peeche JavaScript hoti hai.

## JavaScript kahan likhte hain?

HTML page ke end par, `</body>` se pehle, `<script>` tag me:

```html
<body>
    <h1>JavaScript Seekhna</h1>
    <script>
        alert("Assalam-o-Alaikum!");
    </script>
</body>
```

`alert()` ek chhota sa popup message dikhata hai. Is page ko kholein to sab se pehle ye message aayega.

## Variables (dabbe)

Variable ek **dabba** hota hai jis me hum koi value rakhte hain taake baad me use kar sakein. `let` se dabba banate hain:

```javascript
let naam = "Tanveen";
let umar = 20;
let seekhRahaHai = true;
```

- `"Tanveen"` — text ko **string** kehte hain (quotes me likhte hain)
- `20` — number hai (baghair quotes)
- `true` — haan/naa wali value ko **boolean** kehte hain

Dabbe ki value baad me badal bhi sakte hain:

```javascript
let score = 0;
score = 10;   // ab score 10 ho gaya
```

## If / Else (shart lagana)

Agar ye ho to ye karo, warna wo karo — iske liye `if` aur `else` use hota hai:

```javascript
let number = 15;

if (number > 10) {
    alert("Number 10 se bara hai!");
} else {
    alert("Number 10 se chhota ya barabar hai.");
}
```

Samajh lein:
- `>` ka matlab hai "se bara"
- `<` ka matlab hai "se chhota"
- `===` ka matlab hai "bilkul barabar"

## Loops (ek kaam baar baar karna)

Agar ek hi kaam 5 dafa karna ho to 5 dafa likhne ki zaroorat nahi — **loop** use karein:

```javascript
for (let i = 1; i <= 5; i++) {
    console.log("Dafa number " + i);
}
```

Samajh lein:
- `let i = 1` — ginti 1 se shuru
- `i <= 5` — jab tak ginti 5 se chhoti ya barabar ho, chalte raho
- `i++` — har dafa ginti me 1 jama karo
- `console.log()` — result browser ke console me dikhata hai (F12 dabba kar dekhein)

## Functions (ek kaam ka packet)

Function ek **packet** hota hai jis me hum kuch kaam band kar dete hain, phir jab chahein us packet ko naam le kar chala lete hain:

```javascript
function salamKaro(naam) {
    alert("Assalam-o-Alaikum, " + naam + "!");
}

salamKaro("Tanveen");  // ye line function ko chalati hai
```

## Mukammal example: Button click

```html
<!DOCTYPE html>
<html>
<head>
    <title>Button Wala Page</title>
</head>
<body>
    <h1 id="heading">Mujhe click karo!</h1>
    <button onclick="rangBadlo()">Rang Badlo</button>

    <script>
        let clickCount = 0;

        function rangBadlo() {
            clickCount = clickCount + 1;
            document.getElementById("heading").style.color = "red";
            document.getElementById("heading").innerText =
                "Tum ne " + clickCount + " dafa click kiya!";
        }
    </script>
</body>
</html>
```

Is me kya ho raha hai:
- Button par click hote hi `rangBadlo()` function chalta hai
- `clickCount` har click par 1 barhta hai
- Heading ka rang surkh ho jata hai aur us me click ki ginti likhi aati hai
- `document.getElementById()` ka matlab hai "page par se wo cheez dhoondo jis ki id ye hai"

## Practice exercises

1. Ek button banayein jis par click karne se "Mubarak ho!" ka alert aaye.
2. Ek variable me apni umar rakhein, phir `if` se check karein: agar umar 18 ya zyada ho to "Aap baray hain" warna "Aap chhotay hain" dikhayein.
3. Loop se 1 se 10 tak ginti console me dikhayein.
4. Ek function banayein jo kisi bhi naam ko le kar "Assalam-o-Alaikum, [naam]!" ka alert dikhaye.

---
**Agla lesson:** [Python Basics](04-python-basics.md) — ek asaan programming zubaan seekhein.
