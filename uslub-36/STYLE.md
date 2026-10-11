# uslub-36 — "Pastel kinetik promo" (S oila, referens: xullas.mp4)

Manba: `_src/xullas.mp4` (foydalanuvchi bergan fayl, 2026-10-10), tahlil `_src/xullas_an/` (report.md, metrics.json,
inv/sheetA-B.jpg — 2 fps vaqtli varaqlar, strips/A-D.jpg — har hodisa atrofida 18 kadr, fonts/cmp_*.png — shrift tekshiruvi).
Nutqsiz motion-grafika reklama: "Endi sizga montajor kerak emas → Claude yordamida → 35–40$ emas, 1$ → kutmaysiz → 5 daqiqada".

## 1. Umumiy taassurot / janr
Spikersiz, ovozsiz (faqat musiqa + SFX) kinetik tipografiya + shisha UI kartalar + 3D emoji ikonkalar. Apple-keynote/Dribbble
pastel estetikasi: yumshoq, toza, "premium-o'yinqaroq". Bitta uzluksiz kadr (kesim yo'q), sahnalar blur-fade bilan almashadi.

## 2. Tuzilma (20.0 s, 1920×1080, 24 fps)
| Vaqt | Beat | Matn |
|---|---|---|
| 0.00–4.55 | HUK | Endi sizga / montajor / ~~kerak~~ *emas!* |
| 4.75–10.1 | YECHIM | ✳ Claude yordamida siz · 3 karta (Motion animatsiya / Reels / YouTube videolar) · montajini *bemalol* qilishingiz mumkin! |
| 10.05–14.75 | NARX | Bitta video · ~~35–40$~~ *emas,* · (1$) evaziga · *sifatli* videoga ega bo'lasiz. |
| 14.8–16.7 | OG'RIQ | Endi montajor / bo'sh vaqtini *kutmaysiz,* · 3 bildirishnoma "Montajor …" |
| 16.5–20.0 | YAKUN | taymer 05:00→00:00→✅🎉 · ✳ Claude sizga / *5 daqiqada* / tayyor montajni beradi |
CTA yo'q (handle/havola yo'q).

## 3. Montaj ritmi
0 kesim (bitta "kadr"); sahna almashuvi = guruh blur 0→12 px + opacity 1→0 + scale 1→0.97, 0.35–0.45 s, keyingi sahna 0.1–0.2 s keyin.
Har sahna ichida elementlar ~0.25–0.5 s oraliqda ketma-ket qo'shiladi (musiqa 117 BPM ≈ 0.51 s/zarb ga taxminan).

## 4. Kompozitsiya (% — 1920×1080 dan)
- Sarlavha bloki markazda (x 50%); "Endi sizga" y 6.5%, "montajor" y 38–55%, ikkinchi qator y 63–73%.
- 2-sahna: tepa sarlavha y 6%, 3 karta x 20/50/80%, y 30–72% (har biri ~250×300 px), pastki qator y 86%.
- 3-sahna: tepada sarlavha → 12.0 s da 40% ga kichrayib y 5% ga ko'tariladi (keyingi bo'lim "kontekst" bo'lib qoladi), tanga markazda.
- 4-sahna: chapga tekislangan sarlavha x 8%, y 47–55%; bildirishnomalar o'ngda x 63–92%, y 45/52/59%.
- 5-sahna: oldingi sarlavha chap-tepaga (scale 0.4) "kontekst" bo'lib qoladi; taymer x 20% y 58%, matn x 38%.
- Burchaklarda ikonkalar (12/88% × 17/71%).

## 5. Tipografiya (kadr kesimi yonida render qilib tekshirildi — fonts/cmp_*.png)
- Sarlavha: **Inter Tight 800** (eng yaqin; asl — SF Pro Display Bold ehtimoli), tracking −2%, rang #1d1512. "montajor" ~190 px, "35–40$" ~160 px, "Endi montajor" ~90 px.
- Kichik qator: Inter Tight 600, 40–48 px ("Endi sizga", "Claude yordamida siz", "evaziga").
- Urg'u: **Instrument Serif Italic** (tekshirildi — eng mos), rang #b35841, 110–150 px ("emas!", "5 daqiqada"), qator ichida 40 px ("bemalol", "sifatli", "kutmaysiz").
- Bekor qilingan so'z: rang #9a918b ga o'tadi + terrakota chiziq #cc6d5a, qalinligi ~10 px (so'z balandligining ~10%), chapdan o'ngga 0.15 s.

## 6. Ranglar / grade
Fon: krem #f0e9e1 + 4 ta katta xira blob — coral #e5a591 (chap-tepa), lavanda #ccc0ea (o'ng-tepa), havorang #c1dcec (chap-past),
shaftoli #efcdae (o'ng-past); bloblar sekin suzadi va shaklini o'zgartiradi. Grade: luma p50 0.82, kontrast 0.125, to'yinganlik 0.175, iliq 0.10.
Arvoh so'zlar: "MONTAJ" (chap-tepa, y 5–25%) va "MOTION" (pastda, y 62–85%), ~260–280 px qalin, ~8–10% to'q, xira.

