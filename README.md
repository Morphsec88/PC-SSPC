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

### Dynamic Load Control (Pneumatic Actuation)
*   **Sequential Switching (Voltage Stabilization):** Unlike chemical batteries, the control electronics sequentially engage individual cell matrix blocks as active cassettes discharge. This progressive activation maintains a highly stable output voltage curve across the entire operating cycle, eliminating the need for inefficient heavy DC-DC step-up conversion.
*   **Simultaneous Engagement (Boost Mode):** When the system demands maximum torque or an immediate power surge (e.g., heavy machinery startup), the pneumatic block inflates all membranes simultaneously, delivering peak current density instantly.
*   **Zero-Power Static Retention:** The pneumatic capillary network operates as a closed, valve-controlled system. Energy is only consumed during the milliseconds required to inflate or vent a chamber; once a state is set, the valves lock the pressure, maintaining mechanical contact with zero continuous parasitic power draw.

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

## Operational Ecosystem & Modular Scaling

To seamlessly integrate the PC-SSPC architecture into the commercial market, the operational model is built around automated corporate logistics rather than traditional retail consumer charging:

*   **B2B Fleet Operations:** The system is primarily engineered for commercial, industrial, and heavy-duty vehicles. Battery replenishment and management are handled exclusively by corporate fleet operators at dedicated depots, removing the charging infrastructure burden from individual end-users.
*   **Standardized Modular Slots:** The external chassis and potential cassettes are designed with a universally standardized geometric form factor. This enables automated drive-in service stations where robotic arms can instantly slide out depleted cassettes and hot-swap them with fully re-polarized units in under a minute.
*   **Extended Range Scaling (Auxiliary Cargo Storage):** Due to the dry, non-volatile, and safe nature of the solid-state architecture, users can purchase additional standalone cassettes. According to the design framework, these modular units can be safely transported in the cargo beds of utility vehicles (e.g., pickup trucks) or larger trunks to serve as plug-and-play range extenders for remote off-grid operations.

A kiegészítő pneumatika és a robusztus kazettaszerkezet miatt a PC-SSPC **fizikailag nagyobb térfogatú és nehezebb**, mint egy azonos kapacitású Li-ion akkumulátor. 

Ez a tömeg- és méretnövekedés egy tervezett mérnöki kompromisszum.
A gyártás a nagyobb felépítésű járművek (SUV, teherautók, vonatok, hajók) és a hálózati energiatárolás (Grid) esetében válik kifizetődővé a következők miatt:
*   **Életciklus-költség:** Nem igényel időszakos, méregdrága akkupakk-cserét, túlélve a jármű élettartamát.
*   **Abszolút biztonság:** A gyúlékony elektrolitok hiánya és a milliszekundumos pneumatikus vészlekapcsolás megszünteti a tűzveszélyt.

## Licenc

Ez az architektúra és koncepció a **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** licenc alatt áll. 

A licenc feltételei szerint szabadon megoszthatod és átdolgozhatod a projektet, feltéve, hogy megjelölöd a szerzőt (**Attribution**),
és az átdolgozott anyagokat ugyanezen licenc alatt terjeszted (**ShareAlike**).
