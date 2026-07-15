Projekt: Chess Puzzle Web (React + TypeScript prototípus)

Leírás Ez egy kliens-oldali webalkalmazás prototípus sakkfeladványok megadására és automatikus megoldására. Főbb funkciók:

Szerkeszthető sakk tábla (drag & drop)
FEN beviteli mező
Feladatválasztó: "Mate in N" és "Deliver N checks without you checked"
Megoldás keresése depth-limited DFS-sel (helyi JS engine: chess.js)
SAN kimenet és lépések visszajátszása
Profi kinézet TailwindCSS-sel
Gyors indulás

Node 18+ és npm/yarn/pnpm telepítve.

Klónozd/hozd létre a mappát, majd illeszd be a fájlokat.

Telepítés: NPM telepítés vagy fonal

Indítás: NPM futtatása fejlesztője vagy Fonal fejlesztő

Megjegyzések

A kereső egyszerű, demonstrációs célú és nem optimalizált (nincsenek transzpozíciós table-ek, alpha-beta, stb.). Komolyabb feladatokra célszerű továbbfejlesztőni a motort.
A "Deliver N checks without getting checked" feladat definíciója: keresünk olyan játékfolyamatot, ahol a kezdő oldal (side to move) N alkalommal ad checket a saját lépésein, és a kezdő oldal soha nem lesz sakkban (nem él át sakkot) a teljes variáns alatt. (Amennyiben más definíciót szeretnél, módosítom.)
Fejlesztési javaslatok

Alpha-Beta + TT + Iterative Deepening hozzáadása a gyorsabb, mélyebb keresésekhez.
WebWorkerbe helyezni a keresőt, hogy nagy keresések blokkolás nélkül fussanak.
További puzzle típusok és hint rendszer.
Szerveres backend / WebAssembly motor (Rust/C++) ha nagyobb teljesítmény kell.
