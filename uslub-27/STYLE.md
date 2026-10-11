# Uslub 27 — "Ko'cha intervyusi, hujjatli" (@uktamjontuygunovv, M oila)

Manba: instagram.com/reel/Dd8-UiOMI2x — "Ayrim quruvchilar haqida…", 49.7 s, 1080×1920, 29.97 fps, −14.2 LUFS, 71 like.
Mavzu: ko'chmas mulk / qurilish, qurilish maydonchasida ikki kishi gaplashadi (savol beruvchi + ekspert, kaska).
Keyframes: `keyframes/c00..c48.jpg` (2 fps varaq, har qator 4 s), `keyframes/<t>.jpg` (t dan 18 ketma-ket kadr).

## 1. Umumiy taassurot
Tez kesimli hujjatli intervyu: keng kadr (3 kishi) ↔ yaqin plan (ekspert) ↔ arxiv/olomon kadrlari ↔ film-B-roll.
Matn chapga tekislangan, ikki darajali: **sariq kalit so'z (katta)** + oq izoh qatorlari (kichik). Hamma narsa so'zma-so'z chiqadi.
Ohang: jiddiy, "fosh qiluvchi" — premium emas, lekin bachkana ham emas.

## 2. Kompozitsiya va zonalar
- Matn bloki: chap chetdan ~40–60 px, vertikal ko'krak/kamar balandligida (y ≈ 780–1250), yuzdan pastda. Yuzga tushmaydi.
- Keng kadrda matn odamlar orasidagi bo'sh joyga, markazga yaqin (`Nimaga / deb o'ylaysiz?` 2 odam orasida).
- Yaqin planda katta so'z ko'krak ustida, gavda bo'ylab (`Shunaqa`, `gipoteza*`, `ko'p endi omillar bor`).
- Kesimlar 1.0–3.5 s (22 ta kesim / 49.7 s ≈ har 2.2 s).

