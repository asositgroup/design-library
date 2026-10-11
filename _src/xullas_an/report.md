# Referens tahlili — xullas

## 1. Texnik
- 1920x1080, 24.000 fps, 20.00 s | -9.3 LUFS, LRA 9.5 LU, peak -0.7 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 0 so'z, nutq 0.0 s (0% vaqt), 0 so'z/daq
- Uzun pauzalar (>=0.4 s): 0 ta []
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 0 kesim, kadr uzunligi: median 20.00 s, min 20.00, max 20.00 (kesim har 20.00 s)
- Kesim-nutq: 0/0 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 20.0 | 0.405/0.817/0.908 | 0.125 | 0.175 | 0.101 | 4.95 |  |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median nan dBFS, pauzalarda -6.0 dBFS → farq nan dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -0.6 dB, nutq polosasi -12.3 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 29 ta, shundan kesimda (±0.15 s): 0 → [5.9, 6.4, 7.2, 7.4, 8.0, 8.5, 9.0, 9.3, 10.1, 10.3, 10.6, 11.1, 11.4, 12.2, 12.7, 13.2, 13.5, 14.3, 14.8, 15.3]
- TODO (Claude): SFX turlari (whoosh/pop/glitch/riser) va qaysi vizual hodisaga bog'langani — tv_*.png to'lqinlarida ko'r.

## 6. Vizual material (KO'R)
- Kontakt: contact_00.jpg, contact_16.jpg
- video-use timeline_view (filmstrip + to'lqin + so'zlar): tv_huk.png, tv_yakun.png
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
