# TUTORIAL COMPLET — site-ul tău de fotografie

De la folderul pe care îl ai acum, până la un site live pe internet, cu domeniul tău.
Nu trebuie să știi să programezi. Ai nevoie doar de un browser și de răbdare 30 de minute.

---

## CUPRINS

1. [Ce ai primit](#1-ce-ai-primit)
2. [Deschide site-ul pe calculatorul tău](#2-deschide-site-ul-pe-calculatorul-tău)
3. [Pune-ți pozele](#3-pune-ți-pozele)
4. [Schimbă textele](#4-schimbă-textele)
5. [Adaugă sau șterge poze din galerie](#5-adaugă-sau-șterge-poze-din-galerie)
6. [Fă formularul de contact să funcționeze](#6-fă-formularul-de-contact-să-funcționeze)
7. [Publică site-ul pe internet](#7-publică-site-ul-pe-internet) — 3 metode
8. [Domeniul tău propriu](#8-domeniul-tău-propriu)
9. [Google, SEO și clienți noi](#9-google-seo-și-clienți-noi)
10. [Cum actualizezi site-ul după publicare](#10-cum-actualizezi-site-ul-după-publicare)
11. [Checklist final înainte de lansare](#11-checklist-final-înainte-de-lansare)
12. [Probleme frecvente](#12-probleme-frecvente)
13. [Ce poți schimba la design](#13-ce-poți-schimba-la-design)

---

## 1. Ce ai primit

```
site/
├── index.html          ← pagina principală (Home)
├── portfolio.html      ← galeria cu filtre + lightbox
├── about.html          ← despre tine + cum lucrezi
├── services.html       ← pachete, prețuri, întrebări frecvente
├── contact.html        ← formular + date de contact
├── 404.html            ← pagina care apare la link-uri greșite
├── favicon.svg         ← iconița din tab-ul browserului
├── robots.txt          ← pentru Google
├── sitemap.xml         ← pentru Google
├── TUTORIAL.md         ← fișierul ăsta
├── assets/
│   ├── css/style.css   ← TOT designul (culori, fonturi, spațieri)
│   └── js/main.js      ← meniu mobil, filtre, lightbox
└── images/             ← toate pozele (acum sunt placeholdere)
```

**Reguli de aur:**

- Nu redenumi folderele `assets` și `images`. Dacă le muți, se strică linkurile.
- `index.html` trebuie să rămână cu numele ăsta. Este pagina pe care internetul o deschide prima.
- Fă o copie a folderului înainte de modificări mari. E gratis și te salvează.

---

## 2. Deschide site-ul pe calculatorul tău

Dublu-click pe `index.html`. Se deschide în browser și funcționează complet — meniu, galerie, lightbox, tot.

**Ca să editezi fișierele ai nevoie de un editor de text.** Nu folosi Word. Recomand, în ordine:

- **Visual Studio Code** — gratuit, [code.visualstudio.com](https://code.visualstudio.com). Cel mai bun. Colorează codul, îți arată greșelile.
- **Notepad++** (Windows) sau **TextEdit** în modul Plain Text (Mac) — merg și ele.
- La nevoie, chiar Notepad-ul din Windows.

În VS Code: `File → Open Folder` → alegi folderul `site`. Vezi toate fișierele în stânga.

> **Trucul care îți economisește ore:** ține site-ul deschis în browser într-un tab. După fiecare modificare salvată (`Ctrl+S` / `Cmd+S`), dai `F5` în browser și vezi imediat rezultatul.

---

## 3. Pune-ți pozele

Asta e cea mai importantă parte. Un site de fotograf este 90% pozele lui.

### 3.1 Metoda simplă (recomandată)

Fiecare placeholder din folderul `images/` are scris pe el ce trebuie să pui acolo și în ce dimensiune.
**Nu schimba numele fișierelor.** Redenumește poza ta exact cum se numește placeholderul și suprascrie-l.

Exemplu: ai o poză grozavă de la un concert → o redenumești `hero.jpg` → o pui peste cea din `images/`. Gata. Nu trebuie să atingi niciun cod.

### 3.2 Ce poză merge unde

| Fișier | Unde apare | Format | Ce să pui |
|---|---|---|---|
| `hero.jpg` | Prima imagine, tot ecranul | orizontal, foarte lat | Cea mai puternică poză a ta. De la un concert, cu lumini. Lasă loc gol în partea de jos-stânga, acolo vine textul mare. |
| `cat-concerts.jpg` | Card categorie | vertical 4:5 | Un artist pe scenă |
| `cat-portraits.jpg` | Card categorie | vertical 4:5 | Cel mai bun portret |
| `cat-events.jpg` | Card categorie | vertical 4:5 | Un moment de la o nuntă/botez |
| `featured-1.jpg` | Secțiunea neagră | vertical 4:5 | Portret puternic |
| `featured-2.jpg` | Secțiunea neagră | orizontal | Concert |
| `featured-3.jpg` | Pagina About | orizontal | Detaliu / atmosferă |
| `footer.jpg` | Fundal la banda finală | orizontal | Apus, lumini, ceva cu atmosferă. Apare la 38% opacitate, deci nu trebuie să fie perfect clară. |
| `about.jpg` | Pagina About | vertical 4:5 | **O poză cu tine.** Obligatoriu. Oamenii vor să vadă cine vine la evenimentul lor. |
| `about-2.jpg` | Pagina About | orizontal | Tu la lucru, cu aparatul în mână |
| `portrait-1..8.jpg` | Galerie | vertical | Portrete |
| `concert-1..7.jpg` | Galerie | orizontal | Concerte și festivaluri |
| `event-1..6.jpg` | Galerie | orizontal | Nunți, botezuri, evenimente |

### 3.3 Pregătirea pozelor — nu sări peste pasul ăsta

Un JPEG direct din Lightroom are 8–15 MB. Dacă pui 20 de poze așa, site-ul se încarcă în 40 de secunde și oamenii pleacă. Iar Google te penalizează.

**Ce trebuie:**

1. **Redimensionează** — latura lungă la **2000 px** e mai mult decât suficient pentru web. Pentru pozele din galerie, 1600 px e perfect.
2. **Salvează la calitate 75–82%** (în Lightroom: Export → JPEG → Quality 80, Limit File Size 400 K).
3. **Ținta: sub 400 KB per poză.** Hero-ul poate merge până la 600 KB.
4. **Nume fișier fără diacritice, fără spații, cu litere mici.** `concert-1.jpg` da, `Poză Concert 1.JPG` nu.

**Unelte gratuite dacă nu ai Lightroom:**

- [squoosh.app](https://squoosh.app) — tragi poza în browser, alegi calitatea, vezi diferența live, descarci. Cel mai bun.
- [tinypng.com](https://tinypng.com) — tragi până la 20 de poze deodată, îți dă înapoi versiuni mai mici.

> **Watermark?** Părerea mea: nu pe tot, e urât. Dacă vrei, pune-l discret în colț, la 30% opacitate. Oricine vrea să-ți fure poza o va face oricum; ce contează e ca poza să arate bine.

### 3.4 Dacă vrei să folosești alte nume de fișiere

Deschizi fișierul `.html`, cauți `images/` și schimbi numele. De exemplu în `index.html`:

```html
<img src="images/hero.jpg" alt="Crowd lit by stage lights at a festival">
```

devine

```html
<img src="images/concert-untold-2026.jpg" alt="Mulțime la Untold, lumini de scenă">
```

**Schimbă și textul din `alt=`.** Ăla descrie poza pentru Google și pentru cine nu vede imaginea. Contează la SEO.

---

## 4. Schimbă textele

Deschizi fișierul `.html` în editor și scrii peste. Textul este între paranteze ascuțite, tu modifici doar ce e **între** ele:

```html
<h1>The last song before the lights go out</h1>
     ↑ pe ăsta îl schimbi        ↑ pe astea nu le atingi
```

### 4.1 Lucrurile pe care TREBUIE să le schimbi

Caută în **toate** fișierele `.html` (în VS Code: `Ctrl+Shift+F` caută în tot folderul) și înlocuiește:

| Caută | Înlocuiește cu |
|---|---|
| `+40 700 000 000` | numărul tău real de telefon |
| `instagram.com/USERNAME` | linkul tău real de Instagram |
| `facebook.com/USERNAME` | linkul tău real de Facebook |
| `REPLACE-WITH-YOUR-DOMAIN.com` | domeniul tău, după ce îl cumperi (pasul 8) |
| `YOUR CITY` | orașul tău (în `contact.html`) |
| `from €XXX` | prețurile tale reale (în `services.html`) |
| `Client name` | numele real al clienților care ți-au lăsat recenzii (în `index.html`) |
| `ingradufrant@gmail.com` | dacă vrei altă adresă de email pentru clienți |

> **Sfat serios despre prețuri:** ori pui prețuri reale, ori scoți complet coloana cu prețuri. „from €XXX" pe un site live arată neterminat și pierzi clientul. Dacă nu vrei să afișezi prețuri, șterge liniile `<span class="price">from &euro;XXX</span>` din `services.html` — restul rămâne aranjat.

### 4.2 Textele de vânzare — scrie-le tu

Textele pe care le-am scris sunt un punct de plecare bun, dar sunt ale mele, nu ale tale. Rescrie-le cu vocea ta. Trei sfaturi:

- **Vorbește despre client, nu despre tine.** „Ai o zi pe care nu o repeți" bate „Am 10 ani experiență".
- **Concret bate general.** „48 de ore până la primele poze" bate „livrare rapidă".
- **Scurt.** Nimeni nu citește trei paragrafe pe un site de fotografie. Se uită la poze.

### 4.3 Titlul din tab și descrierea pentru Google

Sus, în fiecare fișier, între `<head>` și `</head>`:

```html
<title>Radu Frantz — Concert, Festival & Portrait Photographer</title>
<meta name="description" content="...">
```

`<title>` = ce scrie în tabul browserului și ce vede lumea în Google, cu litere albastre.
`<meta name="description">` = textul gri de sub el în Google. Maxim 155 caractere.

Pune în ele orașul tău: **„Fotograf concerte și portrete — Cluj-Napoca"** te găsește mult mai ușor decât „Photographer".

---

## 5. Adaugă sau șterge poze din galerie

Deschide `portfolio.html` și caută secțiunea `<div class="gallery">`. Fiecare poză e un bloc de o linie:

```html
<figure data-cat="concerts">
  <img src="images/concert-1.jpg" alt="Singer under stage lights" loading="lazy">
  <figcaption>Festival — main stage</figcaption>
</figure>
```

- **Ca să adaugi o poză:** copiază tot blocul `<figure>...</figure>`, lipește-l dedesubt și schimbă `src`, `alt` și textul din `figcaption`.
- **Ca să ștergi o poză:** șterge tot blocul, de la `<figure` până la `</figure>`.
- **`data-cat`** decide sub ce filtru apare. Valori posibile: `concerts`, `portraits`, `events`. Scrise exact așa, cu litere mici.
- Ordinea din cod = ordinea pe site. Pune cele mai bune poze primele.

Filtrele, lightboxul și aranjarea în coloane se ocupă singure. Nu trebuie să atingi nimic altceva.

**Câte poze?** 20–30 în total e ideal. 15 poze foarte bune bat 60 de poze bunicele. Un client se uită la primele 10 și decide.

---

## 6. Fă formularul de contact să funcționeze

Acum, formularul arată bine dar nu trimite nimic nicăieri. Un fișier HTML pur nu poate trimite emailuri singur — are nevoie de un serviciu. Ambele variante de mai jos sunt gratuite.

### Varianta A — Formspree (merge pe orice hosting)

1. Intri pe [formspree.io](https://formspree.io) și îți faci cont gratuit.
2. `+ New Form` → îi dai un nume → pui emailul unde vrei să primești mesajele.
3. Îți dă o adresă de forma `https://formspree.io/f/abcdwxyz`.
4. Deschizi `contact.html`, cauți:
   ```html
   <form class="form" data-contact method="POST" action="REPLACE_WITH_FORM_ENDPOINT">
   ```
   și înlocuiești `REPLACE_WITH_FORM_ENDPOINT` cu adresa ta:
   ```html
   <form class="form" data-contact method="POST" action="https://formspree.io/f/abcdwxyz">
   ```
5. Salvezi. Gata. Primul mesaj trimis îți cere să confirmi adresa de email, o singură dată.

Planul gratuit: 50 de mesaje pe lună. Suficient.

### Varianta B — Netlify Forms (doar dacă publici pe Netlify)

Și mai simplu. În `contact.html`, schimbi linia formularului în:

```html
<form class="form" data-contact method="POST" name="contact" data-netlify="true" action="/">
```

Atât. Netlify prinde automat mesajele. Le vezi în panoul lor, la `Forms`, și poți seta notificare pe email.

### Anti-spam

Formularul are deja o „capcană" invizibilă (câmpul `_gotcha`). Roboții o completează, oamenii nu. Nu o șterge — blochează majoritatea spamului fără să ceară nimic clienților tăi.

---

## 7. Publică site-ul pe internet

Trei metode. Îți recomand **A**, dacă nu ai motive să alegi altceva.

---

### METODA A — Netlify (gratis, 2 minute, cea mai simplă)

**De ce asta:** e gratuit, HTTPS automat, site-ul se încarcă rapid oriunde în lume, și publici trăgând un folder cu mouse-ul.

1. Intri pe **[app.netlify.com/drop](https://app.netlify.com/drop)**
2. **Tragi folderul `site` întreg** din calculator în pătratul din pagină. Nu fișiere individual — tot folderul.
3. Aștepți ~20 de secunde. Primești o adresă de forma `https://sparkly-cupcake-a1b2c3.netlify.app`.
4. **Site-ul tău e live.** Poți deja să dai linkul cuiva.
5. Îți faci cont gratuit (butonul care apare) ca să nu pierzi site-ul și ca să poți conecta domeniul tău.
6. Schimbă adresa aiurea: `Site configuration → Site details → Change site name` → pui `radufrantz` și devine `radufrantz.netlify.app`.

**Ca să actualizezi mai târziu:** `Deploys` → tragi din nou folderul în zona de drop. Se înlocuiește tot, în 20 de secunde.

---

### METODA B — GitHub Pages (gratis, bun dacă vrei istoric al modificărilor)

**De ce asta:** păstrează fiecare versiune a site-ului, poți da înapoi oricând. Un pic mai mulți pași.

1. Cont gratuit pe [github.com](https://github.com).
2. `New repository` → nume: `radufrantz.github.io` (**exact numele tău de utilizator** + `.github.io`) → **Public** → `Create`.
3. În pagina repository-ului: `uploading an existing file` → tragi **conținutul** folderului `site` (fișierele și folderele dinăuntru, nu folderul în sine).
4. Jos: `Commit changes`.
5. `Settings` → `Pages` → la `Branch` alegi `main` și `/ (root)` → `Save`.
6. Aștepți 1–3 minute. Site-ul e la `https://radufrantz.github.io`.

**Ca să actualizezi:** intri în repository, `Add file → Upload files`, tragi fișierele modificate, `Commit changes`.

---

### METODA C — Hosting clasic cu cPanel (dacă ai deja gazdă plătită)

**Când folosești asta:** ai deja hosting cumpărat de la un furnizor (Hostico, Romarg, GoDaddy, Hostinger etc.), sau vrei totul la un singur loc cu domeniul.

**Prin File Manager (fără programe suplimentare):**

1. Intri în cPanel (de obicei `https://domeniultau.ro/cpanel` sau linkul primit pe email).
2. `File Manager` → intri în folderul **`public_html`**.
3. Dacă e ceva acolo (o pagină „Coming soon" a gazdei), șterge.
4. `Upload` → încarci **conținutul** folderului `site`.
   - Mai rapid: fă un `.zip` cu tot conținutul, încarcă zipul, apoi click dreapta pe el → `Extract`. Șterge zipul după.
5. Verifici că `index.html` stă direct în `public_html`, nu într-un subfolder.
6. Deschizi `https://domeniultau.ro`. Site-ul e acolo.

**Prin FTP (pentru încărcări mari, mai stabil):**

1. Descarci [FileZilla](https://filezilla-project.org) (gratuit).
2. Datele FTP le găsești în emailul de la gazdă sau în cPanel → `FTP Accounts`.
3. Te conectezi: Host, Username, Password, Port `21`.
4. În dreapta intri în `public_html`, în stânga deschizi folderul `site`, selectezi tot conținutul și tragi în dreapta.

**HTTPS (lacătul verde):** în cPanel caută `SSL/TLS Status` sau `Let's Encrypt` și activează certificatul gratuit. Fără el, browserul scrie „Not secure" lângă adresa ta și pierzi clienți.

---

## 8. Domeniul tău propriu

`radufrantz.netlify.app` funcționează, dar `radufrantz.ro` arată ca un profesionist.

### 8.1 Cumpără domeniul

Costă 10–50 lei pe an pentru `.ro`, în jur de 12€ pe an pentru `.com`.

- **`.ro`** — [rotld.ro](https://rotld.ro) sau prin orice gazdă românească. Cel mai bun dacă lucrezi în România.
- **`.com`** — [namecheap.com](https://namecheap.com), [porkbun.com](https://porkbun.com). Mai bun dacă țintești festivaluri și clienți din afară.
- Alternative bune pentru fotografi: `.photo`, `.studio`, `.foto`.

**Cum alegi numele:** scurt, ușor de dictat la telefon, fără cratime dacă se poate. `radufrantz.ro` bate `radu-frantz-photography-cluj.ro`.

### 8.2 Conectează-l la Netlify

1. În Netlify: `Domain management` → `Add a domain` → scrii `radufrantz.ro` → `Verify` → `Add domain`.
2. Netlify îți arată ce trebuie configurat. Ai două variante:

   **Varianta simplă — nameservere:** Netlify îți dă 4 adrese de forma `dns1.p01.nsone.net`. Intri în contul de unde ai cumpărat domeniul, cauți `Nameservers` / `DNS` și le înlocuiești pe cele existente cu astea 4.

   **Varianta clasică — records:** în zona DNS a domeniului adaugi:
   - `A` record, host `@`, valoare `75.2.60.5`
   - `CNAME` record, host `www`, valoare `numele-tau.netlify.app`

3. Aștepți. Propagarea DNS durează între 10 minute și 24 de ore. E normal, nu ai stricat nimic.
4. Când e gata, în `Domain management` → `HTTPS` → `Verify DNS configuration` → `Provision certificate`. Gratuit, automat.
5. **După ce domeniul merge:** întoarce-te în fișierele `.html`, `robots.txt` și `sitemap.xml` și înlocuiește peste tot `REPLACE-WITH-YOUR-DOMAIN.com` cu domeniul real. Republici. Contează pentru Google și pentru cum arată linkul pe WhatsApp.

### 8.3 Email cu domeniul tău

`contact@radufrantz.ro` arată mult mai bine decât un Gmail pe cărțile de vizită.
Cea mai ieftină variantă: [improvmx.com](https://improvmx.com) — gratuit, redirecționează `contact@radufrantz.ro` către Gmailul tău. Varianta serioasă: Google Workspace, ~6€/lună.

---

## 9. Google, SEO și clienți noi

Site-ul nu aduce clienți dacă nu îl găsește nimeni. Astea sunt lucrurile care chiar contează, în ordinea impactului:

### 9.1 Google Search Console (obligatoriu, 5 minute)

1. [search.google.com/search-console](https://search.google.com/search-console) → `Add property` → domeniul tău.
2. Confirmi că e al tău (dacă ai domeniul pe Netlify, metoda cu record DNS e cea mai simplă).
3. `Sitemaps` → scrii `sitemap.xml` → `Submit`.

Din momentul ăsta Google știe de tine și îți arată pe ce cuvinte te găsește lumea.

### 9.2 Google Business Profile (cel mai mare impact local)

[business.google.com](https://business.google.com) — gratuit. Așa apari pe hartă și în căutări de tipul „fotograf nunți Cluj". Pentru un fotograf care lucrează local, ăsta aduce mai mulți clienți decât site-ul în sine. Pune poze, orar, link către site și **cere recenzii clienților mulțumiți.**

### 9.3 Cuvintele care contează

Google nu te caută după „photographer" dacă clienții tăi scriu „fotograf concerte". Pune în titluri și texte exact ce ar scrie un client:

- „fotograf concerte [orașul tău]"
- „fotograf festival România"
- „ședință foto portret [orașul tău]"
- „fotograf nuntă [orașul tău]"

Nu le înghesui artificial. Scrie natural, dar folosește cuvintele reale.

### 9.4 Restul

- **`alt=` la fiecare poză** — descrie ce e în ea. Google „citește" pozele doar așa.
- **Viteza** — pozele optimizate (pasul 3.3) sunt cel mai mare factor. Testează pe [pagespeed.web.dev](https://pagespeed.web.dev).
- **Instagram → site** — pune linkul în bio. Traficul de acolo e cel mai calificat pe care îl vei avea.
- **Răbdare** — Google indexează în 1–4 săptămâni. Nu te panica în prima săptămână.

---

## 10. Cum actualizezi site-ul după publicare

Ciclul e mereu același:

1. Modifici fișierele **local**, pe calculatorul tău.
2. Verifici în browser (dublu-click `index.html`, apoi `F5` după fiecare salvare).
3. Republici:
   - **Netlify:** `Deploys` → tragi din nou folderul.
   - **GitHub Pages:** `Add file → Upload files` → `Commit`.
   - **cPanel/FTP:** încarci doar fișierele modificate, peste cele vechi.

> **Foarte important:** păstrează mereu folderul local ca sursă de adevăr. Nu edita direct pe server, ajungi să nu mai știi ce versiune e cea bună.

**Ritm sănătos:** actualizează portofoliul o dată la 2–3 luni, cu cele mai bune poze de la ce ai fotografiat între timp. Un site care nu se schimbă niciodată arată abandonat.

---

## 11. Checklist final înainte de lansare

Bifează tot înainte să dai linkul lumii:

- [ ] Toate placeholderele înlocuite cu pozele mele (niciun dreptunghi colorat rămas)
- [ ] Toate pozele sub 400 KB
- [ ] Numărul de telefon real, peste tot
- [ ] Linkurile de Instagram și Facebook merg
- [ ] Adresa de email e corectă și o verific
- [ ] Prețurile sunt reale, sau coloana e ștearsă
- [ ] Recenziile sunt reale, cu nume reale (cu acordul lor)
- [ ] `REPLACE-WITH-YOUR-DOMAIN.com` înlocuit peste tot
- [ ] Formularul de contact e conectat și **l-am testat trimițând un mesaj către mine**
- [ ] Am deschis site-ul pe telefon și arată bine
- [ ] Am dat click pe fiecare link din meniu și din footer
- [ ] Titlurile din tab (`<title>`) au orașul meu în ele
- [ ] Lacătul de HTTPS apare lângă adresă
- [ ] Am trimis linkul unui prieten să-l verifice cu ochi proaspeți

---

## 12. Probleme frecvente

**Pozele nu apar, văd doar iconițe rupte.**
99% din cazuri e numele fișierului. Verifică literele mari/mici — `Concert-1.JPG` și `concert-1.jpg` sunt fișiere diferite pe server, chiar dacă pe Windows par la fel. Fă totul cu litere mici.

**Site-ul arată fără stil, ca un document Word.**
Nu găsește `style.css`. Verifică să existe folderul `assets/css/` și fișierul înăuntru. Cel mai des se întâmplă când ai încărcat folderul `site` în loc de **conținutul** lui.

**Am publicat pe cPanel și apare pagina gazdei.**
`index.html` nu e direct în `public_html`, e într-un subfolder. Mută-l.

**Am modificat ceva și nu se vede pe site.**
Browserul ține versiunea veche în memorie. `Ctrl+F5` (Windows) sau `Cmd+Shift+R` (Mac) — reîncarcă forțat.

**Meniul de pe telefon nu se deschide.**
Nu găsește `main.js`. Verifică folderul `assets/js/`.

**Formularul nu trimite nimic.**
Ai lăsat `REPLACE_WITH_FORM_ENDPOINT` neschimbat. Vezi pasul 6.

**Domeniul nu merge nici după 2 ore.**
Normal. DNS-ul poate dura până la 24 de ore. Verifică pe [dnschecker.org](https://dnschecker.org) dacă s-a propagat.

**Am stricat ceva și nu știu ce.**
De asta faci copie de siguranță înainte de modificări. Dacă nu ai făcut: pe GitHub ai istoricul complet, pe Netlify ai `Deploys` cu toate versiunile anterioare și un buton de restaurare.

---

## 13. Ce poți schimba la design

Tot designul stă în variabilele de la începutul fișierului `assets/css/style.css`. Schimbi acolo o valoare și se schimbă în tot site-ul, pe toate paginile:

```css
:root {
  --ink:   #0a0a0a;   /* negrul principal */
  --paper: #ffffff;   /* fundalul alb */
  --red:   #ff0000;   /* accentul roșu — cercuri, linii, hover */
  --mute:  #6f6f6f;   /* textul gri secundar */
}
```

Vrei accent portocaliu în loc de roșu? Schimbi `--red: #ff0000;` în `--red: #ff5c00;` și gata, tot site-ul.

**Fonturile** — tot acolo:

```css
--font-display: "Archivo Black", ...;   /* titlurile mari */
--font-body:    "Archivo", ...;         /* textul normal */
```

Dacă vrei alt font, îl alegi de pe [fonts.google.com](https://fonts.google.com), copiezi linia `<link>` pe care ți-o dă și o pui în `<head>`-ul fiecărei pagini, în locul celei existente. Apoi schimbi numele aici.

**Panglicile înclinate** (elementul-semnătură din design) — clasa `.ribbon` în CSS. `transform: rotate(-2.2deg)` e înclinarea. Viteza textului care se mișcă: `animation: slide 34s` — număr mai mic, derulare mai rapidă.

**Cercurile roșii** — clasa `.badge`. Le muți cu `.badge--tr` (sus-dreapta), `.badge--br` (jos-dreapta), `.badge--bl` (jos-stânga).

---

## Ordinea în care aș face-o eu

1. Pune-ți pozele (pasul 3). Doar asta transformă site-ul din șablon în site-ul tău.
2. Schimbă telefonul, Instagramul, orașul (pasul 4.1).
3. Publică pe Netlify (pasul 7A). Ai deja ceva live, în 2 minute.
4. Conectează formularul (pasul 6) și testează-l.
5. Rescrie textele cu vocea ta (pasul 4.2), fără grabă.
6. Cumpără domeniul și conectează-l (pasul 8).
7. Google Search Console + Google Business Profile (pasul 9).

Nu încerca să faci tot într-o zi. Publică-l imperfect și îmbunătățește-l pe parcurs — un site live imperfect aduce clienți, unul perfect care stă pe calculatorul tău nu aduce niciunul.

Baftă.
