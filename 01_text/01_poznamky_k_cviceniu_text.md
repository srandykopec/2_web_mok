# Poznámky z hodiny — HTML základy <p> a <h1> až <h6>

---

## 1. Párový vs. nepárový tag

**Párový tag** — má otvárací aj zatvárací tag, medzi nimi je obsah:
```html
<h1>Meno</h1>
<p>Text odseku</p>
```
Zatvárací tag spoznáš podľa lomítka `/` pred názvom — `</h1>`, `</p>`.

**Nepárový tag** — nemá zatvárací tag, nič medzi seba "nepribalí":
```html
<meta charset="UTF-8">
<br>
```

👉 **Skoro všetky tagy, ktoré sme dnes používali (h1, h2, h3, p), sú párové.** Ak zabudneš zatvárací tag, stránka sa môže zobraziť nesprávne alebo neprehľadne.

---

## 2. `<head>` a `<body>` — aký majú význam

| Časť | Význam |
|---|---|
| `<head>` | **Neviditeľná** časť stránky. Návštevník ju na stránke nevidí — obsahuje info *o* stránke (title, meta charset, viewport). |
| `<body>` | **Viditeľná** časť. Všetko, čo je medzi `<body>` a `</body>`, sa zobrazí na obrazovke. |

V dnešnom cvičení bolo v `<head>` navyše aj:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
Toto zabezpečí, že sa stránka správne zobrazí aj na mobile — zapamätaj si ho, budeme ho dávať do každej stránky.

---

## 3. Formátovanie kódu a odsadzovanie

Všimni si v ukážkovom kóde:
- Obsah `<body>` je **odsadený** (tabulátorom) od okrajov — vidno tak, čo je "vnútri čoho".
- Kód je čitateľný aj vďaka **prázdnym riadkom** medzi jednotlivými časťami (napr. medzi jednotlivými sekciami o Wilberforcovi).
- V kóde boli aj **komentáre** — text, ktorý prehliadač ignoruje, slúži len tebe/programátorovi ako poznámka:
```html
<!-- heading 1 úroveň nadpisu 1 -->
```
Komentár sa píše medzi `<!--` a `-->` a **nezobrazí sa** na stránke.

👉 Odsadzovanie a prázdne riadky nemenia to, ako stránka vyzerá v prehliadači — sú tu **len pre teba**, aby si sa v kóde vedel/vedela vyznať a ľahšie našiel/našla chybu.

---

## 4. Element `<p>` (odsek)

```html
<p>
  Text odseku môže byť aj na viacerých riadkoch v kóde...
</p>
```
- Slúži na súvislý text (vety, opis).
- Aj keď text v kóde rozdelíš na viac riadkov, v prehliadači sa zobrazí ako **jeden súvislý odsek** — nový riadok v kóde ≠ nový riadok na stránke.
- Chceš nový, oddelený odsek? Musíš použiť **nový `<p>`**, nie len Enter.

---

## 5. Úrovne nadpisov (h1–h6)

- `<h1>` je **najdôležitejší/najväčší** nadpis, `<h6>` najmenej dôležitý.
- V dnešnej ukážke boli použité `<h1>`, `<h2>` aj `<h3>` — nadpisy takto **členia text na logické časti** (napr. „Politik", „Filantrop", „hlavný iniciátor zrušenia obchodu s otrokmi" boli `<h2>` — podkapitoly v rámci textu o Wilberforcovi).

⚠️ **Všimni si:** v ukážke boli na stránke **dva `<h1>`** (Meno a William Wilberforce). Toto v skutočnosti nie je odporúčaný postup — na stránke by mal byť spravidla **len jeden `<h1>`**, ktorý predstavuje hlavný názov/tému celej stránky. Ak by sme stránku robili poriadne, mali by sme si vybrať jednu hlavnú tému a zvyšok podriadiť ako `<h2>`, `<h3>` atď.

---

## Čo si z dnešného cvičenia odnies

- [ ] Párový tag má otvárací aj zatvárací tag, nepárový nie.
- [ ] `<head>` = neviditeľné info o stránke, `<body>` = to, čo vidí návštevník.
- [ ] Odsadzovanie a komentáre `<!-- -->` sú kvôli prehľadnosti kódu, na zobrazenie stránky nemajú vplyv.
- [ ] `<p>` = odsek; nový riadok v kóde nevytvorí nový odsek na stránke.
- [ ] `<h1>`–`<h6>` = nadpisy podľa dôležitosti; na stránke by mal byť ideálne len jeden `<h1>`.
