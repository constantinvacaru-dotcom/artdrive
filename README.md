# ArtDrive.MD — Site web

Site de prezentare (o pagină), bilingv RO/RU, pentru atelierul auto ArtDrive.MD
(îndreptare caroserie, vopsire, polisare).

## Structura fișierelor
```
artdrive-site/
├── index.html      # conținutul paginii
├── styles.css      # design (negru / roșu / alb)
├── script.js       # comutator limbă, meniu mobil, galerie, animații
├── favicon.svg     # iconița din tab-ul browserului
├── server.js       # server local pentru testare (nu e necesar la găzduire)
├── gallery/        # AICI pui pozele lucrărilor: 1.jpg, 2.jpg ... 6.jpg
└── README.md
```

## ✅ Ce trebuie completat înainte de publicare

### 1. Pozele lucrărilor (galerie)
Pune 6 poze în folderul `gallery/`, denumite exact:
`1.jpg`, `2.jpg`, `3.jpg`, `4.jpg`, `5.jpg`, `6.jpg`
Dacă lipsesc, site-ul afișează automat un placeholder elegant (nu se strică).
Recomandat: poze orizontale (4:3), max ~1600px lățime, sub 500 KB fiecare.

### 2. Formularul „Cere ofertă"
În `index.html`, la `<form ... action="https://formsubmit.co/CHANGE_ME@example.com">`
înlocuiește `CHANGE_ME@example.com` cu adresa de email a atelierului.
Serviciul FormSubmit e gratuit; la prima trimitere vei primi un email de confirmare — apasă linkul o singură dată ca să activezi.

### 3. Harta locației
În `index.html`, la `<iframe ... src="https://www.google.com/maps?q=Chișinău&output=embed">`
înlocuiește `Chișinău` cu adresa exactă (ex. `Strada Exemplu 10, Chișinău`).

### 4. Verifică datele de contact
Telefon și WhatsApp sunt setate la **068 171 799** (`tel:+37368171799`, `wa.me/37368171799`).
Program: „Luni – Sâmbătă: 09:00 – 18:00" — ajustează în `index.html` / `script.js` dacă diferă.

## 🌐 Publicare gratuită (Netlify — cel mai simplu)
1. Intră pe https://app.netlify.com/drop
2. Trage tot folderul `artdrive-site` în pagină.
3. Gata — primești un link de forma `nume-aleatoriu.netlify.app`.
4. (Opțional) Din *Site settings → Domain* poți conecta un domeniu propriu, ex. `artdrive.md`.

## 🔧 Testare locală
```
node artdrive-site/server.js
# apoi deschide http://localhost:4321
```
