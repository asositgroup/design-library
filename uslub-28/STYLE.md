# Uslub 28 — "Podkast-intervyu, UI kartalar" (@uktamjontuygunovv, M oila)

Manba: instagram.com/reel/Dd_39GWs0Wy — "Oylik to'lov kechiksa jarima beriladimi?", 55.8 s, 1080×1920, 29.97 fps, −14.2 LUFS, 120 like.
Mavzu: ko'chmas mulk savol-javob; ofisda 3 kishi kreslolarda (2–3 kamera: yaqin plan, yon profil, keng).
Keyframes: `keyframes/c00..c48.jpg` (2 fps), `keyframes/<t>.jpg` (18 ketma-ket kadr).
Uslub-27 bilan bir oila (shrift, CTA, yakun bir xil) — bu yerda UI-kartalar va marker urg'ular asosiy.

## 1. Umumiy taassurot
Toza "biznes-podkast": tabiiy rang, yumshoq fon blur (kamera f/1.8), matn chapda ikki darajali (oq katta + oq kichik).
Har 3–5 s da bitta "UI hodisa": oq karta + 3D emoji, to'q-sariq pill, ogohlantirish kartasi, marker bo'yoq, qo'lda chizilgan aylana.

## 2. Kompozitsiya
- Matn: chap chet 40 px, y ≈ 1000–1300 (ko'krak). Yon profil kadrida karta/pill so'zlovchining iyagi ostida, bo'yin balandligida.
- Kesim: savol beruvchiga — savol matni bilan (`" Qurilish kechiksachi? "` sariq qo'shtirnoq), javobda ekspert yaqin plan.
- Shahar aerial va qo'l/hujjat kadrlari (yuzsiz) — B-roll.

## 3. Tipografiya
Kengroq grotesk (ikki qavatli `a`, to'g'ri `y`), nomzodlar: **Satoshi 700**, Gilroy-o'xshash, Manrope 700, General Sans.
Katta qator 64–72 px 700; kichik 36–42 px 500; karta sarlavhasi 64 px 800 qora; karta izohi 28 px 500 kulrang.

## 4. Ranglar
Oq, qora matn (kartada), yashil marker `#0A9A1A` (~`#008C0A`), sariq-yashil marker `#C8D400`, to'q-sariq `#FB6C2A`,
qizil qo'lyozma aylana `#E3202A`, sariq qo'shtirnoq `#FAE837`.

## 5. Elementlar (29.97 fps o'lchovlari)
| Element | Tafsilot |
|---|---|
| **Oq karta + 3D emoji** ("Oylik to'lov / kechiksa jarimalar qo'llangan" + uchar pul 💸) | oq, radius 22, yumshoq soya; ekspert qo'li yonidagi nuqtadan scale 0.2→1 + chapga-pastga siljib, blur bilan ~10 kadr. Chiqish: **o'ngga surilib ketadi**, shu payt keyingi subtitr chapdan kirib keladi (konveyer/push) |
| Sariq qo'shtirnoq savol | `" "` sariq, matn oq; harflar chapdan surilib, 6 kadr |
| So'zma-so'z subtitr | har so'z blur→aniq; ikki darajali: 1-qator katta, 2–3 qator kichik |
| **"Sochilib → joylashish"** | so'zlar har xil balandlikda zinapoya bo'lib tushadi (pulni / yanvarni / ham / fevralni), gap tugagach bir tekis qatorlarga yig'iladi |
| Qo'lda chizilgan qizil aylana | so'z ("Fevral") atrofida ellips chiziladi ~12 kadr, oxiri ochiq qoladi |
| Marker bo'yoq | so'z orqasida to'rtburchak chapdan o'ngga to'ladi ~8 kadr (yashil, keyin sariq-yashil boshqa so'zda) — "yashil ro'yxat / sariq ro'yxat" ma'nosiga mos rang |
| **To'q-sariq pill** (izoh/iqtibos) | tor chiziqdan eniga o'sadi (scaleX 0.25→1, ~8 kadr), shtrix ichki chegara (dashed oq), matn yoziladi; ostidan oq pill ikkinchi qator ("moliya bo'limimiz habar oladi") |
| **Ogohlantirish kartasi** | oq karta, chapda to'q-sariq ustun + oq `!`; kichik nuqtadan o'sadi (~8 kadr), matn **typewriter** harfma-harf, karta balandligi qator qo'shilgan sari o'sadi |
| `[aka 3-oy bo'ldi to'lay olmayapsiz]` | kvadrat qavsli kichik qator — boshqa odam gapi (iqtibos) |
| Kursiv urg'u | `"bekor"` italic qo'shtirnoqda |

## 6. O'tishlar
Hard cut'lar (17 ta / 55.8 s ≈ 3.3 s), matn kesimda saqlanib qolishi mumkin. Elementlar ichida o'tish = push (biri o'ngga, boshqasi chapdan).

## 7. Kamera
Ko'p kamerali podkast (yaqin / keng / yon profil), sekin raqamli push. Aerial kadrda sekin panorama.

## 8. B-roll
Shahar aerial, qo'llar + hujjat varaqlash, call-center xodimi (yon profil, yuz qisman). Hammasi B-roll stokdan — Pexels bilan mos.

## 9. CTA va yakun
Uslub-27 bilan bir xil: avatar+@handle pill → **to'q-sariq gradient chapdan to'lib** "obuna bo'ling" + ✓ → oq yakun ekrani (YouTube anons).

## 10. Audio
Fon nutqdan ~16 dB past (pauza −28.4 dBFS, nutq −12.4). SFX kartalar kirishida (pop/whoosh) — 7/17 kesimda.

## 11. Silliqlik moslamasi
Kartalar: 0.8 s `expo.out` scale 0.85→1 + blur 12→0 (0.2 dan EMAS — overshoot hissi bermasin); push-chiqish 0.6 s `power2.inOut` + motion blur 8;
pill o'sishi 0.7 s `expo.out`; typewriter — harf opacity 0.05 s stagger (matn emas, harflar span), karta balandligi `scaleY` emas — oldindan
to'liq balandlikda qurib `clip-path inset` bilan och (layout xossasini tween qilma); marker `scaleX 0→1, transformOrigin left` 0.5 s `power2.inOut`;
"sochilib → joylashish" ikki bosqich: kirish y-ofsetlar bilan, joylashish 0.6 s `expo.inOut`.

## 12. HyperFrames retsepti
- Karta: `.card{background:#fff;border-radius:22px;box-shadow:0 18px 40px rgba(0,0,0,.25)}` + emoji PNG (Apple/Fluent 3D emoji — litsenziyaga qara; Microsoft Fluent Emoji 3D MIT).
- Ogohlantirish: `.alert::before` ustun 26 px `#F0562A` + `!`; matn `span.ch` harfma-harf.
- Qizil aylana: SVG path `pathLength=1`, dasharray 1, offset 1→0.06 (oxiri ochiq) 0.6 s `power2.inOut`.
- Marker: so'z ortida `.hl{position:absolute;inset:-4px -8px;background:#0A9A1A;transform-origin:left}`.

## 13. video-use + ref_analyze o'lchovlari (`_src/Dd_39GWs0Wy_an/report.md`, `tv_*.png`)
- **Tuzilma:** HUK 0–5.7 s (muammo + karta "Oylik to'lov / kechiksa jarimalar") → SAVOL 5.7–7.0 ("Qurilish kechiksachi?") → JAVOB 7–14 ("bizda sanksiya yo'q",
  yanvar→fevral misoli) → MEXANIZM 14–33 (yashil / sariq / qizil ro'yxat, moliya bo'limi xabar oladi) → ISTISNO 33–48 (4-oyga o'tsa — yurist, shartnoma "bekor")
  → XULOSA 48–50 ("yechim qidiriladi") → CTA 50–51.7 → YAKUN 51.75–55.8 (YouTube anons). Arxetip: Intervyu, savol-javob + qoida tushuntirish.
- **Temp:** 128 so'z/daq, nutq 81%, ≥0.4 s pauza 2 ta.
- **Montaj:** 17 kesim, har 3.1 s, kadr median 2.94 s (1.33–6.0). **11/17 kesim gap o'rtasida** — ko'p kamerali podkast: ovoz uzluksiz, burchak almashadi.
  Pauzadagi kesimlar bo'shliq 0.04–0.34 s (video-use "spiker almashinuvi 400–600 ms" qoidasidan ancha qisqa — tez reel ritmi).
- **Grade:** tabiiy, biroz iliq (R−B +0.04), to'yinganlik 0.27–0.31, kontrast 0.24; aerial shahar va hujjat B-roll'i o'chiqroq (0.09–0.18).
- **Kamera:** intervyu kadrlari deyarli statik (0.4–2.2, shtativ), B-roll va karta kadrlari 4.5–9.8.
- **Audio:** nutq −14.8, pauza −26.5 → farq **11.7 dB** (musiqa 27-uslubdan ~4 dB balandroq); bas −7.7 dB. **Karta kirishida (1.49 s) aniq SFX zarbasi** —
  UI-hodisa = SFX ("hit on the frame"); kesimlarda SFX 4/17.
