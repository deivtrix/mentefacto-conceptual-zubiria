# Sistema Experto de Mentefactos Conceptuales (Zubiría Samper)

Sistema modular y router para la generación asistida por IA de **Mentefactos Conceptuales** (Pedagogía Conceptual de Miguel de Zubiría Samper) y **Pseudomentefactos Técnicos** para ingeniería, ciencias y tecnología.

Diseñado bajo la arquitectura **Divide y Vencerás (Lazy Loading)** para erradicar la saturación atencional (*instruction dilution*) en Modelos de Lenguaje Grande (LLMs) y garantizar el cumplimiento estricto de las leyes lógicas del pensamiento formal.

---

## 🏛️ Arquitectura del Sistema

El proyecto separa el enrutamiento inmediato del conocimiento especializado:

```
MENTEFACTOS_IA/
├── SKILL.md                                 # Router maestro (< 110 líneas: Gate 0 + 5 Reglas Duras)
├── README.md                                # Guía de implementación y arquitectura
└── references/
    ├── decalogo_zubiria.md                  # Fundamentación teórica, 10 leyes canónicas y lectura en cruz
    ├── pseudomentefactos.md                 # Metodología de mutación funcional para artefactos técnicos
    ├── proposiciones_argumentaciones.md     # Modelo proposicional dinámico y argumentación científica
    └── svg_specification.md                 # Especificación geométrica SVG canónica (viewBox 850x560)
```

---

## 🚦 Gate 0: Semáforo Ontológico de Entrada

Antes de generar cualquier diagrama, el sistema clasifica el término:

* 🟢 **Luz Verde (Concepto Formal)**: Entidad abstracta, clase natural o científica (*Célula, Democracia, Algoritmo, Gravedad*). Genera Mentefacto Conceptual.
* 🟡 **Luz Ámbar (Artefacto Técnico)**: Objeto físico manufacturado, instrumento o dispositivo (*Osciloscopio, Microcontrolador, Motor*). Consulta `references/pseudomentefactos.md` y muta a función técnica y principios operativos.
* 🔵 **Luz Azul (Ambigüedad Semántica)**: Palabras polisémicas ingresadas solas (*Red, Tejido, Campo, Masa*). **Pausa obligatoria**: pregunta primero la disciplina científica.
* 🔴 **Luz Roja (Individuo o Evento Histórico)**: Nombres propios, especímenes singulares o hitos cronológicos. Detiene la generación y sugiere la clase universal correspondiente.

---

## ⚖️ Las 5 Reglas Duras (Falsables en el Output)

1. **Género Próximo (Anti-Meronimia)**: Clase inclusiva directa (*¿Qué es?*), jamás relación parte-todo (*¿De qué forma parte?*).
2. **Anticontenencia**: Ninguna isoordinada puede pertenecer al género supraordinado ni ser tautológica.
3. **Mismo Nivel y Exclusión Canónica**: Las exclusiones pertenecen a la misma supraordinada ($E \subset G$) y carecen de la nota privativa del concepto ($E \notin Ext(I_{priv})$).
4. **Criterio Real y Completez**: Variable medible/observable que genera particiones mutuamente excluyentes ($A \cap B = \emptyset$) que agotan el 100%.
5. **Esencia por Necesidad y Suficiencia**: De 1 a 3 notas esenciales formuladas con verbos relacionales activos. Cero relleno accidental.

---

## 🚀 Despliegue en Plataformas

### 1. Google Gemini Gems (Gemini Advanced / AI Studio)
1. Crea un nuevo **Gem**.
2. Copia y pega el contenido íntegro de `SKILL.md` en el recuadro de **Instrucciones**.
3. En la sección **Conocimiento (Knowledge)**, sube los 4 archivos de la carpeta `references/`:
   - `decalogo_zubiria.md`
   - `pseudomentefactos.md`
   - `proposiciones_argumentaciones.md`
   - `svg_specification.md`
4. Guarda el Gem.

### 2. Claude Projects (Anthropic)
1. Crea un nuevo **Project**.
2. Pega `SKILL.md` en las **Project Instructions**.
3. Sube la carpeta `references/` a los **Project Files**.

### 3. IDEs y Asistentes CLI (Antigravity CLI, Cursor, Claude Code)
* Coloca la carpeta en el espacio de trabajo. El agente leerá `SKILL.md` como skill nativa y cargará los archivos de `references/` mediante herramientas de lectura de disco bajo demanda.

---

## 📝 Flujo de Generación Progresiva

* **Fase 1 (Inmediata)**: Tipificación epistemológica, esquema visual monoespaciado en cajas ASCII y bloque de **Prueba de Falsabilidad Visible**.
* **Fase 2 (Bajo Demanda)**: Menú interactivo para generar:
  * `[1]` Código vectorial SVG profesional listo para insertar en web o documentos.
  * `[2]` Paquete proposicional relacional y argumentación científica.
  * `[3]` Ajuste asistido de cualquier rama del diagrama.
