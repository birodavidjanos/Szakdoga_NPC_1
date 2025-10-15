# 🧠 Tanuló NPC-k Harca Unity-ben

## 🎮 Játék koncepciója

Ez egy 2D oldalnézeti harci játék, ahol két mesterséges intelligenciával vezérelt NPC küzd meg egymással:

- **Pap (RL tanulás)**: fekete köpenyben, mágikus harcos. A köpeny eltakarja a lábait, így nem kell megtanulnia járni. Döntéseit megerősítéses tanulással hozza.
- **Ördög (evolúciós tanulás)**: látható lábakkal rendelkező fizikai harcos. Mozgása előre programozott, viselkedését evolúciós algoritmus fejleszti.

Mindkét karakter képes:
- Ütni
- Védekezni
- Rúgni
- Ugrani

---

## 🔧 Fejlesztői környezet

- Unity Hub + Unity 2D projekt
- Visual Studio (C# scripteléshez)
- ML-Agents csomag (RL tanításhoz)

---

## 🧱 Alapjáték felépítése

### 1. Karakterek létrehozása
- Pap: fekete köpeny, lebegő mozgás
- Ördög: páncélos, látható lábak, négy akcióval

### 2. Mozgás és harc script
- `BoxerAI.cs`: mozgás, támadás, védekezés, ugrás
- `Health.cs`: életpont rendszer, sebzés, halál

### 3. Aréna
- Egyszerű 2D pálya
- Platformok, akadályok (később)
- Kamera követés, UI életpont kijelzés

---

## 🧬 Evolúciós tanulás (Ördög NPC)

- `DNA.cs`: paraméterek (pl. támadási gyakoriság, védekezési hajlam)
- Generációk: harc → értékelés → szelekció → új generáció
- Tanulás célja: hatékony harci viselkedés

---

## 🧠 Megerősítéses tanulás (Pap NPC)

- ML-Agents konfigurálása
- Akciók:
  - 0: semmit nem csinál
  - 1: ütés
  - 2: védekezés
  - 3: rúgás
  - 4: ugrás
- Jutalmazás:
  - Sikeres támadás → +10
  - Védekezés jó időben → +5
  - Elhibázott akció → -3
  - Tétlenség → -1

---

## 🥊 Összeeresztés és tesztelés

- RL Pap vs. Evolúciós Ördög
- Több harc szimulálása
- Statisztikák gyűjtése:
  - Győzelmek aránya
  - Átlagos sebzés
  - Viselkedésminták

---

## 📈 További bővítések (később)

- Speciális képességek (pl. varázslat, roham)
- Akadályok, mozgó platformok
- Többféle NPC, csapatok, AI versenyek
