# "Imona Ahmedova uslubi" — O oila pasporti (4 ta referens BIRGALIKDA)

Foydalanuvchi "Imona Ahmedova uslubida montaj qil" desa — **shu pasport asosiy manba**. Uslub bitta videodan emas, quyidagi
4 ta videoning hammasidan olinadi; qaysi element qaysi videodan va qachon ishlatilishi pastda. Tafsilotlar: `uslub-31/STYLE.md`, `uslub-32/STYLE.md`.

| # | Video | Format | Asosiy hissasi |
|---|---|---|---|
| R1 | DeKDOv2IB3- "Nega erkak boshida ko'p e'tibor beradi…" (53.5 s, 60 fps) | 2 kishi podkast, split-ekran | split kompozitsiya, chegaradagi sariq subtitr, CAPS savol-huk, qizil ro'yxat yorliqlari |
| R2 | DeE5xZWIGSA "Erkakni shu 3 ta narsasini…" (67.4 s) — eng mashhur (2468 like) | monolog TOP-3 | oltin plashka huk, gradient CAPS, raqam 1/2/3, B-roll'da chap-tepa matn, "arvoh" ro'yxat qatorlari |
| R3 | Dd_wDslI42c "Yil oxirigacha qarzdorlikdan…" (62.5 s) | monolog TOP-3 | shart-huk ("Agar…") gradient CAPS, B-roll ritmi (pul, hujjat), CTA "VIDEONI SAQLAB QO'YING" |
| R4 | Dd9lcCloHfh "Agar siz 18–25 yosh…" (62.8 s) | monolog TOP-3 | yosh/auditoriya huki, juftlik/ayol B-roll, CTA "MENGA OBUNA BO'LING" |
Fayllar: `design-library/_src/<id>.mp4`, tahlil `_src/<id>_an/` (report.md, metrics.json, tv_*.png).

## 1. Qaysi qolip — foydalanuvchi videosiga qarab
| Foydalanuvchi videosi | Qolip | Elementlar |
|---|---|---|
| Bitta spiker, maslahat/ro'yxat | **Monolog** (R2–R4 asosida) | gradient CAPS + oq subtitr, raqam 1/2/3, B-roll, vinyetka |
| 2 kishi, savol-javob / suhbat | **Split-podkast** (R1) | tepada gapiruvchi, pastda keng kadr, chegarada sariq subtitr, qizil yorliqlar |
| Aralash (monolog + boshlovchi savollari) | Monolog asosiy, savol bo'laklari split (R1) | o'tish hard cut |
Ikkala qolipda UMUMIY (to'rttalasida bor): tez ritm, pauzasiz nutq, gap o'rtasida kesim, kinematografik B-roll, iliq grade,
so'zma-so'z "xira → yorqin" matn kirishi, sariq/to'q sariq aksent, CAPS urg'u, CTA og'zaki + CAPS yozuv.

## 2. Tuzilma (R2–R4 da bir xil, R1 savol-javob varianti)
HUK 0–3 s (shart / savol / taqiq: "Agar…", "Nega ayrim…", "…aslo sevib qolmang") → VA'DA ("mana shu 3 ta…") → #1 → #2 → #3
(har band 12–15 s, band boshida keng kadr + raqam) → XULOSA (1–2 gap) → CTA (saqlang / obuna bo'ling / qayta ko'ring).
Foydalanuvchi matni 3 bandga bo'linmasa — bandlarni gap mazmunidan ajrat, raqamsiz variantda faqat gradient CAPS urg'ular.

## 3. Raqamli maqsadlar (4 referens: median / oraliq)
| Ko'rsatkich | Median | Oraliq | Izoh |
|---|---|---|---|
| Kesim har N s | 1.99 | 1.87–3.82 | monolog ~1.9, podkast ~3.8 |
| So'z/daqiqa | 138 | 92–167 | pauzalar olinadi (≥0.4 s pauza 0–2 ta) |
| Gap o'rtasida kesim | 0.87 | 0.46–0.90 | kamera almashuvi nutqni to'xtatmaydi |
| O'rta yorug'lik | 0.23 | 0.18–0.51 | monolog qorong'i, podkast yorqin |
| Kontrast / to'yinganlik | 0.24 / 0.27 | 0.23–0.32 / 0.26–0.30 | |
| Iliqlik (R−B) | +0.086 | +0.077…+0.145 | doim iliq |
| Kamera harakati | 2.3 | 1.9–2.6 | shtativ — ichki harakat yo'q |
| Nutq − pauza | 6.3 dB | −0.5…12.8 | **olinmaydi**: bizda qoida 9 (≥19 dB nutq polosasida) |

## 4. Rang
```bash
S=~/Desktop/AI-Videos/AbuDev/design-library/_src
python ~/.claude/skills/reel-uslub/scripts/grade_match.py $S/DeKDOv2IB3-.mp4,$S/DeE5xZWIGSA.mp4,$S/Dd_wDslI42c.mp4,$S/Dd9lcCloHfh.mp4 <manba.mp4> analysis
```
Monolog qolipida grade'ga oval vinyetka qo'sh (`vignette=angle=PI/4.2`) — R2–R4 da kuchli; podkast (R1) da vinyetka yo'q.

## 5. Uslub tekshiruvi (render'dan keyin)
```bash
python ~/.claude/skills/reel-uslub/scripts/style_compare.py $S/DeKDOv2IB3-_an/metrics.json $S/DeE5xZWIGSA_an/metrics.json \
  $S/Dd_wDslI42c_an/metrics.json $S/Dd9lcCloHfh_an/metrics.json analysis/out_an/metrics.json --md analysis/style_compare.md
```
Monolog bo'lsa faqat R2–R4 metrikalarini, sof podkast bo'lsa R1 ni berish ham mumkin (aniqroq oraliq).

## 6. Elementlar (aniq qiymatlar — STYLE.md 11/12-bo'limlar; ishlaydigan kod — reel-montaj `templates/iman_elements.html`)
- Gradient CAPS so'z (R2–R4): Anton/Bebas kondensat 104 px, `#FA7B01 → #F9A51E → #F9E23F`, xira kirish 0.55 s + chapdan "to'lish" 0.45 s.
- Oq subtitr (R2–R4): 46 px, so'zma-so'z 0.45 s `expo.out`.
- Raqam 1/2/3 (R2–R4): 330 px baland, scaleX .72, chapda, pastdan o'sadi 0.7 s.
- Oltin plashka huk (R2): B-roll ustida 2 qator qora CAPS, metall-oltin gradient.
- B-roll matni (R2–R4): chap-tepa gradient CAPS + oq izoh; ro'yxat — "arvoh" oltin qatorlar.
- Split (R1): tepa 0–1060 (1.35×, yuz tepadan ~380 px), past 1060–1920 keng; chegarada sariq subtitr 50 px; qizil yorliqlar `#AB0103` + oltin chegara.
- CTA (R2–R4): keng kadr + gradient CAPS chaqiruv.

## 7. OLINMAYDI (sababi bilan — rejada ochiq yoz)
- Baland musiqa (nutq−pauza 5–13 dB) → qoida 9.
- Boshqa sahifalarning videolari (watermark) va serial parchalari → mualliflik huquqi, Pexels.
- B-roll odamlari: mavzu diniy ohangda (Alloh, ehson) bo'lsa boshi ochiq ayollar yo'q; munosabat mavzusida yuzsiz/orqadan kadrlar.
- Tez pop/hard-cut grafika chiqishlari → smooth-motion.md (0.5 s chiqish).
