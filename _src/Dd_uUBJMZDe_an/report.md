# Referens tahlili — Dd_uUBJMZDe

Manba: https://www.instagram.com/reel/Dd_uUBJMZDe/ | Islomxon Saidov | SAT Mentor (@islomxon.saidov) | like: 730
Izoh: 'Izohga English deb yozib qoldiring'

## 1. Texnik
- 1080x1920, 29.970 fps, 44.61 s | -14.1 LUFS, LRA 2.0 LU, peak -0.2 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 103 so'z, nutq 40.0 s (90% vaqt), 139 so'z/daq
- Uzun pauzalar (>=0.4 s): 1 ta [0.4]
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 7 kesim, kadr uzunligi: median 3.22 s, min 1.54, max 20.75 (kesim har 5.58 s)
- Kesim-nutq: 1/7 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz
  -    4.17 s — pauzada (oldingi so'zdan 0.25 s, keyingisigacha 0.03 s)
  -   10.08 s — pauzada (oldingi so'zdan 0.28 s, keyingisigacha 0.04 s)
  -   12.35 s — SO'Z ICHIDA ('taqminan') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   14.62 s — pauzada (oldingi so'zdan 0.38 s, keyingisigacha 0.03 s)
  -   20.15 s — pauzada (oldingi so'zdan 0.25 s, keyingisigacha 0.11 s)
  -   21.69 s — pauzada (oldingi so'zdan 0.10 s, keyingisigacha 0.15 s)
  -   23.86 s — pauzada (oldingi so'zdan 0.16 s, keyingisigacha 0.10 s)

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 4.17 | 0.011/0.229/0.718 | 0.224 | 0.582 | 0.203 | 2.67 | Bir sum sarflamasdan SAT English -tan yuqqara bal alishisiri |
| 1 | 4.17 | 5.91 | 0.008/0.106/0.601 | 0.172 | 0.545 | 0.111 | 1.41 | Videon yuqqat qoymasi uchun xaziraq saklabani. SAT English q |
| 2 | 10.08 | 2.27 | 0.033/0.04/0.297 | 0.106 | 0.416 | 0.121 | 2.05 | Bar yoxu torta bolimna ibarat va taqminan |
| 3 | 12.35 | 2.27 | 0.297/0.938/0.951 | 0.159 | 0.091 | 0.083 | 2.02 | 10 taga yaqin soval turu mavcud. |
| 4 | 14.62 | 5.54 | 0.008/0.104/0.596 | 0.169 | 0.541 | 0.107 | 1.36 | Imtikanda sovallar xar sefer yanginanib kilad. Lekim sovalla |
| 5 | 20.15 | 1.54 | 0.014/0.037/0.373 | 0.1 | 0.713 | 0.104 | 2.14 | Xar bir soval turun tartiflan |
| 6 | 21.69 | 2.17 | 0.296/0.922/0.992 | 0.144 | 0.062 | 0.053 | 2.65 | yazib organib çıxsangiz, |
| 7 | 23.86 | 20.75 | 0.008/0.108/0.603 | 0.172 | 0.553 | 0.109 | 2.79 | imtikanda siz kormagan soval turu çıxmaydi. və minnab matinl |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median -14.2 dBFS, pauzalarda -25.3 dBFS → farq 11.1 dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -7.3 dB, nutq polosasi -2.8 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 34 ta, shundan kesimda (±0.15 s): 1 → [1.9, 2.5, 2.8, 3.2, 6.8, 7.6, 8.3, 11.7, 12.0, 13.1, 17.6, 20.3, 20.6, 21.9, 22.2, 22.9, 26.0, 26.2, 26.6, 27.6]
- TODO (Claude): SFX turlari (whoosh/pop/glitch/riser) va qaysi vizual hodisaga bog'langani — tv_*.png to'lqinlarida ko'r.

## 6. Vizual material (KO'R)
- Kontakt: contact_00.jpg, contact_16.jpg, contact_32.jpg
- video-use timeline_view (filmstrip + to'lqin + so'zlar): tv_huk.png, tv_yakun.png, tv_kesim_4.17.png, tv_kesim_10.08.png, tv_kesim_12.35.png, tv_kesim_14.62.png, tv_kesim_20.15.png, tv_kesim_21.69.png, tv_kesim_23.86.png
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
