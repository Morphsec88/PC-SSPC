# PC-SSPC

# Pneumatically Controlled Solid-State Potential Cell (PC-SSPC)

A PC-SSPC egy tisztán fizikai, szilárdtest-alapú energiatárolási koncepció heavy-duty és stationary alkalmazásokhoz.
A rendszer elektrosztatikus potenciálmagok és egy pneumatikusan vezérelt, rugalmas membrán-interfész kombinációjára épül, 
kiváltva a hagyományos kémiai (pl. Li-ion) akkumulátorokat.

## Kulcsfontosságú elemek

*   **Potential Cassette (Mag):** Száraz, cserélhető, kettős rekeszű egység (Charged és Uncharged zónák).
*   A belső mag ultrahangos marással strukturált, mikroméretű lamellákból álló porózus mátrix.
*   Unipoláris felépítése miatt nincs belső feszültségkülönbség vagy ívkisülés-veszély.
*   **Pneumatic Control Block (Aktuátor):** Sűrített levegővel működtetett kapilláris rendszer,
*    amely egy fémbevonatú gumimembránt deformál sík állapotból „C” profilúvá, mechanikus kontaktust létrehozva a kazetta fix termináljaival.
*   **Buffer Capacity (Stabilizátor):** Kondenzátortelep, amely tompítja a kezdeti áramlökéseket és simítja a külső terhelés felé menő kimenetet.

## Működési elv és vezérlés

### Működési ciklus
1.  **Standby (Fail-Safe):** Lapos membrán, fizikai légrés, tökéletes galvanikus leválasztás, 0% önkisülés.
2.  **Activation:** A sűrített levegő C-alakúra fújja a membránt, zárva a mechanikus hidat.
3.  **Buffering & Output:** Az áram feltölti a kondenzátortelepet, amely kiszolgálja a külső terhelést.
4.  **Depletion & Swap:** A kazetta 0 Voltig kisüthető szerkezeti károsodás nélkül, majd kicsúsztatható és újra polarizálható.

### Terheléskezelés (Pneumatikus vezérlés)
*   **Szekvenciális kapcsolás:** Normál üzemben a szelepek folyamatosan, egymás után aktiválják a cellákat az egyenletes teljesítményért.
*   **Simultán kapcsolás (Boost mód):** Extrém nyomatékigény esetén (pl. nehézgépjármű indítása)
*    a rendszer az összes cellát egyidejűleg rákapcsolja a hálózatra a maximális áramsűrűségért.

## Technikai összehasonlítás

<img width="3268" height="1728" alt="PC-SSPC" src="https://github.com/user-attachments/assets/4a2bb7fb-876c-4222-9c76-0c6cd3628487" />

| Jellemző | Lithium-Ion | PC-SSPC |
| :--- | :--- | :--- |
| **Tárolási mechanizmus** | Kémiai reakció | Fizikai / Elektrosztatikus felület |
| **Önkisülés** | Magas (~2-5% / hónap) | Abszolút nulla (évtizedekig stabil) |
| **Ciklusélettartam** | 1 000 - 3 000 ciklus | Végtelen (nincs kémiai degradáció) |
| **Kisütési tartomány** | 3.0V - 4.2V (0V-nál tönkremegy) | 0V-ig biztonságosan kisüthető |
| **Biztonság / Leválasztás** | Termikus megfutás veszélye | Azonnali mechanikus lekapcsolás (levegőleeresztés) |
| **Környezeti hatás** | Kritikus bányászat (Li, Co) | Száraz fémek, teljesen újrahasznosítható |

## Mérnöki kompromisszum és pozicionálás

A kiegészítő pneumatika és a robusztus kazettaszerkezet miatt a PC-SSPC **fizikailag nagyobb térfogatú és nehezebb**, mint egy azonos kapacitású Li-ion akkumulátor. 

Ez a tömeg- és méretnövekedés egy tervezett mérnöki kompromisszum.
A gyártás a nagyobb felépítésű járművek (SUV, teherautók, vonatok, hajók) és a hálózati energiatárolás (Grid) esetében válik kifizetődővé a következők miatt:
*   **Életciklus-költség:** Nem igényel időszakos, méregdrága akkupakk-cserét, túlélve a jármű élettartamát.
*   **Abszolút biztonság:** A gyúlékony elektrolitok hiánya és a milliszekundumos pneumatikus vészlekapcsolás megszünteti a tűzveszélyt.

## Licenc

Ez az architektúra és koncepció a **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** licenc alatt áll. 

A licenc feltételei szerint szabadon megoszthatod és átdolgozhatod a projektet, feltéve, hogy megjelölöd a szerzőt (**Attribution**),
és az átdolgozott anyagokat ugyanezen licenc alatt terjeszted (**ShareAlike**).
