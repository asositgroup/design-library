# Referens tahlili — DdhCayXMAnN

Manba: https://www.instagram.com/reel/DdhCayXMAnN/ | Islomxon Saidov | SAT Mentor (@islomxon.saidov) | like: 176
Izoh: 'Videoni SAT’ga tayyorlanayotgan tanishingizga yuborib qo‘ying'

## 1. Texnik
- 1080x1920, 29.970 fps, 27.56 s | -14.3 LUFS, LRA 1.9 LU, peak -0.7 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 69 so'z, nutq 22.9 s (83% vaqt), 150 so'z/daq
- Uzun pauzalar (>=0.4 s): 3 ta [0.58, 0.56, 0.43]
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 2 kesim, kadr uzunligi: median 5.64 s, min 4.54, max 17.38 (kesim har 9.19 s)
- Kesim-nutq: 0/2 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz
  -    4.54 s — pauzada (oldingi so'zdan 0.32 s, keyingisigacha 0.26 s)
  -   21.92 s — pauzada (oldingi so'zdan 0.14 s, keyingisigacha 0.18 s)

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 4.54 | 0.02/0.302/0.886 | 0.248 | 0.477 | 0.188 | 6.98 | Istanfona ki, SAT -ni oriyani etkanda en islamaydiyan adat k |
| 1 | 4.54 | 17.38 | 0.012/0.214/0.556 | 0.158 | 0.473 | 0.147 | 3.59 | Birintisi, fakat praiksike otorib qalish, yani irtalibdan ke |
| 2 | 21.92 | 5.64 | 0.012/0.212/0.574 | 0.168 | 0.461 | 0.142 | 3.66 | SAT -ki tayinlanish maqtidi, kuydagi ikiti xatodan kaysi bir |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median -14.4 dBFS, pauzalarda -30.0 dBFS → farq 15.7 dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -9.2 dB, nutq polosasi -2.3 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 30 ta, shundan kesimda (±0.15 s): 0 → [0.6, 0.8, 2.9, 3.7, 4.0, 4.8, 6.0, 7.2, 7.4, 7.9, 8.5, 8.7, 9.2, 9.9, 11.0, 12.3, 13.3, 13.6, 14.0, 15.0]
- TODO (Claude): SFX turlari (whoosh/pop/glitch/riser) va qaysi vizual hodisaga bog'langani — tv_*.png to'lqinlarida ko'r.

## 6. Vizual material (KO'R)
- Kontakt: contact_00.jpg, contact_16.jpg
- video-use timeline_view (filmstrip + to'lqin + so'zlar): tv_huk.png, tv_yakun.png, tv_kesim_4.54.png, tv_kesim_21.92.png
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