## 7. Matn kirishi (strips/A–D)
- Harfma-harf: har harf pastdan ~40% balandlikdan ko'tariladi + blur 8→0 + opacity, stagger 0.03–0.06 s, harf 0.25–0.3 s, ease power3.out.
- Bekor qilish: so'z kulranglashadi (0.1 s) → chiziq chiziladi (0.15 s) → kursiv so'z 0.1 s keyin harfma-harf.
- Pastki qator: so'zma-so'z ko'tarilish + blur, 0.08 s stagger.
- Raqam "1$": tanga ichida 4$→2$→1$ almashadi (0.4 s), keyin "evaziga".
- Taymer: 05:00 dan tezlashib 00:00 gacha (1.3 s), keyin raqamlar blur bilan yo'qolib ✅ chiqadi.

## 8. Grafik elementlar
| Vaqt | Element | Kirish | Turish | Chiqish |
|---|---|---|---|---|
| 0.45–4.5 | 4 ta ikonka-plitka (oq shisha, radius ~22, 3D emoji: noutbuk/klaket/palitra/TV) | scale 0.6→1 + blur, 0.3 s | ichidagi emoji har ~1 s almashadi | guruh bilan blur |
| 5.25–9.7 | 3 shisha karta (oq→shaftoli gradient, radius 24, yumshoq soya) | 3D: rotateY −25°→0 + chapdan + blur, 0.5 s, stagger 0.4 s | 1-kartada qizil doira + qora kvadrat animatsiyasi (aylanish), uchqunlar | blur |
| 10.3–12.0 | pul xaltasi, uchar pullar (3D emoji), 2 kulrang metall shar | pop + blur | sekin suzish | pastga/yonga chiqib ketadi |
| 12.35–14.7 | "1$" tanga (shaftoli doira, ikki halqa, ~170 px) | scale + blur | — | blur |
| 15.0–16.9 | 3 bildirishnoma qatori (shisha pill: ⏳ / 😴 / 📱 + "Montajor" + "…") | o'ngdan + blur, stagger 0.25 | — | o'ngga + fade |
| 16.5–20 | taymer (shisha doira ~230 px), qizil progress halqa #d9705a | blur-pop | sanoq | ✅ + 🎉 |
| 4.75, 17.0 | Claude ✳ (to'q sariq yulduzcha) matn oldida | matn bilan | — | — |

## 9. O'tishlar
Faqat blur-fade (yuqorida). Kamera: butun kadr sekin 1.0→1.03 kattalashadi (sahna ichida), kesimda sakrash yo'q.

## 10. Kamera / B-roll
Kamera yo'q (grafika). B-roll yo'q.

## 11. Audio
- 0–4.3 s: sokin intro (−23 dB RMS), 4.4–4.6 s: drop (yuqori energiyali pop/elektro trek, 117 BPM, −8 dB), oxirigacha.
- SFX: 29 yuqori chastotali zarba (whoosh/pop/klik) — har element kirishiga bog'langan (5.9…15.3 s), kesim yo'q.
- Umumiy −9.3 LUFS (baland), peak −0.7.

## 12. Silliqlik moslamasi (smooth-motion.md)
Referens deyarli tepkisiz; ikonka/tanga pop'larida yengil overshoot bor → bizda `expo.out` + blur, overshoot yo'q. Chiqishlar ≥0.4–0.5 s.

## 13. HyperFrames retsepti (raqamlar)
- Fon: `#f0e9e1` + 4 radial blob (har biri ~60–75% ekran, `filter: blur(80px)`), bloblar `x/y ±6%`, `scale 0.9↔1.1`, 6–9 s sine.
- Harf kirishi: `fromTo(chars, {yPercent:45, opacity:0, filter:'blur(8px)'}, {yPercent:0, opacity:1, filter:'blur(0)', duration:0.3, ease:'power3.out', stagger:0.04})`.
- Strike: `.strike{height:0.1em; background:#cc6d5a; transform-origin:0 50%}` `scaleX 0→1, 0.15 s, power2.out`.
- Sahna chiqishi: `to(group,{opacity:0, filter:'blur(12px)', scale:0.97, duration:0.4, ease:'power2.in'})`.
- Shisha karta: `background: linear-gradient(160deg,#fff 0%,#fbe3d6 100%); border-radius:24px; box-shadow:0 30px 60px rgba(150,90,70,.18)`.

## 14. OLINMAYDI / moslash
- Ikonka/tanga pop'idagi yengil overshoot → expo.out (qoida 7).
- Apple emoji (mualliflik huquqi) → Microsoft Fluent 3D Emoji (MIT litsenziya) — ko'rinishi juda yaqin.
- Referens musiqasi (manbasi noma'lum) → Content ID'siz trek (foydalanuvchi o'zi bersa — o'shani).

## 15. Qachon ishlatish
Nutqsiz qisqa xizmat/mahsulot reklamasi, "X kerak emas → Y bilan → narx → vaqt" tuzilmasi, ilova/AI vosita promo, 16:9 yoki 9:16.

## Loyiha-namuna
`AbuDev/reel-montajor-kerakmas/` (2026-10-10, "kreativroq + wow" versiya, 16:9 24 s 60 fps): timeline'da so'z-kliplar + Claude kursori
"kerak"ni qaychi bilan kesadi → ✳ bloom drop → 3D tarqatilgan jonli kartalar → ipda osilgan narx yorlig'i qirqiladi → 3D tanga 1$ →
montajor chati supurib tashlanadi → taymer 05:00→✅ → kamera orqaga: butun video montaj dasturi monitorida (editor reveal).
Arvoh so'zlar PNG qilib render qilingan (check contrast/overlap xatosiz). SFX: tools/sfx_cues.json → tools/mix_sfx.py.
