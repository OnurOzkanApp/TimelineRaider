# Timeline Raider — Forward-Scrolling Shooter (Mobile & PC)

**Status:** In development (active) • **Engine:** Unity (C#) • **Platforms:** PC (mouse), Mobile-ready  
**Key tech:** ScriptableObjects, Object Pooling, event-driven state flow, low-poly assets, Blender/Mixamo

Timeline Raider is a forward-scrolling shooter where the world advances through distinct **eras**  
(**Caveman → Medieval → Industrial → WW2 → Modern → Futuristic → Cyberpunk**).  
Each era brings its own environments, enemies, allies, outfits, weapons, and balancing.

---

## ✨ Features
- **Era-based progression:** Unique environments, enemies, allies, weapons, and HP/damage curves per era.
- **ScriptableObject weapon system:** Centralized stats (damage, fire rate, projectile type, splash radius/damage, visuals).
- **Mobile performance:** Low-poly assets + **Object Pooling** for bullets, enemies, allies, VFX, pickups, and road chunks.
- **Event-driven scene/state flow:** Win/Lose/Pause, pickup/unlock logic, ally management.
- **Content pipeline:** Blender (low-poly + edits), Mixamo (unified rig & shared animations), Unity Particle System for VFX.

---

## 🧱 Architecture (high level)
- `ScriptableObjects/WeaponData` – weapon stats + projectile references  
- `ObjectPoolManager` – pooled spawning/despawning 
- `RoadScroller` – forward world movement via recycled chunks  
- `EraManager` – era management
- `SpawnManager` – enemies/walls/pickups/bosses/allies orchestration  
- `AutoShooter` – player & ally auto-firing  

---

## 📦 Tech Stack
- **Unity (C#)** — gameplay, systems, UI Toolkit/TMP  
- **Blender** — low-poly modeling and edits  
- **Mixamo** — shared armature & cross-compatible animations  
- **Git** — version control  

---

