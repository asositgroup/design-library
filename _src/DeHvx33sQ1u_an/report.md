# Referens tahlili — DeHvx33sQ1u

Manba: https://www.instagram.com/reel/DeHvx33sQ1u/ | Islomxon Saidov | SAT Mentor (@islomxon.saidov) | like: 1346
Izoh: 'SAT haqida ma’lumotlarni yo‘qotib qo‘ymaslik uchun video’ni saqlab oling @islomxon.saidov'

## 1. Texnik
- 1080x1920, 29.970 fps, 34.77 s | -14.2 LUFS, LRA 2.6 LU, peak -0.7 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 94 so'z, nutq 30.5 s (88% vaqt), 162 so'z/daq
- Uzun pauzalar (>=0.4 s): 4 ta [0.79, 0.41, 0.64, 0.78]
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 0 kesim, kadr uzunligi: median 34.77 s, min 34.77, max 34.77 (kesim har 34.77 s)
- Kesim-nutq: 0/0 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 34.77 | 0.0/0.113/0.767 | 0.187 | 0.514 | 0.108 | 3.79 | SAT -iye uydatun payalanish uchun sayt bar mi? Ha, albat, SA |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median -14.6 dBFS, pauzalarda -39.8 dBFS → farq 25.2 dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -8.6 dB, nutq polosasi -2.6 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 29 ta, shundan kesimda (±0.15 s): 0 → [0.5, 1.1, 3.1, 3.9, 4.1, 5.2, 6.3, 7.5, 9.2, 11.6, 13.3, 13.5, 15.7, 16.6, 19.2, 20.5, 21.3, 21.6, 21.9, 23.3]
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
