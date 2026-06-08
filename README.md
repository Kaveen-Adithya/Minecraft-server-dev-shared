# ⚔️ Minecraft Server Project Manifest & Specification

Welcome to the official development blueprint and configuration manifest for the upcoming Minecraft Server Network. This document outlines the structural framework, core mechanics, economy systems, and feature rollouts required to build a premium, highly engaging player experience.

---

## 🧭 1. Core Network Architecture

### 🛡️ The Hub (Lobby)
The central gateway and first impression for all incoming players.
* **Purpose:** Portal matchmaking, community interaction, news displays, and cosmetic showcases.
* **Key Features:**
    * **NPC Navigation:** Interactive Citizens NPCs for seamless server routing.
    * **Parkour & Mini-activities:** Built-in lobby parkour with leaderboard tracking to keep waiting players engaged.
    * **Server Selector Menu:** Custom DeluxeMenus GUI styled around the server's central theme.

### 🏹 Main Game Mode: Survival Realms
* **New Identity:** **`Aetheria Survival: Fractured Lands`** *(Alternative Suggestions: Realm of Crowns, Valoria RPG, Primal Frontiers)*
* **Core Style:** An economy-driven, progression-heavy Survival experience combining traditional vanilla gameplay with deep RPG elements, clan warfare, and custom progression.

---

## 🔱 2. Clan System & Territorial Warfare
A quad-faction framework designed to foster competitive rivalries, community building, and tactical PvP.

### ⚜️ The Four Great Factions
| Clan | Associated Color | Theme & Lore Concept |
| :--- | :--- | :--- |
| **`Void Walkers`** | 🟣 Purple | Masters of the End, shadow magic, arcane technology, and dimensional travel. |
| **`Wildwood Collective`** | 🟢 Lime Green | Keepers of nature, ancient druid lore, stealth tactics, and rapid agility. |
| **`Frostguard Core`** | 🔵 Light Blue | Wardens of the northern peaks, defensive juggernauts, resilience, and heavy armor. |
| **`Vanguard Citadel`** | 🟠 Orange | Industrial conquerors, flame-wielders, siege masters, and tactical brute force. |

### 🛠️ Recommended Core Systems for Management:
* **Clan Levels & Perks:** Earn clan experience through active playtime, block breaking, and PvP kills to unlock shared vaults, custom clan per-member buffs, and distinct prefixes.
* **Territory Claims:** Integrated land claiming to secure clan bases, preventing griefing while maintaining structured raiding windows if war is declared.

---

## 🎖️ 3. Progression & Hierarchy (Custom Ranks)
A comprehensive 6-tiered structural ladder blending accessible free-to-play progression with premium options. Each rank introduces unique permissions, kits, and exclusive abilities.

### 📊 Rank Progression Framework
1.  **`Novice` [Greenhorn]** (Default Rank)
    * *Abilities:* Basic survival kit, single home set (`/sethome`), access to general public chat.
2.  **`Vagabond` [Scout]** (Playtime / Economy Unlock)
    * *Abilities:* Additional home slot, access to the `/ah` (Auction House) listing limits increased, `/back` command on death.
3.  **`Centurion` [Elite]** (Playtime / Economy Unlock)
    * *Abilities:* Auto-sorting chests, access to the workbench via command (`/wb`), exclusive chat colors.
4.  **`Chronos` [Champion]** (Advanced Progression / Special Unlock)
    * *Abilities:* **[Custom Ability] Time-Step:** Temporary speed boost and health regeneration when health drops below 25% (60s cooldown).
5.  **`Overlord` [Mythic]** (High-Tier Mastery Rank)
    * *Abilities:* **[Custom Ability] Void Aegis:** 3-second immunity to all incoming projectile attacks upon manual activation (`/ability`) (5-minute cooldown).
6.  **`Aetherial` [Immortal]** (Premium / Ultimate Achievement Tier)
    * *Abilities:* **[Custom Ability] Sovereign Wrath:** Emits a small, non-griefing shockwave pushing back hostile entities and rival players within a 5-block radius (10-minute cooldown). Fly access strictly within Hub and personal claims.

---

## 🎒 4. Custom Gear, Alchemy & Attributes
Moving beyond basic netherite to give players unique combat styles and endgame goals.

### 🧪 Advanced Alchemy (Custom Potions)
* **Haste Elixir (Tier I - III):** Grants mining speed increases outside of standard beacon ranges.
* **Vampiric Brew:** Converts 10% of dealt melee damage into immediate health regeneration for 15 seconds.
* **Gravity Vial:** Increases jump height significantly while eliminating fall damage entirely during active status duration.

