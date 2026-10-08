# Victor Wembanyama – interaktív rajongói oldal 👽
 
Egyetlen HTML fájlból álló, interaktív weboldal Victor Wembanyamáról, a San Antonio Spurs francia kosarasáról. Sötét, kosárlabdás stílus, Bootstrap 5-tel és saját JavaScripttel.
 
> Nem hivatalos rajongói oldal. Nincs kapcsolatban Wembanyamával, az NBA-vel vagy a Spurs-szal.
 
## Mit tud az oldal?
 
| Rész | Leírás |
|---|---|
| **Hero** | Címsor és Spurs-mezes fotó, a kép széle elhalványul a háttérbe |
| **Mérd magad hozzá** | Csúszkával beállítod a magasságod, az oldal kirajzolja a különbséget Wembanyához (224 cm) képest |
| **Számok** | Négy kártya, amelyekre kattintva megfordulnak. A számok felfutnak betöltéskor |
| **Galéria** | Trófeás fotó és egy rajongói grafika, utóbbi alatt pontosító felirattal |
| **Blokkolós játék** | 20 másodperces minijáték: a felbukkanó labdákra kell kattintani, mielőtt eltűnnek. Számolja a blokkokat, a kihagyottakat és a rekordot |
| **Az útja** | Bootstrap harmonika: francia kezdetek, 2023-as draft, újonc év, olimpia, sérülés |
| **Furcsaságok** | Bootstrap fülek: pályán, pályán kívül, becenevek |
| **Kvíz** | 5 kérdéses feleletválasztós teszt pontszámmal |
| **Lábléc** | Csapatünneplős fotó az oldal alján |
 
## Használt technológiák
 
- **HTML5 + CSS3** egyedi stílussal (CSS változók, 3D kártyaforgatás, animációk)
- **[Bootstrap 5.3.3](https://getbootstrap.com/)**: rács, harmonika, fülek, gombok, progress bar, sötét téma
- **Vanilla JavaScript**: magasságmérő, számlálók, játék, kvíz (külső könyvtár nélkül)
- **Google Fonts**: Anton (címsorok) és Barlow (szöveg)
## Futtatás
 
Nincs telepítés és build lépés.
 
1. Töltsd le a `wembanyama.html` fájlt.
2. Nyisd meg bármelyik böngészőben.
Ha GitHub Pages-en szeretnéd kiadni, nevezd át `index.html`-re, majd a repo **Settings → Pages** menüjében válaszd ki a főágat.
 
## Fontos tudnivalók
 
- A **Bootstrap CSS és JS be van ágyazva** a fájlba, és a **képek is base64-ként vannak benne**, ezért a fájl nagy (kb. 0,8 MB), viszont egyetlen fájlként bárhová átvihető, és internet nélkül is működik. Kivétel a két Google betűtípus: ezek nélkül az oldal tartalék betűtípusokra vált.
- A **számok megközelítőleg értendők**. A galériában lévő rajongói grafikán szereplő 7'7" és 8'3" eltúlzott, a hivatalos magasság kb. 224 cm.
- A képek szerzői jogai a jogtulajdonosokat illetik. Publikus használat előtt ellenőrizd, hogy felhasználhatod-e őket.
## Egyszerű módosítások
 
- **Kvíz kérdései:** a szkriptben a `Q` tömb. Egy kérdés formája: `["Kérdés?", ["válasz1","válasz2","válasz3","válasz4"], helyesIndex]`.
- **Játék hossza:** a `left=20` érték és a `20` másodperc a játék szkriptben.
- **Színek:** a `<style>` elején a `:root` változói (`--hot`, `--ice`, `--silver`).
- **Új kártya:** másolj ki egy `.flip` blokkot a „Számok" szekcióban, és írd át a szöveget.
## Fájlok
 
```
wembanyama.html   – a teljes oldal (HTML, CSS, JS, Bootstrap és képek)
README.md         – ez a leírás
```
 