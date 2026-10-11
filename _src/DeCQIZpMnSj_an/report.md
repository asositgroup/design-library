# Referens tahlili — DeCQIZpMnSj

Manba: https://www.instagram.com/reel/DeCQIZpMnSj/ | Islomxon Saidov | SAT Mentor (@islomxon.saidov) | like: 665
Izoh: 'Toshkentdagi eng qimmat maktab'

## 1. Texnik
- 1080x1920, 29.970 fps, 45.08 s | -14.2 LUFS, LRA 1.9 LU, peak -0.5 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 90 so'z, nutq 38.3 s (85% vaqt), 120 so'z/daq
- Uzun pauzalar (>=0.4 s): 5 ta [0.67, 0.83, 0.81, 1.75, 0.63]
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 0 kesim, kadr uzunligi: median 45.08 s, min 45.08, max 45.08 (kesim har 45.08 s)
- Kesim-nutq: 0/0 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 45.08 | 0.008/0.126/0.664 | 0.158 | 0.531 | 0.016 | 2.13 | Oshkendegi eni qamat khususi maytab xaysi. Inventor Internat |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median -14.1 dBFS, pauzalarda -21.7 dBFS → farq 7.6 dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -5.8 dB, nutq polosasi -3.7 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 25 ta, shundan kesimda (±0.15 s): 0 → [1.8, 4.5, 5.0, 5.4, 10.1, 10.6, 11.1, 13.9, 15.1, 16.9, 17.4, 18.0, 20.1, 22.8, 26.0, 26.7, 27.0, 29.0, 29.9, 31.5]
- TODO (Claude): SFX turlari (whoosh/pop/glitch/riser) va qaysi vizual hodisaga bog'langani — tv_*.png to'lqinlarida ko'r.

## 6. Vizual material (KO'R)
- Kontakt: contact_00.jpg, contact_16.jpg, contact_32.jpg
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
