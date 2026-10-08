# Java III — Klinika e CSS: shpëto afishen

Kjo detyrë ndërton një afishe të aksesueshme për një aktivitet të klubit të
debatit.

## Çfarë u realizua

- `index.html` përmban titullin, datën, vendin, përshkrimin dhe lidhjen e
  regjistrimit.
- `style.css` është skedar i jashtëm dhe përdor klasa të ripërdorshme,
  variabla CSS dhe `box-sizing: border-box`.
- Tre etiketat dallohen edhe pa ngjyrë: `Falas`, `Vende të kufizuara: 20` me
  vijë të ndërprerë dhe `Edhe online` me tekst të theksuar.
- `:focus-visible` paraqet një kontur të dukshëm kur përdoret tastiera.
- Afisha përshtatet me ekranet e ngushta dhe nuk del jashtë një viewport-i
  360px.
- `gabime.css` dokumenton dhe rregullon konfliktin e selektorëve dhe
  tejkalimin e gjerësisë pa përdorur `!important`.

## Reflektim

Në kaskadë fiton `#poster`, sepse një selektor ID ka specifikë më të lartë se
selektori i klasës `.poster`. Megjithatë, zgjidhja përdor vlera të
njëjta dhe madhësi elastike në të dy rregullat, në mënyrë që specifika të mos
shkaktojë tekst të bardhë mbi sfond të bardhë ose overflow.

## Hapja

Nga folderi `JavaIII`:

```sh
python -m http.server 8000
```

Pastaj hap `http://127.0.0.1:8000/`.
