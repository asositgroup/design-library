# Uslub pasporti — Islomxon Saidov | SAT Mentor (@islomxon.saidov), 8 referens

R1 DeHvx33sQ1u (qizil jadval, savol-javob, 0 kesim) · R2 DeCQIZpMnSj (1–5 reyting zinapoyasi, logolar, 0 kesim)
R3 Dd_uUBJMZDe (orange plashka huk, oq-pushti motion-grafika insertlari, CTA "Izohda 'English'")
R4 Dd1anF0spLl (split huk + B-roll, orange plashka, SAT masala qog'ozi) · R5 DdwTnoYsHij (masala yechish, izohlar UI CTA)
R6 Ddtr-fESZ5J (qizil "SAT" insertlari, maktab vs SAT) · R7 DdrHPiisnnz (split huk, qizil kalit so'z, Bluebook B-roll)
R8 DdhCayXMAnN (qizil stiker huk + 🎯, qizil kalit so'z + oq mayda so'zlar)

Spiker: referenslardagi odam = bizning videodagi odam, ofis ham bir xil (yog'och + to'q teal parda).

| Jihat | Referens (o'lchangan) | Bizda |
|---|---|---|
| Tuzilma | HUK (orange plashka / split B-roll, 0–5 s) → asosiy blok (jadval/reyting/kalit so'z) → insert(lar) → CTA "Izohda 'X' so'zini qoldiring" | huk 0–4.6 → jadval 4.6–20.3 (R1 formati aynan) → oq-pushti insert 20.3–24.1 → CTA 24.2–27 |
| Montaj ritmi | R1/R2: 0 kesim (bitta kadr + grafika). Boshqalari: kesim har 3–8 s, insertlar 1–4 s | jadval paytida KESIMSIZ (sekin push 1.0→1.06), hukda split, insert, CTA'da yaqinroq kadr |
| Huk | orange #F07B1E dumaloq plashka (r≈22), oq qalin 2 qator, divider ustida; split: tepa spiker, past B-roll, qizil 6 px chiziq | split: tepada spiker (1.35×), pastda Pexels SAT javob varag'i (yuzsiz), orange plashka "SAT Math'ga qaysi mavzular kerak?" |
| Jadval (R1) | x160–925, y1035–1423, 4 qator×~97 px, 3 ustun (nom / 3D emoji / javob), hujayra #B01018, oq-pushti 6 px oraliq, radius ~10, oq SF Pro semibold ~38 px; javob aytilganda ikonka + matn paydo | 8 qator×70 px, x150–930, y≈1010–1600; ustunlar: mavzu / ✅❌ 3D emoji / "Kerak"/"Kerakmas"; mavzular oldindan yozilgan (tomoshabin o'zi tanlaydi), aytilayotgan qator yoritiladi |
| Matn | SF Pro Display: CTA Light oq + Bold qizil #FF1A1A; kalit so'z qizil Bold katta + oq mayda so'zlar ustida | Inter (SF Pro analogi) 300/800, qizil #FF1F1F |
| Insert (R3/R6) | oq→pushti radial gradient fon, qora Poppins 800 + qizil pill/serif, kartochkalar ✓ qizil doira, kursor | "To'liq mavzular / ro'yxati" + 4 ta kerak mavzu ✓ kartalari + yopiq qatorlar |
| CTA | "Izohda / 'English' / so'zini qoldiring" — 3 qator markazda, ko'krakda, so'zma-so'z kirish | "Izohda / 'MAVZU' / so'zini qoldiring" |
| Rang | luma p50 0.11, p98 0.63–0.77, sat 0.51, iliq; pastki 25% qorong'i vinyetka | grade_match (strength 0.4) + pastki vinyetka |
| Audio | -14.2 LUFS, nutq−pauza 25 dB, fon musiqasi past; ~1 yuqori chastotali SFX/s (jadval hujayralari, insertlar) | jiddiy musiqa (v3), hujayra to'lganda yumshoq pop/click, insertda whoosh |
| OLINMAYDI | "ПОДПИСАТЬСЯ" (ruscha shablon), film/TV parchalari B-roll (R4 — mualliflik huquqi), pop'dagi overshoot | o'zbekcha / Pexels / smooth-motion.md |

## HyperFrames retsepti (reel-vau27 v4, 2026-10-07)
- Andoza: AbuDev/reel-vau27/scripts/compose.py + index.tpl.html (split huk + orange plashka, qizil jadval 8 qator, oq-pushti insert kartalar, CTA 3 qator).
- Shrift: Inter (SF Pro analogi) 300/600/800. Qizil: hujayra #b01018, matn #ff1f1f; orange plashka #f9902e→#f07415.
- 3D emoji: Microsoft Fluent Emoji 3D (MIT) — cdn.jsdelivr.net/gh/microsoft/fluentui-emoji@main/assets/<Nom>/3D/<nom>_3d.png.
  Qizil fonda qizil ❌ ko'rinmaydi -> oq 14 px radiusli fon.
- Grade (shu ofis, iPhone 10-bit): grade_match curves + eq=saturation=1.45 + colorbalance rm=.12 bm=-.12 + S-curve + gamma 1.12 + vignette; luma p50 ~0.10 (ref 0.11).
- Silliqlik: hamma kirish expo.out + blur, overshoot yo'q (referensdagi pop'lar moslashtirildi).

## So'zlar va elementlar joylashuvi (O'LCHANGAN, foydalanuvchi 2026-10-08 talab qildi — "so'zlar qayerda va qanday chiqishiga ahamiyat ber")
- Kalit so'z subtitri (R6 Ddtr, R7 DdrH, R8 DdhC, R4 Dd1a): QIZIL katta so'z (~100 px, Bold, #ff1414) CHAPGA tekis (x≈150),
  QO'LLAR/stol tepasida (y≈1320–1430). Jumla boshida so'zma-so'z pastdan + blur bilan chiqadi.
  Oq mayda so'zlar (~44 px Regular) uning USTIDA 2–3 qatorda, turli x da sochilib, AYTILGAN PAYTIDA qo'shiladi.
- Markazdagi jadval yoki markaziy subtitr EMAS. Yuqoridagi qoida asosiy.
- Reyting (R2 DeCQ): chap chetda vertikal zinapoya — raqamlar (pastdagilar qizil, eng tepadagisi oq), oq->qizil chiziq, logo pog'onaga tushadi.
- Andoza: AbuDev/reel-sat2/scripts/compose.py + index.tpl.html (v2).
