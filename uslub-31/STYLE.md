# Uslub 31 — "Iman: studiya monologi, TOP-3" (@iimaan_akhmedovna — IMAN | Shaxsiy rivojlanish, O oila)

Manbalar (bir xil studiya, bir xil grafika tizimi):
- instagram.com/reel/DeE5xZWIGSA — "Erkakni shu 3 ta narsasini hech qachon sevib qolmang!", 67.4 s, 30 fps, 2468 like (eng mashhuri)
- instagram.com/reel/Dd_wDslI42c — "Yil oxirigacha qarzdorlikdan butkul qutilish", 62.5 s, 30 fps, 524 like
- instagram.com/reel/Dd9lcCloHfh — "Agar siz 18–25 yosh atrofida bo'lsangiz…", 62.8 s, 30 fps, 572 like
Keyframes: `keyframes/<id>_cNN.jpg` (2 fps, har qator 4 s), `keyframes/<id>_<t>.jpg` (18 ketma-ket kadr, 30 fps).

## 1. Umumiy taassurot
Bitta spiker, hashamatli qorong'i studiya (oq panelli devor, qora parda, qizil-pushti divan, kafel pol, yog'och stul).
Mavzu: ayollar uchun maslahat / munosabatlar / moliya — har doim **TOP-3** ("shu 3 ta narsa", "uchta ish").
Grafika kam, lekin bir xil va taniqli: **to'q sariq→sariq gradientli kondensat CAPS** kalit ibora + **oq kichik subtitr**
+ **katta baland gradient raqam (1/2/3)**. Kinematografik B-roll har 1–2 gapda. Premium, ayollarga mo'ljallangan, iliq.

