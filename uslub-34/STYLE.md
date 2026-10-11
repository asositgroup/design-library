# Uslub pasporti — uslub-34 "Cutout-kollaj + oltin glow" (Jason Pro @jasonp.media, reel DdltV3FsZsw)

Referens: BMW M4, cho'l, oltin soat. 1080x1920, 60 fps, 18.02 s, nutqsiz va matnsiz, faqat musiqa (161.5 BPM, 1 takt = 1.486 s).
Asosiy g'oya: kesimlar deyarli yo'q (detektor 2 ta topgan). Hikoyani fon ustiga qo'yilgan **rotoskop qatlamlar** quradi.
Fondan qirqib olingan mashina yoki uning qismi har takt / yarim taktda kadr chetidan sirg'alib kiradi.

| Jihat | Referens (o'lchangan, 10 fps strip) | Bizda (moslash) |
|---|---|---|
| Tuzilma | A 0–6.08 kollaj-stek · B 6.08–9.8 to'liq kadr + obyekt-wipe/iris · C 9.8–12.07 qatlam + rul glow · D 12.07–18 yonma-yon cutout, ghost, kulrang fon | xuddi shu 4 qism, shu musiqa, bir xil grid |
| Ritm | yangi qatlam har 0.743 s (2 zarba): downbeat 0.07/1.58/3.07/4.57/6.08… va yarim takt | grid audiomap'dan |
| Qatlam kirishi | chetdan (tepa/past/chap/o'ng) ~0.15–0.2 s, motion-blur bilan, overshootsiz | xPercent/yPercent + blur 0.18 s power3.out |
| Oltin glow | qatlam avval to'q-oltin tana + neon qirralar ko'rinishida chiqadi, ~0.5 s da haqiqiy teksturaga o'tadi (0.1→0.7, 1.6→2.3, 3.0→3.7, 4.6→5.3) | `_glow.webm` (Canny qirralar + kontur, #FFB23C halo, #FFECBE yadro) → `real.webm` crossfade 0.45 s |
| Rul glow | 11.3 s: rul konturi ko'k neon → oltinga o'tadi | 6424 rul doira-kesmasi, hue ko'k→oltin |
| Obyekt-wipe | 6.7: mashina tanasi old planda diagonal o'tadi; 7.6: arka chapdan | 6447 cutout x3 masshtabda 0.3 s da kadrni kesib o'tadi, orqasida kesim |
| Iris | 8.1–8.4: shina halqasi kadrni yopadi; 9.7: disk ichidan keyingi kadr ochiladi | clip-path circle, g'ildirak markazidan |
| Ghost | 10.4, 16.3: yuqori qatlam opacity 1→0 (~0.15 s) | opacity 0.15 s |
| Fon | to'liq kadr, xiralashtirilmagan; yakunda (17.8) fon kulrang, mashina rangli | studiya kadrlari; 17.7 da fon grayscale(1) |
| Rang | luma p50 0.35–0.39, kontrast 0.19–0.27, to'yinganlik 0.30–0.37, iliq R-B +0.13 (quyosh botishi) | studiya oq va binafsha tusli: binafshani yo'qotish, biroz iliq, kontrast + (to'liq "cho'l" ko'chirilmaydi, oq mashina sarg'ayadi) |
| Kamera | gimbal, doimiy harakat (motion 15–19) | iPhone kadrlarining o'z harakati + yengil push |
| Matn | yo'q | yo'q |
| Audio | faqat musiqa, -14.2 LUFS | xuddi shu trek |
| OLINMAYDI | — | cho'l/oltin soat rangi (sahna boshqa), Dubai raqami va M4 kadrlari (bizda faqat foydalanuvchi footage'i) |