### 🛡️ Mythic Armaments (Custom Armor, Tools & Weapons)
* **Armor Sets:** * *Reaper Set:* Full set gives a 15% damage multiplier during nighttime cycles.
    * *Titanium Exo:* Reduces structural knockback by 50% and enhances explosive resistance.
* **Tools & Combat Weaponry:**
    * *Tremor Pickaxe:* Built-in 3x3 explosive mining capability (toggled via sneak).
    * *Lifesteal Scythe:* Deals sweeping edge damage with a chance to siphon enemy hunger or health bars.

---

## 🪙 5. Unified Economy Ecosystem

```
             ┌────────────────────────────────────────┐
             │       Global Point & Coin Engine       │
             └───────────────────┬────────────────────┘
                                 │
         ┌───────────────────────┼───────────────────────┐
         ▼                       ▼                       ▼
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│   Server Shop   │     │  Player Shops   │     │  Auction House  │
│ (Admin Managed) │     │ (Player Driven) │     │  (Global Bids)  │
│ Core items, raw │     │ Rentable plots, │     │ P2P marketplace │
│ resources, food │     │ custom chests   │     │ for rare gear   │
└─────────────────┘     └─────────────────┘     └─────────────────┘
```

### 🏪 Macro-Economic Outlets
* **The Royal Market (`/shop`):** Static server economy used to anchor item values. Prevents inflation by regulating the prices of baseline raw materials, agriculture, and building blocks.
* **Merchant Districts (Player Shops):** Physically rentable plots inside designated economy hubs. Players can set up custom ChestShops to form hyper-localized trading hubs.
* **The Black Market (`/ah`):** Dynamic global auction house. Allows seamless peer-to-peer bidding and buyout options for custom gear, rare enchants, and legendary loot drops.
* **Point System (Premium/Voucher Currency):** Earned via voting, completing milestones, or hard dungeon clears. Used to purchase exclusive visual particles, custom titles, and key components for high-tier item forging.

---

## 🗺️ 6. Instanced PvE & Structured PvP Combat

### 🏔️ Instanced Dungeons & Arenas
* **Mechanic:** Separate, resetting worlds where squads can fight tiered boss entities.
* **Rewards:** Forging components for Custom Armor, Point vouchers, and high-tier Enchantment Books.

### 🧭 The Mystery Map (The Uncharted Frontier)
* **Concept:** A world map that automatically resets every 14 days with completely randomized seeds and custom structure generation algorithms.
* **High-Stakes Loot:** Standard claims are completely disabled here. Ore generation rates are tripled, encouraging high-risk, high-reward resource raids where PvP is permanently enabled.

### ⚔️ Combat Arenas (Structured PvP)
* Dedicated, lag-optimized arenas containing various preset layouts (e.g., Gladiator Pit, Ruined Citadel) utilizing standard fair-play dueling configurations, ranked leaderboards, and wagering mechanics.

---

## 📅 7. Strategic Feature Roadmap
Phased developmental structure designed to ensure server stability and sustained player retention.

### 🚀 Phase 1: Foundations (Alpha Testing)
* Setup of BungeeCord/Velocity proxy layer.
* Finalization of core Survival land management configuration.
* Balancing the base `/shop` economy and baseline 6-tier rank permissions.

### 🛠️ Phase 2: Refinement (Beta Launch)
* Introduction of Custom Armor, Tools, and Potion item tables.
* Opening the first Arena Dungeon layout for balance testing.
* Launch of the 14-day cycle Mystery Map.

### 🌟 Phase 3: Expansion (Future Updates)
* **Companion System (Pets Update):** Introduce functional utility pets providing minor passive stats (e.g., auto-pickup, speed modifiers, underwater breathing).
* **Custom Ability Expansion:** Adding custom ultimate abilities bound specifically to specialized playstyles chosen within the Clan System.
* **Cross-Server Tournaments:** Scheduled weekend events tracking structural clan wars and combat leaderboard resets.

---

## 🛠️ 8. Recommended Plugin Stack Architecture
For performance optimization, stability, and ease of feature maintenance:
* **Core Core Engine:** PaperMC / Purpur (1.20.x+)
* **Permissions:** LuckPerms
* **Land Management:** Lands / GriefPrevention
* **Factions/Clans:** SaberFactions / AdvancedClans
* **Economy Engine:** EssentialsX / Treasury / ExcellentShop / AuctionHouse
* **Custom Items:** MMOItems / EcoBits / CustomItems
* **Menu GUIs:** DeluxeMenus / PlaceholdersAPI
