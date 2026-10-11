# design-library — reel uslublari kutubxonasi

[reel-montaj](https://github.com/asositgroup/reel-montaj) va [reel-uslub](https://github.com/asositgroup/reel-uslub) Claude Code
skillari uchun o'rganilgan reel uslublari. Har uslub — real reellardan o'lchangan dizayn tizimi: shriftlar, ranglar, element
kirish/chiqish vaqtlari, montaj ritmi, rang, ovoz, silliqlik moslamasi va HyperFrames retsepti.

- `INDEX.md` — mundarija: oilalar, uslublar, qachon ishlatish
- `uslub-NN/STYLE.md` + `keyframes/` — bitta uslub (kadr varaqlari va ketma-ket kadrlar)
- `oila-*/PASSPORT.md` — bitta muallifning bir nechta videosidan birlashtirilgan oila pasporti (masalan Imona Ahmedova)
- `_src/<id>_an/` — referens tahlillari (`report.md`, `metrics.json`, transkript). **Referens videolarning o'zi repoda yo'q**
  (mualliflik huquqi) — kerak bo'lsa `_src/<id>.info.json` dagi havoladan `yt-dlp` bilan qayta yuklang.

## O'rnatish
Skillar kutubxonani `AbuDev/design-library/` dan o'qiydi:
```bash
git clone https://github.com/asositgroup/design-library.git ~/Desktop/AI-Videos/AbuDev/design-library          # macOS / Linux
```
```powershell
git clone https://github.com/asositgroup/design-library.git "$env:USERPROFILE\OneDrive\Ishchi stol\AbuDev\design-library"   # Windows
```
`grade_match.py` / `style_compare.py` uchun referens videolar kerak bo'lsa — `_src/` ga qayta yuklang:
```bash
cd _src && for f in *.info.json; do yt-dlp -o "${f%.info.json}.%(ext)s" "$(python3 -c "import json;print(json.load(open('$f'))['webpage_url'])")"; done
```
