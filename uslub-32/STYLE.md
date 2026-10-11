# Uslub 32 — "Iman: ikki qavatli podkast (split-ekran)" (@iimaan_akhmedovna, O oila)

Manba: instagram.com/reel/DeKDOv2IB3- — "Nega erkak boshida ko'p e'tibor beradi, keyin soviydi?", 53.5 s, **60 fps**, 359 like.
Keyframes: `keyframes/DeKDOv2IB3-_cNN.jpg` (2 fps), `keyframes/DeKDOv2IB3-_<t>.jpg` (18 kadr, 30 fps ga tushirilgan).
Uslub-31 bilan bir oila (bir xil studiya, rang, ritm), lekin bu podkast formati: mehmon/boshlovchi (oq kiyimda) savol beradi,
Iman (qora kiyimda) javob beradi.

## 1. Kompozitsiya — asosiy g'oya
Ekran gorizontal **ikki qavat**:
- **Tepada (0–1060 px):** gapirayotgan odamning YAQIN plani (16:9 kameradan kesilgan, yuz tepadan ~1/4 da, mikrofon kadrda).
- **Pastda (1060–1920 px):** studiyaning KENG ikki kishilik kadri — deyarli o'zgarmas (statik), "kontekst" panel.
- Chegara: chiziqsiz, to'g'ridan-to'g'ri (oq parda / qizil gilam kontrasti chegara vazifasini bajaradi).
- Tepa panel gapiruvchiga qarab almashadi (savol → boshlovchi yaqin plani, javob → Iman yaqin plani); pastki panel o'sha-o'sha.
- B-roll to'liq ekranni egallaydi (ikkala panel o'rniga), keyin split qaytadi.

## 2. Tipografiya va matn
- **Subtitr ikki panel CHEGARASIDA** (y≈1000–1080, tepa panel pastida) — markazda, sariq (`#E0AD22 → #F7EF49` xira→yorqin),
  qalin grotesk sentence case 46–52 px, 1–2 qator; savol huki CAPS ("NEGA AYRIM ERKAKLAR"), kalit so'zlar CAPS ("ERKAK KISHI").
- So'zma-so'z: so'z xira-sariq paydo bo'lib ~0.2 s da yorqin sariqqa o'tadi (uslub-31 "to'lish" ning sodda varianti, gradientsiz).
- Chegaraning chap chetida kichik qizil kanal belgisi (logo) — doimiy.

## 3. Ro'yxat yorliqlari (qizil plashkalar)
"YAXSHI KO'RGANI YONIDA / HOTIRJAMLIGI YONIDA / HIMOYACHISI YONIDA" — to'q qizil `#AB0103` to'rtburchak, ingichka oltin chegara,
ichida sariq kondensat CAPS 30–34 px. Tepa panelning pastki qismida (y≈850–1000) zinapoya: 1-chi chapda, 2-chi o'ngroq/pastroq, 3-chi chapda pastda.
Kirish: kichikdan (scale ~0.4) kattalashadi ~5 kadr; uchalasi gap tugaguncha qoladi. Kichik qizil pill — so'z yonida izoh ("hotirjam bo'ladi").

## 4. Montaj ritmi
Kesim = gapiruvchi almashuvi + B-roll. Tepa panelda bitta odam 2–8 s turadi. 60 fps (silliq ko'rinish).

## 5. B-roll
Kinematografik sahnalashtirilgan kadrlar (yigit-qiz, gul, bog') — to'liq ekran, sariq subtitr markazda saqlanadi.
Bizda: Pexels, qoida 4 (yuzsiz/orqadan, diniy ohangda boshi ochiq ayollar yo'q).

## 6. Ranglar
Yorqin, iliq-krem studiya (oq parda), qora va oq kiyim kontrasti, qizil gilam. Uslub-31 dan yorqinroq (kunduzgi yorug'lik).

## 7. Silliqlik moslamasi
Qizil yorliq: scale 0.85→1 + blur 8→0, 0.6 s `expo.out` (manbadagi 0.4→1 tez pop o'rniga); subtitr so'zi 0.45 s `expo.out`
+ rang xira→yorqin 0.35 s; B-roll ↔ split o'tishi hard cut (manbadagidek) — kamera sakramaydi, chunki panel ichida zoom yo'q.

## 8. HyperFrames retsepti
- Ikki `<video>` (yoki bitta manbadan ikki kesim): `#top{position:absolute;top:0;height:1060px;overflow:hidden}` ichida video
  `object-fit:cover` + yuz bo'yicha `object-position`; `#bot{top:1060px;height:860px}` keng kadr.
- Bitta kameradan bo'lsa: pastki panel = keng kadr (1.0), tepa = o'sha kadrning zoom'i **~1.35×** (demo'da 2× faqat ko'zlarni ko'rsatdi),
  yuz markazi panel tepasidan ~380 px da (bosh qutisidan hisobla: `top = 380 − yuz_y×zoom`); matn/yorliqlar ko'krak-qo'llar ustida (y 800–1040).
  Ishlaydigan namuna: reel-montaj `templates/iman_elements.html` (5–10 s qismi).
- Subtitr `#seam{top:990px}` — ikkala panel ustida, yuzga tegmaydi.
- Yorliqlar: `.tag{background:#AB0103;border:2px solid #D8B04A;color:#F7E14A;font:400 32px 'Bebas Neue';padding:6px 14px}`.

## 9. video-use + ref_analyze o'lchovlari (`_src/DeKDOv2IB3-_an/`)
- 53.5 s, 60 fps; temp 92 so'z/daq (suhbat, savol-javob), nutq 72%, ≥0.4 s pauza 1 ta.
- 13 kesim, har 3.8 s, kadr median 2.7 s; gap o'rtasida 46% (savol ↔ javob almashuvi pauzada ham bo'ladi).
- Yorqin-iliq: o'rta yorug'lik 0.50, kontrast 0.32, to'yinganlik 0.30, R−B +0.145 (eng iliq); harakat 1.9 (statik).
- Musiqa nutq bilan deyarli bir darajada (pauza o'lchovi −0.5 dB) — bizda olinmaydi (qoida 9).
