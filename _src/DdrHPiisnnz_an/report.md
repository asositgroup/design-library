# Referens tahlili — DdrHPiisnnz

Manba: https://www.instagram.com/reel/DdrHPiisnnz/ | Islomxon Saidov | SAT Mentor (@islomxon.saidov) | like: 949
Izoh: 'Obuna bo‘ling @islomxon.saidov'

## 1. Texnik
- 1080x1920, 50.000 fps, 53.60 s | -14.2 LUFS, LRA 1.4 LU, peak -0.7 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 115 so'z, nutq 48.2 s (90% vaqt), 129 so'z/daq
- Uzun pauzalar (>=0.4 s): 1 ta [0.49]
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 4 kesim, kadr uzunligi: median 9.62 s, min 5.58, max 16.84 (kesim har 10.72 s)
- Kesim-nutq: 3/4 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz
  -    5.58 s — SO'Z ICHIDA ('Bu') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   18.88 s — SO'Z ICHIDA ('rasmi') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   35.72 s — SO'Z ICHIDA ('Bukham') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   43.98 s — pauzada (oldingi so'zdan 0.48 s, keyingisigacha 0.01 s)

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 5.58 | 0.02/0.623/0.992 | 0.371 | 0.212 | 0.065 | 5.79 | SAT -dan 1400 -dan koppal alishigiz chun shu ikte saytda dai |
| 1 | 5.58 | 13.3 | 0.016/0.218/0.618 | 0.192 | 0.394 | 0.116 | 13.15 | ayat etkin saytlarini koppchilik biladi. Tanchalik faydali i |
| 2 | 18.88 | 16.84 | 0.016/0.216/0.618 | 0.189 | 0.404 | 0.121 | 7.97 | platformasi soplanad. Test güni, siz aynan usha platformada  |
| 3 | 35.72 | 8.26 | 0.012/0.202/0.623 | 0.185 | 0.444 | 0.145 | 4.97 | College Board -lar hamkorlikta tuzulgan, hamda mutlaqo biyap |
| 4 | 43.98 | 9.62 | 0.012/0.208/0.623 | 0.184 | 0.446 | 0.144 | 1.55 | Bularini bittasi sizgi bilim deradi, ikincisi, usha bilimlar |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median -15.0 dBFS, pauzalarda -27.7 dBFS → farq 12.7 dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -8.3 dB, nutq polosasi -2.9 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 50 ta, shundan kesimda (±0.15 s): 0 → [2.0, 4.2, 5.8, 6.1, 6.7, 7.5, 8.3, 8.5, 9.0, 10.5, 11.1, 12.7, 13.1, 14.1, 15.7, 18.3, 18.6, 20.7, 21.4, 22.2]
- TODO (Claude): SFX turlari (whoosh/pop/glitch/riser) va qaysi vizual hodisaga bog'langani — tv_*.png to'lqinlarida ko'r.

## 6. Vizual material (KO'R)
- Kontakt: contact_00.jpg, contact_16.jpg, contact_32.jpg, contact_48.jpg
- video-use timeline_view (filmstrip + to'lqin + so'zlar): tv_huk.png, tv_yakun.png, tv_kesim_5.58.png, tv_kesim_18.88.png, tv_kesim_35.72.png, tv_kesim_43.98.png
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
