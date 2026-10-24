# Lesson 4: Python Basics

## Python kya hai?

Python ek programming zubaan hai jo **sab se aasan** mani jati hai. Iska code parhne me aam English jaisa lagta hai, is liye beginners ke liye ye behtareen shuruaat hai.

Python se websites, apps, games, aur data ka kaam — sab kuch hota hai. Aaj duniya ki bari companies (Google, Netflix, Instagram) bhi Python use karti hain.

## Print (screen par likhna)

Sab se pehla program — screen par kuch likhna:

```python
print("Assalam-o-Alaikum!")
print("Main Python seekh raha hoon.")
```

`print()` ka matlab hai "screen par dikhao". Jo quotes `" "` ke andar likhenge, wo waise ka waisa nazar aayega.

## Variables (dabbe)

JavaScript ki tarah, Python me bhi variables **dabbe** hote hain. Farq sirf ye hai ke yahan `let` likhne ki zaroorat nahi:

```python
naam = "Tanveen"
umar = 20
lambai = 5.8
```

- `"Tanveen"` — string (text)
- `20` — integer (poora number)
- `5.8` — float (dashamlah wala number)

## Input (user se poochna)

User se kuch poochne ke liye `input()` use hota hai:

```python
naam = input("Aap ka naam kya hai? ")
print("Assalam-o-Alaikum, " + naam + "!")
```

User jo likhega, wo `naam` dabbe me chala jayega.

## If / Else (shart lagana)

```python
number = 15

if number > 10:
    print("Number 10 se bara hai!")
else:
    print("Number 10 se chhota ya barabar hai.")
```

**Zaroori baat:** Python me brackets `{ }` nahi hote. Us ki jagah **space (indentation)** kaam aata hai — `if` ke baad wali lines ko thora aage (4 spaces) likhna zaroori hai. Agar space galat hoga to program nahi chalega.

Aur zyada shartein lagani hon to `elif` use karein (else + if ka milap):

```python
marks = 75

if marks >= 80:
    print("Grade: A")
elif marks >= 60:
    print("Grade: B")
elif marks >= 40:
    print("Grade: C")
else:
    print("Grade: Fail")
```

## Loops (ek kaam baar baar karna)

**For loop** — jab pata ho ke kitni dafa karna hai:

```python
for i in range(1, 6):
    print("Dafa number", i)
```

`range(1, 6)` ka matlab hai 1 se 5 tak (aakhri number 6 shamil nahi hota).

**While loop** — jab tak shart poori ho, chalte raho:

```python
ginti = 1
while ginti <= 3:
    print("Ginti:", ginti)
    ginti = ginti + 1
```

## Mukammal example: Marks se grade batane wala program

```python
print("=== Grade Checker ===")

naam = input("Aap ka naam likhein: ")
marks = int(input("Aap ke marks likhein (0-100): "))

if marks >= 80:
    grade = "A"
elif marks >= 60:
    grade = "B"
elif marks >= 40:
    grade = "C"
else:
    grade = "Fail"

print(naam + ", aap ka grade hai: " + grade)
```

Samajh lein:
- `int(input(...))` — user se number lena. `int` ka matlab hai ke jo likha gaya usay number samjho (warna wo text samjha jayega).
- Program marks dekh kar grade nikalta hai aur naam ke saath dikhata hai.

## Practice exercises

1. Ek program likhein jo user se uska naam aur sheher pooch kar ye dikhaye: "Mera naam [naam] hai aur main [sheher] se hoon."
2. Ek program likhein jo user se umar pooch kar bataye ke wo vote de sakta hai ya nahi (18 ya zyada = haan).
3. Loop se 1 se 10 tak table (pehra) banayein — jaise 2 ka pehra: 2, 4, 6, 8...
4. Grade checker program me ye izafa karein: agar marks 90 ya zyada hon to "A+ aur Mubarak ho!" dikhaye.

---
**Mubarak ho!** Aap ne 4 lessons mukammal kar liye — HTML, CSS, JavaScript aur Python ki buniyad aap ke paas hai. Ab apna pehla chhota project banayein, chahe wo ek apni website ho ya ek chhota program. Wapas [README](README.md) par jayein.