## 2. Tuzilma (3 videoda bir xil)
HUK 0–3 s (shart/va'da: "Agar siz 18–25 yosh…", "Agar shu yilning oxirigacha…", "Shu 3 ta narsasi aslo sevib qolmang") →
VA'DA 3–9 s ("mana shu uchta ishni darhol qiling" / "3 ta narsa") → **#1** (raqam + 3–4 gap + 1–2 B-roll) → **#2** → **#3** →
XULOSA (1–2 gap: "Inshaalloh…", "Alloh har birimizni individual yaratgan") → CTA ("VIDEONI SAQLAB QO'YING", "MENGA OBUNA BO'LING",
"USHBU VIDEOMIZNI QAYTA KO'RING"). Har band ~12–15 s.

## 3. Kamera va montaj
- 2 kamera bitta olishda: **KENG** (to'liq gavda, markazda, stul, kuchli vinyetka) va **O'RTA-YAQIN** (3/4 burchak, ortda qora parda
  + oq yorug'lik bokeh, yuz kadr tepasidan 1/4 da). Kesim har 2–3 s, KENG ↔ YAQIN navbatma-navbat, gap o'rtasida ham.
- Raqam (1/2/3) faqat KENG kadrda chiqadi — band boshlanishi = keng kadrga kesim.
- B-roll to'liq ekran 1.5–4 s, ovoz ustida; bitta gapga bitta kadr, ro'yxat aytilsa har so'zga yangi kadr.

## 4. Tipografiya
- **Kalit ibora:** baland kondensat grotesk CAPS (Bebas Neue / Anton / Oswald 700 nomzodlar — mock bilan tanla), 84–110 px,
  harf oralig'i ~0; 1–2 qator; markazda (keng kadrda tizza balandligi y≈1150; yaqin kadrda ko'krak y≈1050–1150),
  B-roll'da CHAP-TEPADA (x≈60, y≈330–420).
- **Gradient:** gorizontal chapdan o'ngga to'q sariq `#FA7B01` → sariq `#F9E23F` (har so'z o'zicha emas — butun qator bo'ylab).
  Yengil qora soya (0 4px 14px rgba(0,0,0,.45)).
- **Oddiy subtitr:** oq, sentence case, yumaloq grotesk (Inter / SF Pro 600 o'xshash), 44–52 px, 1–3 qator markazda;
  kalit ibora ostida bo'lsa ~36–40 px.
- **Raqam:** juda baland kondensat raqam (~300 px balandlik, eni ~70 px), vertikal gradient to'q sariq→sariq, chap chetda
  (x≈50, y≈250–520) — spiker yonida, yuzdan chapda.

## 5. Ranglar va grade
Iliq-kinematografik: qora studiya, terining iliq rangi, qizil-pushti aksent (divan). Kuchli oval vinyetka (burchaklar −40%).
B-roll'lar ham iliq, yumshoq kontrast, ko'pincha sayozroq fokus.

## 6. Elementlar (o'lchangan, 30 fps)
| Element | Kirish | Turish | Chiqish |
|---|---|---|---|
| Gradient CAPS so'zi | **so'zma-so'z**: so'z avval XIRA (opacity ~0.35, qo'ng'ir-zaytun) paydo bo'ladi, keyin ~10 kadr (0.33 s) ichida chapdan o'ngga yorishib to'liq gradientga keladi ("yorug'lik bilan to'lish") | ibora tugaguncha | keyingi ibora / kesimda yo'qoladi |
| Oq subtitr so'zi | so'zma-so'z, xira→oq ~6 kadr, so'z aytilganda; qator markazlashgan holda o'sadi | gap tugaguncha | fade |
| Raqam 1/2/3 | ingichka chiziq/kichik holatdan bo'yiga o'sadi (scaleY 0.2→1 + biroz yuqoriga) ~6 kadr | butun keng kadr (3–6 s) | kesimda |
| Oltin plashka (huk, faqat DeE5) | kinematografik B-roll ustida metall-oltin to'rtburchak (fask chegarasi, gradient `#7A5A12→#F2D46A`), ichida 2 qator qora kondensat CAPS ("SHU 3 TA NARSASI ASLO / SEVIB QOLMANG") | 3.5 s | kesim |
| B-roll ro'yxat ("arvoh" so'zlar) | har yangi B-roll kadri bilan bitta qator qo'shiladi (OFITSIANTGA / HAYDOVCHIGA / XODIMGA / OTA-ONASIGA / BEGONA ODAMLARGA) — yarim shaffof oltin "shisha/bo'rttirma" CAPS, chap-tepada ustma-ust | ro'yxat tugaguncha | fade |

## 7. O'tishlar
Hard cut'lar (kamera almashuvi, B-roll). Maxsus o'tish effekti yo'q. Silliqlik grafikada va so'z ritmida.

## 8. B-roll
Kinematografik stok: juftliklar (gul, sana), pul (dollar sanash), ishda/uyda ayollar, xafa odamlar, kafe/restoran, ko'cha.
Ba'zan boshqa sahifalarning videolari (watermark ko'rinadi — "ismoil print") va o'zbek seriali parchasi — **bizda yo'q**
(mualliflik huquqi). Mavzu diniy ohangda bo'lsa (Alloh, Inshaalloh, ehson) — bizning qoida 4: boshi ochiq ayollar yo'q;
munosabat mavzusida yuzsiz / orqadan / qo'llar kadrlari afzal.

## 9. CTA va yakun
Oxirgi 3–5 s KENG kadr + gradient CAPS chaqiruv ("VIDEONI SAQLAB QO'YING", "MENGA OBUNA BO'LING") + ostida oq izoh. Profil kartasi yo'q.

## 10. Audio
Nutq toza (lav/studiya), fon musiqasi sokin (pianino/pad) — 13-bo'lim raqamlari. SFX deyarli yo'q.

## 11. Silliqlik moslamasi (MAJBURIY)
- Gradient so'z: kirish 0.55 s — opacity 0→0.4 + blur 8→0 (`expo.out`), keyin "to'lish" — gradient niqobini chapdan o'ngga
  0.45 s `power2.inOut` (background-position yoki `clip-path` bilan oq/xira qatlam ustidan). Overshoot yo'q.
- Oq subtitr: smooth-motion "Subtitr" qiymatlari (0.45 s `expo.out`, y 14→0, blur 6→0).
- Raqam: scaleY 0.25→1 + y 30→0 + blur 10→0, 0.7 s `expo.out`, transformOrigin bottom.
- Chiqishlar: 0.5 s `power2.inOut`, blur 0→8 (manbadagi hard-cut yo'qolishi o'rniga).

## 12. HyperFrames retsepti
```css
.kw{font-family:'Bebas Neue';font-size:104px;line-height:.95;text-transform:uppercase;
    background:linear-gradient(90deg,#FA7B01 0%,#F9A51E 45%,#F9E23F 100%);-webkit-background-clip:text;background-clip:text;
    color:transparent;filter:drop-shadow(0 4px 14px rgba(0,0,0,.45))}
.kw .w{position:relative;display:inline-block}
.kw .w .dim{position:absolute;inset:0;color:rgba(120,95,30,.85);-webkit-text-fill-color:rgba(120,95,30,.85)}  /* xira qatlam */
.num{font-family:'Bebas Neue';font-size:330px;line-height:.8;background:linear-gradient(180deg,#F9C23F,#FA7B01);
     -webkit-background-clip:text;color:transparent;transform-origin:50% 100%}
.sub{font:600 46px/1.15 'Inter';color:#fff;text-shadow:0 2px 10px rgba(0,0,0,.5)}
```
Gradient "to'lish": har `.w` ichida xira nusxa ustida, gradientli nusxa `clip-path: inset(0 100% 0 0) → inset(0 0 0 0)`.
`text_not_painted` lint xatosi chiqsa (color: transparent) — `rgba(...,.01)` fill ber (lessons.md).
Andoza: `~/.claude/skills/reel-montaj/templates/iman_elements.html` (namuna kompozitsiya).

## 13. video-use + ref_analyze o'lchovlari (`_src/<id>_an/report.md`, `metrics.json`, `tv_*.png`)
| | DeE5xZWIGSA | Dd_wDslI42c | Dd9lcCloHfh |
|---|---|---|---|
| Davomiylik | 67.4 s | 62.5 s | 62.8 s |
| Temp | 128 so'z/daq | 167 | 147 |
| Nutq ulushi / ≥0.4 s pauza | 90% / 2 | 92% / 0 | 95% / 0 |
| Kesim | 35 ta, har 1.87 s | 31, har 1.95 s | 30, har 2.03 s |
| Gap o'rtasidagi kesim | 86% | 87% | 90% |
| O'rta yorug'lik / kontrast | 0.24 / 0.23 | 0.18 / 0.24 | 0.22 / 0.24 |
| To'yinganlik / iliqlik (R−B) | 0.28 / +0.08 | 0.26 / +0.08 | 0.26 / +0.09 |
| Kamera harakati | 2.6 (statik) | 2.3 | 2.3 |
| Nutq − pauza | 4.8 dB | 12.8 dB | 7.8 dB |
| SFX zarbalari (kesimda) | 53 (16) | 59 (11) | 61 (9) |
- **Xulosa:** juda tez montaj (har ~1.9 s kesim) — lekin kamera ichida harakat yo'q (shtativ), shuning uchun "tez, lekin xotirjam".
  Kesimlarning ~88% i gap o'rtasida (KENG ↔ YAQIN almashinuvi nutqni to'xtatmaydi). Pauzalar butunlay olingan.
- Qorong'i-iliq grade (o'rta yorug'lik 0.18–0.24, R−B +0.08), kuchli vinyetka.
- Musiqa referensda BALAND (pauzada nutqdan atigi 5–13 dB past) — **bizda olinmaydi** (qoida 9: nutq polosasida ≥19 dB).
- SFX: kesim/B-roll kirishlarining ~25–30% ida yengil whoosh; qolgani grafikaga.
- `reel-uslub` uchun referens metrikasi: `_src/Dd_wDslI42c_an/metrics.json` (o'rtacha vakil).
