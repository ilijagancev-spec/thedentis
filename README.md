# Viva Star — веб-страница (GitHub Pages)

Статична двојазична страница за Стоматолошка ординација „Вива Стар", Кавадарци.

- `/` — македонски (главна)
- `/en/` — англиски
- `assets/` — лого, фотографии (лиценцирани Shutterstock + ваши)
- `sitemap.xml`, `robots.txt`, `llms.txt` — SEO + AI-агенти
- JSON-LD structured data (Dentist + FAQPage) во двете страници

## Објавување на GitHub Pages

1. Направете нов репозиториум на github.com, на пример со име `thedentis`.
2. Во терминал:
   ```bash
   cd ~/projects/thedentis
   git init && git add -A && git commit -m "Viva Star website"
   git branch -M main
   git remote add origin https://github.com/<ВАШЕТО-КОРИСНИЧКО-ИМЕ>/thedentis.git
   git push -u origin main
   ```
3. На GitHub: Settings → Pages → Source: `main` / root → Save.
4. Страницата ќе биде на `https://<корисничко-име>.github.io/thedentis/`, а по поврзување на доменот — на `https://vivastar-dentistry.com/`

## Домен: vivastar-dentistry.com

Сите URL-а во датотеките веќе покажуваат на **https://vivastar-dentistry.com/** и има `CNAME` датотека за GitHub Pages.

**Чекори за поврзување:**
1. Купете го доменот (Namecheap, Porkbun или Cloudflare Registrar — ~$10/год за .com).
2. Кај регистраторот, во DNS поставки додајте:
   - 4 × `A` записи за `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` запис за `www` → `<корисничко-име>.github.io`
3. На GitHub: Settings → Pages → Custom domain → внесете `vivastar-dentistry.com` → Save, па штиклирајте **Enforce HTTPS** (се појавува по неколку минути).

Проверете и: е-пошта vivstarng@gmail.com (точно спелување?), телефон 070 396 301, работно време пон/вто/чет 09–17, сре/пет 12–20.

## По објавувањето

- Пријавете го sitemap-от во [Google Search Console](https://search.google.com/search-console): додајте го сајтот и поднесете `sitemap.xml`.
- Ставете го линкот на страницата во Google Business Profile и на Facebook страницата.
- Кога ќе имате сопствен домен (пр. vivastar.mk), додајте CNAME во Settings → Pages.

## Локален SEO — следни чекори (од конкурентската анализа)

1. **Ажурирајте го zk.mk профилот** (zk.mk/viva-star) — телефонот таму (070 396301) е точен, но работното време е старо — ажурирајте го на пон/вто/чет 09–17, сре/пет 12–20. Конзистентни податоци (NAP) насекаде го креваат локалното рангирање.
2. Исто проверете: Google Business Profile и Facebook да имаат идентичен телефон/адреса/време како сајтот.
3. **Ценовник**: ниту еден од 12 проверени стоматолошки сајтови во МК нема објавено цени — ако објавите макар ориентациски ценовник, се издвојувате веднаш.
4. **Google рецензии на сајтот**: само drjolevski.com (Охрид) ги прикажува — секцијата „Рецензии" е подготвена, пратете ги текстовите од вашите вистински Google рецензии за да се вградат.
5. Блог 1×месечно (совети за заби) — во Кавадарци само Фуџи Дент има блог.
