<div align="center">

# 🏭 SrTownyFactory
### Enterprise Strategic Resource Factories & Rise of Kingdoms Territorial Warfare

[![Java 21](https://img.shields.io/badge/Java-21_LTS-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)](https://openjdk.org/)
[![PaperMC](https://img.shields.io/badge/PaperMC-1.21.x-1F8CEB?style=for-the-badge&logo=minecraft&logoColor=white)](https://papermc.io/)
[![Version](https://img.shields.io/badge/Version-3.0.0-38BDF8?style=for-the-badge)](https://github.com/croxln/SrTownyFactory)
[![Status](https://img.shields.io/badge/Status-🟢_Active_Production-4ADE80?style=for-the-badge)](https://github.com/croxln/SrTownyFactory)
[![Stars](https://img.shields.io/github/stars/croxln/SrTownyFactory?style=for-the-badge&color=FACC15&logo=github)](https://github.com/croxln/SrTownyFactory/stargazers)
[![License](https://img.shields.io/badge/License-Proprietary-EF4444?style=for-the-badge)](https://github.com/croxln/SrTownyFactory)

<p align="center">
  <b>SrTownyFactory</b> introduces large-scale territorial warfare and industrial automation to Minecraft Towny servers.<br>
  Towns advance their border claims across the open world, contest strategic landmark factories, and engage in high-intensity King of the Hill siege battles using persistent war flags.
</p>

</div>

---

### 🌟 Core Architectural Highlights

```text
 ┌─────────────────────────────────────────────────────────────────────────────┐
 │                         RISE OF KINGDOMS WARFARE                            │
 │                                                                             │
 │   [ Town Border Claim ] ────► [ Adjacent Claim ] ────► [ Kuşatma Bayrağı ] │
 │                                                              │              │
 │                                                              ▼              │
 │                   [ 30-Min King of the Hill Battle ]                        │
 │                                  │                                          │
 │                  ┌───────────────┴───────────────┐                          │
 │                  ▼                               ▼                          │
 │           [ Victory: 🏆 ]                 [ Defeat: 🛡️ ]                    │
 │        Ownership Transferred             Ownership Retained                 │
 │       1-Hour Peace Shield Shield         Territory Preserved                │
 └─────────────────────────────────────────────────────────────────────────────┘
```

- **👑 Rise of Kingdoms Territory Mechanics:** Chunks with strategic factories cannot be claimed passively via `/t claim`. Towns must build connected claim lines touching the factory border, then deploy a **Kuşatma Bayrağı (War Flag)** to initiate conquest.
- **⚔️ Modern King of the Hill (KotH) Sieges:** 30-minute timed battles featuring single-controller area control, proximity-based boss bars with live progress percentages, and attacker/defender point tallies.
- **🏭 16 Industrial & Strategic Branches:**
  - `MADEN` (Mining: Coal, Copper, Iron, Gold, Redstone, Lapis, Emerald, Diamond)
  - `TARIM` (Agriculture: Wheat, Carrot, Potato, Cattle, Golden Apples, Enchanted Golden Apples)
  - `ASKERI` (Military: Armors, Weapons, Spectral Arrows, TNT, Kuşatma Bayrağı Supplies)
  - `BUYUCULUK` (Sorcery: Bookshelves, Brewing Stands, Bottles of Enchanting, Ender Eyes)
  - `KADIM_ESER` (Ancient Relics: Netherite, Heart of the Sea, Echo Shards, Totems, Elytra)
  - `NETHER` (Nether: Blaze Rods, Nether Warts, Magma Cream, Ancient Debris, Wither Skulls)
  - `WOOD` & `STONE` (Core Construction: All wood variants, deepslate, stone)
- **🗺️ Live Web Map Integration (Squaremap):** High-definition map layer showcasing factories with medieval heraldic swallowtail flags, town owner tags, immunity shields, and clean Minecraft item texture grids.
- **📜 Monetization & Slot Licensing:** Configurable town factory capacity limits with consumable `+1 Fabrika Kurulum Lisansı (Extra Factory Slot License)` vouchers.
- **💰 Multi-Economy Procurement:** Town officials procure Kuşatma Bayrağı supplies directly from town bank reserves (`Kasaba Askeri Bütçesi`), seamlessly cycling server currency.

---

### 💻 Command Reference

| Command | Permission | Description |
| :--- | :--- | :--- |
| `/fabrika` | `srtownyfactory.factory.use` | Opens the modern Town Industry (`Kasaba Sanayisi`) GUI hub |
| `/fabrika bayrak` | `srtownyfactory.factory.use` | Procures a Kuşatma Bayrağı from the town military bank |
| `/fabrika stratejik liste` | `srtownyfactory.factory.use` | Lists all open-world strategic landmark factories |
| `/fabrika stratejik bilgi [id]` | `srtownyfactory.factory.use` | Inspects rates, status, and connected towns for a factory |
| `/fabrika stratejik topla [id]` | `srtownyfactory.factory.use` | Collects accumulated yields from town factory storage |
| `/fabrika olustur <isim> <tür>` | `srtownyfactory.admin` | Creates and registers an open-world landmark factory |
| `/fabrika sil [onayla]` | `srtownyfactory.admin` | Permanently deletes a factory from the world and database |
| `/fabrika admin flagver <p> [n]` | `srtownyfactory.admin` | Admin utility to grant war flags directly to players |

---

### 🛡️ Technical Specifications

- **Target Engine:** PaperMC 1.21.x / Folia (Java 21 LTS)
- **Persistence:** SQLite / MySQL via HikariCP Connection Pooling
- **Spatial Lookups:** $O(1)$ spatial chunk hashing keying `world:chunkX:chunkZ`
- **Text & Components:** Kyori Adventure MiniMessage with clean small-caps formatting
- **Dependencies:** SrTowny (Core Fork), Towny Advanced, Vault, Squaremap

---

### 📈 Repository Star History

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=croxln/SrTownyFactory&type=Date&theme=dark)](https://star-history.com/#croxln/SrTownyFactory&Date)

</div>

---

> [!IMPORTANT]
> **Source Code Notice:** This repository is a public architectural showcase, issue tracker, and documentation center for the **SrProjects** private server network. Source code is closed-source and proprietary.

<div align="center">
<sub>Engineered by <b>-Serhat (croxln)</b> • Part of the SrProjects Suite</sub>
</div>
