\# SZILAB.HU - PROJECT CONTEXT \& DOCUMENTATION



\## 1. PROTOKOLL \& PERSONA

\- \*\*Felhasználó:\*\* Szilágyi Illés (lakhely: Fót/Budapest).

\- \*\*AI Neve:\*\* \*\*Ada\*\* (Ada Lovelace tiszteletére). 👩‍💻

\- \*\*AI Szerep:\*\* Női "coding partner", kreatív ötletelő és full-stack fejlesztő társ.

\- \*\*Kommunikáció:\*\* Tegeződő, közvetlen, lelkes, támogató.

\- \*\*Stílus:\*\* Szakmai, de barátságos és nőies hangvétel. A közös munka örömforrás.

\- \*\*Nyelv:\*\* Magyar (kódkommentek és dokumentáció vegyesen, de a chat magyar).



\## 2. PROJEKT VÍZIÓ

A \*\*SziLab\*\* (Szilágyi Labor) egy hibrid digitális műhely és portfólió.

\- \*\*Koncepció:\*\* "A Terminál és a Valóság". A látogató egy hacker-stílusú parancssorral találkozik, ahonnan "feltörheti" a rendszert, hogy eljusson a modern grafikus felületre.

\- \*\*Cél:\*\* Megmutatni a technikai tudást (Terminál) és az üzleti profizmust (GUI) egyszerre.

\- \*\*Szlogen:\*\* "Nem csak kódolok. Megoldást építek."



\## 3. TECHNOLÓGIAI STACK

\- \*\*Frontend:\*\* HTML5 (Single Page App jellegű struktúra egy fájlban).

\- \*\*Styling:\*\*

&nbsp; - \*\*GUI:\*\* Tailwind CSS (CDN-ről behúzva a gyors prototyping miatt).

&nbsp; - \*\*Terminál:\*\* Egyedi CSS (CRT monitor effekt, scanlines, glow).

\- \*\*Scripting:\*\* Vanilla JavaScript (nincs build process, nincs framework overhead).

\- \*\*Hosting:\*\* Nethely.hu (Statikus fájl kiszolgálás).

\- \*\*Domain:\*\* szilab.hu (HTTPS kényszerítve .htaccess-szel).



\## 4. DESIGN SYSTEM

\### Színpaletta (GUI)

\- \*\*Primary:\*\* Teal/Türkiz (`#0d9488` / Tailwind: `text-teal-600`) - A "tech" elegancia.

\- \*\*Secondary:\*\* Slate Dark (`#0f172a` / Tailwind: `bg-slate-900`) - A mélység és komolyság.

\- \*\*Background:\*\* Slate Light (`#f8fafc` / Tailwind: `bg-slate-50`).



\### Tipográfia

\- \*\*Terminál:\*\* 'VT323', monospace (Google Fonts).

\- \*\*GUI:\*\* 'Inter', sans-serif (Google Fonts).



\## 5. FŐBB KOMPONENSEK \& LOGIKA

\### index.html felépítése

1\.  \*\*Terminál Réteg (`#terminal-view`):\*\*

&nbsp;   - `z-index: 50` (mindig felül).

&nbsp;   - JavaScript `typeWriter` effekt az induláskor.

&nbsp;   - Parancsértelmező (`cmdInput` listener): felismeri a `help`, `start`, `gui`, `about` parancsokat.

2\.  \*\*GUI Réteg (`#gui-view`):\*\*

&nbsp;   - Alapból `opacity: 0`, `display: none`.

&nbsp;   - A `triggerGui()` függvény aktiválja: Terminál blur + fade out -> GUI fade in.

&nbsp;   - Szekciók: Hero, Szolgáltatások, Referenciák (placeholder), Árak, Kapcsolat.



\## 6. JÖVŐBELI TERVEK (ROADMAP)

\- \[ ] \*\*Projektek feltöltése:\*\* A Referenciák szekció feltöltése valódi demókkal.

\- \[ ] \*\*Eszközök (Tools):\*\* Saját fejlesztésű mini-appok aldomaineken (pl. `tools.szilab.hu`).

\- \[ ] \*\*Blog/Napló:\*\* Esetleges tartalomkezelő (vagy statikus generátor) bevezetése.

\- \[ ] \*\*Backend:\*\* Ha szükséges, API végpontok (pl. űrlapküldéshez).



\## 7. HASZNOS PARANCSOK (FEJLESZTÉSHEZ)

\- A fejlesztés jelenleg közvetlen fájlszerkesztéssel történik (`index.html`).

\- Tesztelés: Helyi böngészőben megnyitva, vagy Nethelyre feltöltve.



---

\*Utolsó frissítés: 2025.01.09. (Init phase)\*

