# Katalog Recepat – Astro + Tailwind CSS

![Astro](https://img.shields.io/badge/Astro-5.15.3-blue?logo=astro)  
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-4.1.17-blue?logo=tailwind-css)  
![License](https://img.shields.io/badge/License-MIT-green)

Jednostavan **katalog recepata** napravljen u **Astro 5** koristeći **Tailwind CSS 4.1.17**.  
Omogućava prikaz liste recepata na početnoj stranici i detaljan prikaz svakog recepta koristeći Markdown fajlove.

---

## 🚀 Pokretanje projekta

1. Kloniraj repozitorij i instaliraj zavisnosti:

```bash
git clone <tvoj-repo-url>
cd recipe-catalog
npm install
```

2. Pokreni razvojni server:

```bash
npm run dev
```

3. Otvori u browseru:

```text
http://localhost:4321
```

---

## 🗂️ Struktura projekta

```text
src/
├─ components/      # RecipeCard, Header, Footer
├─ layouts/         # BaseLayout
├─ pages/           # index.astro + recipes/[slug].astro
├─ data/recipes/    # Markdown fajlovi sa receptima
└─ styles/          # global.css
```

---

## 📝 Dodavanje novih recepata

1. Kreiraj Markdown fajl u `src/data/recipes/`:

```markdown
---
title: "Ime recepta"
slug: "ime-recepta"
prepTime: "15 min"
cookTime: "30 min"
servings: 2
image: "/images/ime-slike.jpg"
tags: ["tag1", "tag2"]
---

## Sastojci
- sastojak 1
- sastojak 2

## Uputstvo
1. Korak 1
2. Korak 2
```

2. Slika treba da se nalazi u `public/images/`.

---

## 🎨 Tehnologije

- [Astro 5](https://astro.build/) – Static Site Generator  
- [Tailwind CSS 4.1.17](https://tailwindcss.com/) – Utility-first CSS framework  
- Markdown – za sadržaj recepata  
- Vite – bundler koji dolazi sa Astro  

---

## 📂 Komponente

- `RecipeCard.astro` – kartica recepta sa slikom, naslovom i tagovima  
- `Header.astro` – navigacija  
- `Footer.astro` – footer sa copyright informacijama  
- `BaseLayout.astro` – layout sa `<head>` i globalnim CSS-om  

---

## 🔧 Preporuke

- Dodaj više Markdown recepata u `src/data/recipes/`  
- Slike stavi u `public/images/`  
- Možeš dodati filtere ili search po tagovima na početnoj stranici  

---

## 📄 License

MIT © 2025 – svi fajlovi su slobodni za korišćenje i prilagođavanje.

