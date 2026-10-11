# Referens tahlili — tabassum_v2

## 1. Texnik
- 1080x1920, 30.000 fps, 32.00 s | -14.0 LUFS, LRA 2.9 LU, peak -1.5 dBFS

## 2. Tuzilma (transkript — `edit/takes_packed.md`)
- 73 so'z, nutq 26.2 s (82% vaqt), 137 so'z/daq
- Uzun pauzalar (>=0.4 s): 2 ta [1.15, 1.36]
- TODO (Claude): takes_packed.md ni o'qib beat'larga ajrat — HUK / MUAMMO / DALIL / XULOSA / CTA (video-use arxetiplari) va har beat vaqti.

## 3. Montaj (kesimlar)
- 11 kesim, kadr uzunligi: median 2.26 s, min 0.50, max 6.00 (kesim har 2.67 s)
- Kesim-nutq: 9/11 so'z ichida (ovoz kesimdan o'tadi), qolgani pauzada/nutqsiz
  -    5.30 s — SO'Z ICHIDA ('Agar') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -    7.70 s — SO'Z ICHIDA ('sabab') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   13.70 s — pauzada (oldingi so'zdan 0.70 s, keyingisigacha 0.45 s)
  -   14.20 s — SO'Z ICHIDA ('Xazirgi') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   16.33 s — SO'Z ICHIDA ('bu') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   18.73 s — pauzada (oldingi so'zdan 1.00 s, keyingisigacha 0.36 s)
  -   22.40 s — SO'Z ICHIDA ('xovaqani') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   23.50 s — SO'Z ICHIDA ('ne') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   27.50 s — SO'Z ICHIDA ('daim') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   29.47 s — SO'Z ICHIDA ('As') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)
  -   30.37 s — SO'Z ICHIDA ('As') — nutq kesimdan o'tadi (J/L-cut yoki B-roll ostida ovoz)

## 4. Grade va harakat (har kadr, o'rtadagi kadr)
| # | vaqt | uzun | luma p2/p50/p98 | kontrast | to'yinganlik | iliq(R-B) | harakat | so'zlar |
|---|---|---|---|---|---|---|---|---|
| 0 | 0.00 | 5.3 | 0.006/0.147/0.783 | 0.221 | 0.407 | 0.019 | 7.53 | Payqambarimizdi daim soqa salam alib gelishkanda, ular bu sa |
| 1 | 5.30 | 2.4 | 0.005/0.177/0.823 | 0.218 | 0.513 | 0.071 | 10.96 | ular sadaqa deyib jawab berisi almastila, sabab |
| 2 | 7.70 | 6.0 | 0.018/0.264/0.808 | 0.239 | 0.421 | 0.044 | 11.46 | -i sadaqa en muqtaq adamgi veriladi, eqsanisi barkcayi beris |
| 3 | 13.70 | 0.5 | 0.01/0.271/0.811 | 0.214 | 0.351 | 0.048 | 26.72 | Xazirgi |
| 4 | 14.20 | 2.13 | 0.0/0.239/0.871 | 0.216 | 0.103 | -0.008 | 3.64 | gunda xamma bitin arsayi muqtaq, bu |
| 5 | 16.33 | 2.4 | 0.006/0.252/0.93 | 0.246 | 0.381 | 0.064 | 3.42 | yan bolsa tabassum. |
| 6 | 18.73 | 3.67 | 0.002/0.394/0.815 | 0.264 | 0.321 | 0.076 | 7.0 | Daim yoxshar bilan surashganimda, ozun ten kurballa bilan ga |
| 7 | 22.40 | 1.1 | 0.0/0.271/0.682 | 0.213 | 0.14 | -0.011 | 2.14 | salib, ne |
| 8 | 23.50 | 4.0 | 0.002/0.254/0.768 | 0.238 | 0.384 | 0.065 | 8.26 | davolni bolish boladi. Bu videonu koryabsimi, demay kimdir b |
| 9 | 27.50 | 1.97 | 0.024/0.224/0.537 | 0.159 | 0.353 | 0.042 | 5.42 | kushmamilalik bilan kulib surashin. As |
| 10 | 29.47 | 0.9 | 0.002/0.399/0.825 | 0.269 | 0.365 | 0.062 | 4.87 |  |
| 11 | 30.37 | 1.63 | 0.002/0.443/0.819 | 0.262 | 0.332 | 0.065 | 12.07 | -salamu alaikum |
- harakat: 6 fps kadr farqi (0.3 dan past = statik/shtativ, 1+ = qo'l kamera/zoom/tez B-roll).

## 5. Audio
- Nutq paytida median -14.1 dBFS, pauzalarda -22.0 dBFS → farq 7.9 dB; fon musiqasi: BOR
- Spektr: bas (<150 Hz) ulushi -11.1 dB, nutq polosasi -1.5 dB (full'ga nisbatan)
- Yuqori chastotali zarbalar (SFX nomzodlari): 25 ta, shundan kesimda (±0.15 s): 3 → [1.2, 2.3, 2.4, 2.9, 5.9, 8.3, 8.8, 10.3, 10.7, 11.4, 12.5, 14.1, 15.4, 16.1, 18.7, 19.1, 19.6, 20.1, 21.9, 23.6]
- TODO (Claude): SFX turlari (whoosh/pop/glitch/riser) va qaysi vizual hodisaga bog'langani — tv_*.png to'lqinlarida ko'r.

## 6. Vizual material (KO'R)
- Kontakt: contact_00.jpg, contact_16.jpg
- video-use timeline_view (filmstrip + to'lqin + so'zlar): tv_huk.png, tv_yakun.png, tv_kesim_5.30.png, tv_kesim_7.70.png, tv_kesim_13.70.png, tv_kesim_16.33.png, tv_kesim_18.73.png, tv_kesim_23.50.png, tv_kesim_27.50.png, tv_kesim_30.37.png
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
