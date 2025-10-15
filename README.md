# 🚀 Teljes projektindító terv: „Tanuló boxoló NPC-k Unity-ben”

## 🔧 1. Fejlesztői környezet beállítása

- ✅ Töltsd le és telepítsd a **Unity Hub**-ot
- ✅ Hozz létre egy új **2D projektet**
- ✅ Telepítsd a **Visual Studio**-t (ha még nincs), ez lesz a kódszerkesztőd

---

## 🎮 2. Egyszerű boxoló NPC létrehozása

**Cél:** Két karakter, akik tudnak mozogni és „ütni”

- Hozz létre két **Capsule GameObjectet** (ezek lesznek az NPC-k)
- Adj hozzá nekik:
  - `Rigidbody2D`
  - `BoxCollider2D`
  - `SpriteRenderer` (ha szeretnél karaktert)
- Készíts egy `BoxerAI.cs` scriptet:
  - Mozgás az ellenfél felé
  - Ha közel van, „ütés” (pl. életpont csökkentése)

---

## ❤️ 3. Életpont rendszer

**Cél:** NPC „meghal”, ha elfogy az élete

- Készíts egy `Health.cs` scriptet
- NPC kapjon sebzést, ha eltalálják
- Ha 0-ra csökken, `Destroy(gameObject)`

---

## 🧬 4. Evolúciós tanulás bevezetése

**Cél:** NPC-k viselkedésének fejlesztése generációkon át

- Hozz létre egy `DNA` osztályt (pl. sebesség, támadási gyakoriság)
- Generálj több NPC-t véletlenszerű értékekkel
- Harcoljanak → értékeld a teljesítményüket → válaszd ki a legjobbakat → új generáció

---

## 🧠 5. Megerősítéses tanulás (később)

**Cél:** Egy másik NPC, aki jutalmazás alapján tanul

- Telepítsd a **Unity ML-Agents** csomagot
- Hozz létre egy RL alapú NPC-t
- Tanítsd meg neki, hogy hogyan győzze le az ellenfelet

---

## 🥊 6. Összeeresztés és összehasonlítás

**Cél:** Evolúciós vs. RL NPC harca

- Hozz létre egy arénát, ahol egymás ellen küzdenek
- Mérd a győzelmeket, sebzést, túlélést
- Készíts statisztikát vagy grafikonokat

---

## 🧭 Hogyan tovább?

Ha szeretnéd, már most elkezdhetjük az első lépést: egy új Unity projekt létrehozását és az első NPC mozgás script megírását. Csak szólj, és diktálom a pontos lépéseket, vagy akár megírom a kódot is neked.
