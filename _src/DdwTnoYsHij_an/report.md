# Referens tahlili — DdwTnoYsHij

Manba: https://www.instagram.com/reel/DdwTnoYsHij/ | Islomxon Saidov | SAT Mentor (@islomxon.saidov) | like: 320
Izoh: 'Videoni tanishlaringizga yuborib qo’ying'

## 1. Texnik
- 1080x1920, 50.000 fps, 61.30 s | -14.3 LUFS, LRA 2.2 LU, peak -0.6 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 132 so'z, nutq 49.9 s (81% vaqt), 129 so'z/daq
- Uzun pauzalar (>=0.4 s): 8 ta [0.59, 0.71, 0.61, 1.13, 2.51, 0.55, 0.45, 0.6]
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 4 kesim, kadr uzunligi: median 4.54 s, min 1.92, max 42.60 (kesim har 12.26 s)
- Kesim-nutq: 3/4 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz
  -    8.74 s — pauzada (oldingi so'zdan 0.24 s, keyingisigacha 0.12 s)
  -   51.34 s — SO'Z ICHIDA ('Misallarini') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   54.84 s — SO'Z ICHIDA ('YouTube') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   59.38 s — SO'Z ICHIDA ('azib') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 8.74 | 0.012/0.29/0.686 | 0.187 | 0.495 | 0.214 | 4.51 | SST -nin matematiki qismidi, musallarinin ishlarisdini bir n |
| 1 | 8.74 | 42.6 | 0.012/0.435/0.988 | 0.367 | 0.262 | 0.101 | 1.92 | Bu musallini kobu haqqetadigan usul orqala ishlidiyan busik, |
| 2 | 51.34 | 3.5 | 0.012/0.285/0.629 | 0.169 | 0.47 | 0.19 | 1.89 | xudusundi, oson islansini korumakchi usayengiz, YouTube |
| 3 | 54.84 | 4.54 | 0.158/0.96/0.992 | 0.218 | 0.11 | 0.093 | 6.22 | kanalimda video darsiglari bo. Olus uchun, izoklardi YouTube |
| 4 | 59.38 | 1.92 | 0.235/0.327/0.992 | 0.233 | 0.727 | 0.671 | 4.6 | qalirik, ve siz gibi borup koyalım. |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median -14.9 dBFS, pauzalarda -33.0 dBFS → farq 18.1 dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -8.1 dB, nutq polosasi -2.8 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 58 ta, shundan kesimda (±0.15 s): 0 → [0.1, 2.2, 3.0, 4.3, 5.4, 6.4, 6.9, 9.1, 10.3, 11.3, 11.5, 12.4, 13.0, 14.8, 15.3, 15.5, 16.8, 17.0, 17.6, 19.3]
- TODO (Claude): SFX turlari (whoosh/pop/glitch/riser) va qaysi vizual hodisaga bog'langani — tv_*.png to'lqinlarida ko'r.

## 6. Vizual material (KO'R)
- Kontakt: contact_00.jpg, contact_16.jpg, contact_32.jpg, contact_48.jpg
- video-use timeline_view (filmstrip + to'lqin + so'zlar): tv_huk.png, tv_yakun.png, tv_kesim_8.74.png, tv_kesim_51.34.png, tv_kesim_54.84.png, tv_kesim_59.38.png
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