## 3. Tipografiya
- Geometrik grotesk, bir qavatli `a`, dumaloq `q` — nomzodlar (mock bilan tanla): **Outfit 600–700**, Urbanist 700, Euclid Circular A.
- Kalit so'z: 96–120 px, sariq; izoh qatorlari: 44–52 px oq, 600; qator oralig'i 1.05–1.1 (zich).
- Urg'u turlari: `gipoteza*` (oq katta + sariq yulduzcha), `umid bilan` (sariq italic so'z qatorda), `mard` (qizil katta),
  `[boshlaydi]` (kvadrat qavsda kichik), `"quruvchilar"` (qo'shtirnoqda — kinoya), qo'lda yozilgan qizil izoh (marker shrift).
- Soya: yengil qora soya (0 2px 12px rgba(0,0,0,.35)) — plashka yo'q.

## 4. Ranglar
Sariq `#FAE837` (kalit so'z), oq, qizil ~`#E3202A` (salbiy urg'u: "mard", qo'lda yozuv, zigzag), to'q shisha `rgba(20,20,24,.55)`.
Grading: neytral, yorqin kunduz; arxiv kadrlari oq-qora yoki xira.

## 5. Elementlar (o'lchangan vaqtlar 29.97 fps)
| Element | Kirish | Turish | Chiqish |
|---|---|---|---|
| Sariq kalit so'z | blur 10→0 + opacity, ~5 kadr (0.17 s), yengil chapdan suzish | kadr oxirigacha | keyingi kesimda yo'qoladi / blur |
| Oq izoh so'zlari | so'zma-so'z, har so'z blur→aniq ~4 kadr, so'z aytilganda | blok to'lguncha | blok bilan birga |
| "Shunaqa" katta so'z | gorizontal cho'zilgan motion-blur + scale 0.7→1, 5 kadr; keyin sekin kattalashish 1→1.08 | ~1.5 s | **burilib (≈25°) pastga-o'ngga uchadi va KESIMDAN O'TIB keyingi kadrda ham davom etadi** |
| "gipoteza*" | kichik so'zlar ("aslida hammasi") arvoh-crossfade; katta so'z ortda blur 12→0, ~6 kadr | 1.5 s | blur |
| "puli bor / mard / puli yo'q" | so'z vertikal cho'zilib (scaleY 1.5→1) + blur kiradi; "mard" qizil harfma-harf yoziladi | — | — |
| Qizil qo'lda yozuv | harfma-harf "chiziladi" ~1 s, oq qatorlar ostiga qiyshiq | 1 s | fade |
| Qizil zigzag | so'z ostida chiziladi (draw-on) 0.3 s | — | — |
| To'q shisha plashka subtitr | plashka markazdan ENIGA o'sadi (scaleX 0.3→1, blur) ~8 kadr, keyin matn so'zma-so'z | butun gap | fade |
| Doira-niqob B-roll | qora fon, yupqa halqali doira ichida klip; neon-sariq qo'lyozma so'z + oq izoh | 2.5 s | kesim |
| 3D chiqish ("ko'p endi omillar bor") | — | — | blok rotateX/Z bilan og'ib, pastga tushib, blur bilan keyingi kadrga "to'kiladi" |

## 6. O'tishlar
- **Negativ (invert) chaqnash** 3–4 kadr kesimda, ba'zan faqat yarmi (yuqori yarim negativ) — glitch urg'u.
- RGB-siljish (xromatik aberratsiya) olomon kadrlarida doimiy yengil.
- Matn kesimdan o'tib harakatlanadi — ko'prik (match-motion) vazifasi.
- Yakun: oq ekranga hard cut.

## 7. Kamera
Manba qo'l kamerasi + sekin push-in/drift (1.0→1.08, butun kadr davomida). Virtual zoom-in kesimlar orasida yo'q.

## 8. B-roll
Olomon/arxiv kadrlari (xira, past sifat — "hujjat" hissi), film parchalari (Social Network, Wolf of Wall Street) — **bizda ishlatilmaydi:
mualliflik huquqi + Content ID xavfi**; o'rniga Pexels, yuzsiz kadrlar (pul, hujjat, qurilish).

## 9. CTA va yakun
1. Gap subtitri ostida oq pill: dumaloq avatar + `@handle` (kichik, 26 px), ~1.5 s.
2. Pill "obuna bo'ling" ga aylanadi + o'ngda to'q-sariq ✓ doira (avatar chapdan suriladi, matn crossfade).
3. Hard cut → OQ ekran: YouTube thumbnail kichikdan kattalashadi (0.6→1, blur), ostida "Tez kunda!" + YouTube logo so'zma-so'z.
   (To'liq intervyu YouTube'da — anons yakuni.)

## 10. Audio
Pauzalarda fon (musiqa/atmosfera) nutqdan ~18 dB past (−30 dBFS vs −12.6). SFX siyrak, kesimlarga bog'lanmagan (5/22 kesimda).
Negativ chaqnash va 3D chiqishlarda qisqa whoosh/glitch.

## 11. Bizning silliqlik standartiga moslash (MAJBURIY)
Manbada kirishlar 0.17–0.3 s — juda tez. Bizda: kalit so'z 0.6 s `expo.out` + blur 12→0; plashka o'sishi 0.7 s `expo.out`;
"Shunaqa" uchib chiqishi 0.6 s `power2.inOut` (rotate 18°, y +220, blur 10) — kesimdan o'tishi saqlanadi;
negativ chaqnash o'rniga 0.3 s `sine.inOut` ekspozitsiya/negativ crossfade opacity ≤0.5 (yoki umuman ishlatma — premium uslubda).
Film B-roll → Pexels doira-niqob.

## 12. HyperFrames retsepti
- Kalit so'z bloki: `.kw` (sariq) + `.ln > span.w` (har so'z alohida tween, so'z vaqti −0.08 s).
- Shisha plashka: `backdrop-filter: blur(14px); background: rgba(20,20,24,.55); border-radius: 18px` → `scaleX 0.3→1, transformOrigin: left center`.
- Qo'lyozma: SVG `<text>` ustiga `clip-path` niqobi chapdan o'ngga (inset(0 100% 0 0) → inset(0 0 0 0)), 1.0 s `power2.inOut`.
- Doira-niqob: `clip-path: circle(0% at 50% 45%) → circle(38% …)` 0.8 s `expo.out` + halqa SVG chiziladi.
- 3D chiqish: o'rovchiga `perspective:900px`, `rotationX: 35, rotationZ: 12, y: 260, filter: blur(10px), opacity: 0`.

## 13. video-use + ref_analyze o'lchovlari (`_src/Dd8-UiOMI2x_an/report.md`, `tv_*.png`)
- **Tuzilma (beat'lar):** HUK 0–4 s (tezis-savol: "ayrim quruvchilar xalqni aldashi…", birinchi so'zdan, pauzasiz) → MUAMMO 4–9.4 (xalqda negativ, olomon arxivi)
  → SAVOL 9.4–17.4 (savol beruvchi: "nimaga deb o'ylaysiz? pul topish uchunmi?") → TEZIS 17.8–24 ("aslida hammasi gipoteza", film B-roll)
  → DALIL 24–37 ("fin model to'g'ri emas, tajriba yo'q", "$10 mln loyihani $2 mln bilan") → XULOSA 37.4–45.4 ("tajribasizlik") → YAKUN 45.7–49.7 (YouTube anons).
  Arxetip: Intervyu (SAVOL → JAVOB) + Hujjatli (TEZIS → DALIL → XULOSA).
- **Temp:** 143 so'z/daq, nutq 82% vaqt, ≥0.4 s pauza 1 ta — gaplar orasidagi pauzalar butunlay kesilgan.
- **Montaj:** 23 kesim, har 2.07 s, kadr median 1.83 s (min 0.27 s — negativ chaqnash kadri). **16/23 kesim gap o'rtasida** — ovoz uzluksiz,
  tasvir almashadi (B-roll ustiga ovoz, kamera almashuvi). Pauzadagi kesimlarda bo'shliq 0.02–0.35 s.
- **Grade:** neytral-iliq (R−B +0.03…+0.07), to'yinganlik o'rtacha 0.17–0.22 (biroz o'chiq), kontrast 0.20–0.30; huk kadri va "puli bor mard"
  kadri OQ-QORA; film B-roll qorong'i (p50 0.05–0.17) va to'yingan (0.45).
- **Kamera:** harakat 7–12 (qo'l kamera + push) deyarli hamma kadrda — "jonli hujjat" hissi; statik faqat film kadrlari (0.5–1).
- **Audio:** nutq −15.0 dBFS, pauzada −30.6 → farq 15.6 dB; bas ulushi −9.4 dB (yengil fon); SFX nomzodlari 36, kesimda faqat 4 —
  SFX asosan matn/grafika kirishiga bog'langan, kesimga emas.
