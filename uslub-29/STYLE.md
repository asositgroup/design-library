# Uslub 29 — "Syurreal 3D sahna, TOP-5" (@smoothbeey — Rasul Ubaydullayev, Visual Editor, N oila)

Manba: instagram.com/reel/Dd9EucloCBH — "Montajingiz uchun top 5 music", 29.2 s, 1080×1920, 30 fps, −14.2 LUFS, 675 like.
Tuzilma: spiker huki (0–3.5 s) → 3D sahnada TOP-5 (3.6–26.4 s, spiker yo'q, ovoz ortda) → spiker CTA (26.4–29.2 s).
Keyframes: `keyframes/c00, c16` (2 fps), `keyframes/<t>.jpg` (18 ketma-ket kadr).

## 1. Umumiy taassurot
"Muharrir portfoliosi" darajasidagi vizual: kechki iliq bokeh fonda spiker, tepada nafis serif CAPS sarlavha so'zma-so'z,
markazda 3D yaltiroq "5 MUSIC". Keyin AI-syurreal sahna (qizil tepalik, ikki stul, ko'k osmon) — har bandda 3D shisha-oltin raqam
tepalik ortidan o'sib chiqadi, tepada "albom kartasi" aylanib ochiladi.

## 2. Kompozitsiya
- Huk: sarlavha tepada (y≈60–120, xavfsiz zona ichida), katta 3D so'z ko'krakda (y≈820–900) — yuz ochiq.
- TOP-5 sahna: karta yuqori uchdan birida (y≈380–520, qiya 6–8°), raqam tepalik o'rtasida (y≈1150–1350), sahna to'liq ekran.
- CTA: serif so'z ko'krakda, markazda.

## 3. Tipografiya
- Sarlavha: yuqori kontrastli Didone condensed CAPS (Bodoni Moda / Playfair Display SC / "Italiana"), 64–72 px, oq + kichik oltin ornament;
  har so'z OLDINGISINING o'rnini egallaydi (bitta so'z ko'rinadi): MONTAJINGIZ → YANA HAM → CHIQISHI → UCHUN → 5 TA → MUZIKANI → ISHLATING.
- "5 MUSIC": qalin kondensat grotesk (Anton / Bebas Neue), oq yuz + oltin-to'q sariq 3D ekstruziya + tashqi iliq glow.
- Karta ichida: kichik qora grotesk, "barcode" uslubidagi qalin vertikal bloklar logotipi.

## 4. Ranglar
Huk: iliq qora-oltin bokeh. Sahna: ko'k osmon `#2F7FB8`, qizg'ish-to'q sariq tepalik `#B8451C`, oq karta, shisha raqam (ichida osmon aksi + oltin `#F6A02A` glow).
O'tish: sepiya/oltin duotone `#3A2208 → #F2D27A` (solarizatsiya).

## 5. Elementlar
| Element | Tafsilot (30 fps) |
|---|---|
| Serif sarlavha so'zi | kirish: tepadan vertikal cho'zilgan "slot" aralashuv (harflar ustma-ust siljiydi, blur), ~6 kadr; o'rnini keyingi so'z egallaydi ~0.5 s da |
| 3D "5 MUSIC" | kichikdan + blur bilan paydo bo'ladi, sekin "suzadi" (rotateY ±6°), chiqishda o'ngga burilib, **yorug'lik izi (light streak)** chizib ketadi |
| Albom kartasi | oq karta (radius 8, qalinlik/soya), qirradan (rotateY 90°→0, ingichka chiziq ko'rinishidan) ochiladi ~8 kadr; ichidan qora vinil disk o'ngga suriladi; trek nomi + ijrochi |
| 3D shisha raqam (1–5) | tepalik ORTIDAN kichik bo'lib ko'tariladi (scale 0.3→1, y +200→0) ~10 kadr; ichida osmon aksi, chetida oltin glow; chiqishda pastga, tepalik ortiga cho'kadi + karta yuqoriga uchib ketadi |
| To'lqinli qora chiziq (kabel) | butun sahna ustida sekin to'lqinlanadigan 2 ta ingichka egri chiziq — doimiy harakat qatlami |
| Serif CTA so'zi | "SAHIFAMGA", "BO'LIB…" — huk sarlavhasi bilan bir xil shrift, ko'krakda |

## 6. O'tishlar
- **Pikselli (blok-mozaika) eritish**: tasodifiy 40–60 px bloklar o'ngdan chapga yangi kadrga almashadi, ~10 kadr (3.4 s va 26.3 s).
- **Oltin solarizatsiya → rang**: yangi kadr avval oltin duotone/solarize ko'rinishida, ~0.8 s da tabiiy rangga crossfade (3.6–4.9 s, 26.5–27.6 s).
- Bandlar orasida kesim yo'q — elementlar chiqib-kirib almashadi (raqam cho'kadi → keyingisi ko'tariladi).

## 7. Kamera
Huk: spiker sekin zoom-in (1.0→1.06). Sahna: statik fon + sekin parallax (kabel chiziqlari, karta tebranishi).

## 8. B-roll / sahna
Sahna — AI-generatsiya qilingan fon (biz uchun: tayyor stok rasm yoki o'zimiz yaratgan fon; odam yo'q — qoidalar bilan to'qnashmaydi).
3D raqamlar: Blender/Spline'da yoki CSS 3D qatlamlar (pastda retsept).

## 9. CTA
Spiker qaytadi, serif so'zlar ko'krakda so'zma-so'z ("SAHIFAMGA OBUNA BO'LIB…"). Profil kartasi yo'q.

## 10. Audio
Bu video MUSIQANING o'zi haqida — TOP bandlarda trek parchalari baland (nutq yo'q). Hukda fon nutqdan ~16 dB past.
O'tishlarda pikselli eritishga "glitch/digital" SFX. Bizning ekspert reellarida faqat vizual uslub olinadi, audio standart o'zimizniki.

## 11. Silliqlik moslamasi
Sarlavha so'z almashuvi 0.5 s (eski so'z y −20 + blur 8 chiqadi, yangisi y +20 + blur 8 kiradi, `power2.inOut`, 0.15 s overlap) — "slot"
aralashuv o'rniga. 3D raqam ko'tarilishi 0.9 s `expo.out` (overshoot yo'q); karta flip 0.8 s `expo.out` rotationY 80→0 + blur;
light streak 0.6 s `power2.inOut`; pikselli eritish 0.6–0.8 s (bloklar stagger `sine.inOut`) — keskin glitch emas.

## 12. HyperFrames retsepti
- 3D shisha raqam: bitta raqam ~12 qatlam (`translateZ` -1…-12 px, to'q sariq gradient) + old yuz `background: linear-gradient(#fff9,#bfe3ff55)`,
  `-webkit-background-clip:text`, `filter: drop-shadow(0 0 24px #F6A02A)`; yoki oldindan PNG (Blender) — tezroq va chiroyliroq.
- Tepalik ortidan chiqish: raqam tepalik qatlami OSTIDA (tepalikni alohida PNG qilib, `rembg`/niqob bilan kes), y animatsiyasi.
- Pikselli eritish: 18×32 katakli grid div'lar, har katak opacity 1→0 tasodifiy `delay` (seeded random, seek-safe), 0.7 s ichida.
- Solarizatsiya: ffmpeg'da oldindan bake — `curves=all='0/0 0.5/1 1/0',colorchannelmixer=…` duotone, keyin HTML'da crossfade 0.8 s.

## 13. video-use + ref_analyze o'lchovlari (`_src/Dd9EucloCBH_an/report.md`, `tv_*.png`)
- **Tuzilma:** HUK 0–3.1 s (spiker: "montajingiz… 5 ta muzikani ishlating") → TOP-5 3.6–26.4 (spikersiz, ~4.5 s har band, faqat musiqa)
  → CTA 25.5–29.0 (spiker: "sahifamga obuna bo'lib qo'ying"). Nutq atigi 21% vaqt — vizual + musiqa asosiy.
- **Montaj:** faqat 2 haqiqiy kesim (3.57 va 26.47); 22.9 s lik grafik blok ichida almashuv elementlar animatsiyasi bilan (kesimsiz).
- **Sinxron:** pikselli o'tish (3.5 s) **musiqa zarbasining aynan kadriga** tushadi — o'tish = beat. Bandlar almashuvi ham trek parchalari chegarasida.
- **Grade:** juda to'yingan (0.56–0.73); huk va CTA iliq oltin (R−B +0.15…+0.19, p50 0.15 — qorong'i, bokeh), 3D sahna sovuq-ko'k (R−B −0.04).
- **Kamera:** harakat 7.7–12.6 — grafik blok doimiy harakatda (kabel to'lqinlari, karta tebranishi).
- **Audio:** musiqa nutqdan BALAND (pauza −14.7 vs nutq −19.2 dBFS) — bu video musiqa haqida; bas ulushi −2.1 dB (og'ir). Bizning ekspert reellarida
  bu audio olinmaydi (qoida 9); faqat "o'tish = musiqa zarbasi" usuli olinadi.
