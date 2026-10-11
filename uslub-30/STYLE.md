# Uslub 30 — "Tabassum" (A oila, Ekspert shaxsiyati — premium tashqi kadr, foydalanuvchining o'z namunasi)

Manba: /Users/user/Downloads/birlashgan_tabassum_final_v2.mp4 (= _src/tabassum_v2.mp4), 32.0 s, 1080x1920, 30 fps, -14.0 LUFS.
Mavzu: diniy-axloqiy maslahat (sadaqa / ehson / tabassum), bitta spiker tashqarida (park), 2 burchak (old + yon profil).
Keyframes: keyframes/seg_00..30.jpg (4 fps, 6 s bo'laklar), zz.jpg (elementlar yaqindan).
Andoza: reel-montaj `templates/compose.example.py` + `index.tpl.example.html` (A oila) — aynan shu elementlar to'plami.

## O'lchangan ritm
- 11 kesim / 32 s (kesim har ~2.7 s, kadr median 2.26 s); 9/11 kesim SO'Z ICHIDA (ovoz uzluksiz, kadr almashadi).
- Virtual kamera: keng 1.0 / o'rta ~1.3 / yaqin ~1.7 navbatlashadi + yon profil burchagi; har kadr ichida sekin push.
- Nutq 137 so'z/daq, pauzalar olinmagan.

## Rang
Kino teal-orange: qora nuqta chuqur (luma p2 ~0.005), o'rtacha qorong'i (p50 ~0.25), to'yinganlik ~0.38, iliqlik R-B ~+0.05,
kuchli vinetka, pastki 40% qorayish gradiyenti (subtitr uchun). B-roll'larning bir qismi to'liq OQ-QORA (ma'yus/salbiy gap).

## Elementlar (vaqt — namunadagi)
| # | Element | Qachon ishlatiladi | Ko'rinishi |
|---|---|---|---|
| 1 | `[ so'z ]` qavsli subtitr | oddiy gap | oq Inter 500 ~44 px, qavslar OLTIN #e8b96a, ko'krak balandligi markazda, 1–3 so'zdan bo'lak |
| 2 | Bosh ORTIDAGI katta so'z | asosiy tushuncha (EHSON 3.8 s, TABASSUM 21.3 s) | Poppins 800 krem #f9f0da ~260 px, tepada, spiker kesmasi ustida (rembg matte), pastdan ko'tariladi, oltin uchqunlar |
| 3 | Ierarxik iqtibos (3 qator) | savol / muhim gap ("Bu sadaqami / yoki ehsonmi? / deb so'rardilar.") | chapda pastda: kichik italic -> katta Poppins 700 -> kichik italic, so'zma-so'z blur |
| 4 | Doira shisha ikon-badj | gapdagi predmet (🎁 sovg'a, ✕ inkor, 👁 ko'rish, ♥ yakun) | ~90 px shisha doira, spiker yonida (yuzga tegmaydi), ichida oq chiziqli ikonka |
| 5 | Split-ekran B-roll | misol/harakat (sovg'a uzatish, qo'l berib so'rashish) | pastki yarim B-roll, OQ ingichka chiziq, spiker yuqoriga suriladi, subtitr "up" |
| 6 | Shisha taqqoslash qatorlari | ikki tushuncha farqi | to'q shisha plashka: italic krem kalit so'z + oltin nuqta + oq izoh, 2-qator pastdan, oxirida oltin ✓ va tagiga chiziq |
| 7 | To'liq ekran OQ-QORA B-roll + chapda oddiy subtitr | umumiy jamiyat holati ("Hozirgi kunda hammamiz…") | oq Inter, chap-pastda, so'zma-so'z |
| 8 | Shisha o'lchagich | sifat/daraja ("Tabassum 100% -> 12%") | pill: italic kalit so'z + oltin chiziq + raqam; kamayishda oq-qora B-roll (ma'yus yuz) |
| 9 | Light leak / flash o'tish | bo'limlar orasida | iliq to'q-sariq yorug'lik 0.5–0.8 s |
| 10 | Yakuniy chaqiriq | xulosa ("Sadaqa qiling.") | katta italic Poppins + ostida oltin chiziq chiziladi |
| 11 | Salom / yakun | "Assalomu alaykum" | kichik italic + qisqa oltin chiziq, ♥ badj, sekin so'nish |

## Audio
Sokin musiqa (pauzada -22 dBFS, nutq -14) — bizning qoida 9 bo'yicha musiqa nutqdan >=19 dB past bo'ladi.
SFX siyrak: kesimlarda yengil whoosh, badj pop, chizilish.

## Silliqlik
Hamma kirish 0.5–0.8 s expo.out + blur, chiqish 0.4–0.5 s, overshoot yo'q (smooth-motion.md).
