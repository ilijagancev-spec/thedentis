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
4. Страницата ќе биде на `https://<корисничко-име>.github.io/thedentis/`

## ⚠️ ЗАДОЛЖИТЕЛНО пред објавување

1. **Заменете го доменот** во сите датотеки — placeholder е `vivastar-kavadarci.github.io`:
   ```bash
   cd ~/projects/thedentis
   grep -rl "vivastar-kavadarci.github.io" . | xargs sed -i '' 's/vivastar-kavadarci.github.io/<вистинскиот-домен>/g'
   ```
2. **Проверете ја е-поштата** — ставена е `vivstarng@gmail.com` како placeholder. Ако вистинската адреса е друга:
   ```bash
   grep -rl "vivstarng@gmail.com" . | xargs sed -i '' 's/vivstarng@gmail.com/вистинска@адреса/g'
   ```
3. Потврдете телефон (070 396 301), адреса (бул. Македонија 3-ж) и работно време (пон–пет 08–20).

## По објавувањето

- Пријавете го sitemap-от во [Google Search Console](https://search.google.com/search-console): додајте го сајтот и поднесете `sitemap.xml`.
- Ставете го линкот на страницата во Google Business Profile и на Facebook страницата.
- Кога ќе имате сопствен домен (пр. vivastar.mk), додајте CNAME во Settings → Pages.

## Локален SEO — следни чекори (од конкурентската анализа)

1. **Ажурирајте го zk.mk профилот** (zk.mk/viva-star) — телефонот таму (070 396301) е точен, но работното време е старо — ажурирајте го на пон–пет 08–20. Конзистентни податоци (NAP) насекаде го креваат локалното рангирање.
2. Исто проверете: Google Business Profile и Facebook да имаат идентичен телефон/адреса/време како сајтот.
3. **Ценовник**: ниту еден од 12 проверени стоматолошки сајтови во МК нема објавено цени — ако објавите макар ориентациски ценовник, се издвојувате веднаш.
4. **Google рецензии на сајтот**: само drjolevski.com (Охрид) ги прикажува — секцијата „Рецензии" е подготвена, пратете ги текстовите од вашите вистински Google рецензии за да се вградат.
5. Блог 1×месечно (совети за заби) — во Кавадарци само Фуџи Дент има блог.
