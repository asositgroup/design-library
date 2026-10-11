# Referens tahlili — Dd9EucloCBH

Manba: https://www.instagram.com/reel/Dd9EucloCBH/ | Ubaydullayev Rasul | Visual Editor (@smoothbeey) | like: 675
Izoh: 'Montajingiz uchun top 5 music🎵\n\n#music #content #création #edit'

## 1. Texnik
- 1080x1920, 30.000 fps, 29.23 s | -14.2 LUFS, LRA 7.2 LU, peak -0.0 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 16 so'z, nutq 6.1 s (21% vaqt), 33 so'z/daq
- Uzun pauzalar (>=0.4 s): 1 ta [22.41]
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 2 kesim, kadr uzunligi: median 3.57 s, min 2.77, max 22.90 (kesim har 9.74 s)
- Kesim-nutq: 1/2 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz
  -    3.57 s — pauzada (oldingi so'zdan 0.45 s, keyingisigacha 21.96 s)
  -   26.47 s — SO'Z ICHIDA ('xarle') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 3.57 | 0.0/0.154/0.977 | 0.233 | 0.561 | 0.145 | 7.67 | Монтажлари дзенаян зорчуцчу, чу шу 5 -ti muzikani ishlatim. |
| 1 | 3.57 | 22.9 | 0.068/0.405/0.93 | 0.228 | 0.612 | -0.043 | 12.57 | Дзенаян xuzi xarle |
| 2 | 26.47 | 2.77 | 0.008/0.154/0.687 | 0.169 | 0.73 | 0.187 | 9.24 | kartetichun, sakhifamge abunubob qoyim. |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median -19.2 dBFS, pauzalarda -14.7 dBFS → farq -4.5 dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -2.1 dB, nutq polosasi -6.7 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 29 ta, shundan kesimda (±0.15 s): 0 → [0.7, 2.2, 3.2, 4.4, 8.1, 8.4, 9.3, 10.6, 11.9, 13.9, 14.4, 14.6, 15.3, 15.5, 16.0, 16.4, 16.9, 17.5, 17.8, 18.1]
- TODO (Claude): SFX turlari (whoosh/pop/glitch/riser) va qaysi vizual hodisaga bog'langani — tv_*.png to'lqinlarida ko'r.

## 6. Vizual material (KO'R)
- Kontakt: contact_00.jpg, contact_16.jpg
- video-use timeline_view (filmstrip + to'lqin + so'zlar): tv_huk.png, tv_yakun.png, tv_kesim_3.57.png, tv_kesim_26.47.png
- Har element kirishi uchun 18 kadrlik strip: `ffmpeg -ss T -t 0.62 -i v.mp4 -vf scale=216:-1,tile=9x2:padding=2 -frames:v 1 s.jpg`

## 7. STYLE.md uchun to'liq ro'yxat (hamma jihat — har birini to'ldir)
- [ ] Umumiy taassurot va janr (video-use: avval qara, keyin taxmin qil)
- [ ] Tuzilma/beat'lar + vaqtlar (2-bo'lim)
- [ ] Montaj ritmi va kesim hunari: J/L-cut, pauzada kesim, spiker almashinuvi oralig'i (3-bo'lim)
- [ ] Kompozitsiya va xavfsiz zonalar (yuz qayerda, matn qayerda)
- [ ] Tipografiya: shrift nomzodlari, o'lcham, ierarxiya, holat (CAPS/kichik)
- [ ] Ranglar (hex) va grade (4-bo'lim raqamlari)
- [ ] Matn/subtitr: bo'laklash (1/2/3 so'z/gap), joylashuv, urg'u usullari
- [ ] Grafik elementlar: har biri kirish/turish/chiqish vaqti (kadr strip bilan o'lcha)
- [ ] O'tishlar
- [ ] Kamera: push/zoom/tebranish (harakat ustuni)
- [ ] B-roll: turi, ulushi, manbasi, qoidalarimizga mosligi (odamlar, mualliflik huquqi)
- [ ] CTA va yakun
- [ ] Audio: musiqa turi/darajasi, SFX lug'ati, nutq-musiqa farqi (5-bo'lim)
- [ ] Silliqlik moslamasi (smooth-motion.md qiymatlari)
- [ ] HyperFrames retsepti
