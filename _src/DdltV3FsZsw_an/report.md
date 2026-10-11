# Referens tahlili — DdltV3FsZsw

Manba: https://www.instagram.com/reel/DdltV3FsZsw/ | Jason Pro (@jasonp.media) | like: 402285
Izoh: 'Catch the flow with M4⬜️.\n\n🚙: @g82rey \n🎥: @jasonp.media \n\n#bmw #m4 #m4competition'

## 1. Texnik
- 1080x1920, 60.000 fps, 18.02 s | -14.2 LUFS, LRA 2.5 LU, peak -3.5 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 3 so'z, nutq 0.7 s (4% vaqt), 10 so'z/daq
- Uzun pauzalar (>=0.4 s): 0 ta []
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 2 kesim, kadr uzunligi: median 6.00 s, min 6.00, max 6.02 (kesim har 6.01 s)
- Kesim-nutq: 0/2 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz
  -    6.02 s — nutqsiz joyda
  -   12.02 s — nutqsiz joyda

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 6.02 | 0.066/0.392/0.731 | 0.192 | 0.303 | 0.13 | 19.02 | Altyazı M .K. |
| 1 | 6.02 | 6.0 | 0.103/0.355/0.875 | 0.266 | 0.304 | 0.13 | 19.26 |  |
| 2 | 12.02 | 6.0 | 0.034/0.392/0.711 | 0.203 | 0.366 | 0.172 | 15.64 |  |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median -16.8 dBFS, pauzalarda -12.2 dBFS → farq -4.7 dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -1.6 dB, nutq polosasi -7.0 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 20 ta, shundan kesimda (±0.15 s): 0 → [0.4, 1.9, 3.4, 4.9, 6.4, 6.6, 7.9, 8.1, 9.4, 9.6, 10.9, 11.1, 12.4, 12.6, 13.9, 14.1, 15.4, 15.6, 16.9, 17.1]
- TODO (Claude): SFX turlari (whoosh/pop/glitch/riser) va qaysi vizual hodisaga bog'langani — tv_*.png to'lqinlarida ko'r.

## 6. Vizual material (KO'R)
- Kontakt: contact_00.jpg, contact_16.jpg
- video-use timeline_view (filmstrip + to'lqin + so'zlar): tv_huk.png, tv_yakun.png, tv_kesim_6.02.png, tv_kesim_12.02.png
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
