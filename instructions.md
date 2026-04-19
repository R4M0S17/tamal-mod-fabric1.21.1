# 🗺️ Roadmap: Zipacná Boss Mod (Fabric 1.21.1)
**Project Name:** Tamal Mod
**Target Version:** Minecraft 1.21.1
**Library:** GeckoLib 4+
**Hardware Target:** Apple M1 (8GB RAM) - Focus on Optimization.

---

## 🟢 FASE 1: Configuración y Assets (Preparación)
- [ ] Configurar entorno de desarrollo (JDK 21, Gradle, IntelliJ/VS Code).
- [ ] Inicializar proyecto Fabric 1.21.1.
- [ ] **Blockbench:** Crear el modelo de Zipacná (basado en el Model Sheet).
- [ ] **Blockbench:** Crear el modelo del Buitre Maya (basado en el Phantom).
- [ ] Exportar modelos `.geo.json`, animaciones `.animation.json` y texturas.

## 🟡 FASE 2: Cimientos de Entidades (Java)
- [ ] Registrar la entidad de `ZipacnaEntity`.
- [ ] Registrar la entidad de `MayanVultureEntity` (heredando de Phantom).
- [ ] Configurar **GeckoLib** en el proyecto (Client-side rendering).
- [ ] Implementar animaciones básicas: `idle`, `walk`, `attack`.

## 🟠 FASE 3: Mecánicas del Jefe y IA de Súbditos
- [ ] **IA Buitre:** Adaptar la lógica de vuelo del Phantom para que sea terrestre/vuelo bajo.
- [ ] **Zipacná Hitboxes:** Implementar sistema de hitboxes múltiples (Cabeza = Crítico, Patas = Tanque).
- [ ] **Ataque 1:** Rugido Sónico (Empuje y partículas).
- [ ] **Ataque 2:** Erupción de picos de obsidiana (Generación de bloques/entidades temporales).

## 🔴 FASE 4: Lógica de la Batalla y Fases
- [ ] Implementar la Boss Bar personalizada.
- [ ] Lógica de fases: Spawn de buitres al 75%, 50% y 25% de vida.
- [ ] Mecánica de "Aturdimiento": Si recibe X daño en las patas, baja la cabeza 5 segundos.
- [ ] Implementar loot especial: "Corazón de la Tierra" (Jade).

## 🟣 FASE 5: Optimización y Pulido (M1 Focus)
- [ ] Revisar `MSPT` (Milliseconds Per Tick) para evitar lag.
- [ ] Optimizar partículas (enviar solo al cliente cercano).
- [ ] Limpieza de memoria (revisar que las entidades temporales desaparezcan).
- [ ] Beta test en el servidor de Tamaland.