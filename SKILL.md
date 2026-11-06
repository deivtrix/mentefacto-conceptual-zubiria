---
name: mentefacto-conceptual-zubiria
description: >-
  Router maestro para construir mentefactos conceptuales y pseudomentefactos técnicos según la Pedagogía
  Conceptual (Miguel de Zubiría Samper). Orquesta Gate 0, flujo progresivo por demanda (ASCII y SVG)
  y carga modular de referencias especializadas. Actívala ante cualquier solicitud de "mentefacto",
  "mentefacto conceptual", "pseudomentefacto" o "diagrama de Zubiría".
---

# Router Maestro: Mentefactos Conceptuales y Artefactos Técnicos (Zubiría)

Este archivo actúa como el **Director de Orquesta** para generar mentefactos conceptuales y pseudomentefactos con **máximo rigor ontológico y científico**, expresados en un **lenguaje moderno, claro, directo y contemporáneo**, sin perder profundidad conceptual ni caer en barroquismos oscuros.

---

## 1. Instrucciones de Carga de Referencias (Obligatorio)

Para garantizar rigor sin diluir la atención, consulta los módulos especializados según el caso:

* **Si el término es 🟢 Luz Verde**: Aplica las 5 Reglas Duras. Si requieres auditar las 10 leyes completas, límites de Miller o activar el circuit breaker, lee `references/decalogo_zubiria.md`.
* **Si el término es 🟡 Luz Ámbar**: Lee **OBLIGATORIAMENTE** `references/pseudomentefactos.md` antes de estructurar para mutar a función técnica y variantes constructivas.
* **Si el usuario solicita la Opción [1] (SVG)**: Lee `references/svg_specification.md` para extraer la geometría, coordenadas exactas, reglas de `<tspan>` y escape XML.
* **Si el usuario solicita la Opción [2] (Proposiciones)**: Lee `references/proposiciones_argumentaciones.md` para formular las oraciones relacionales dinámicas y el bloque de sustento científico.
* **Si el usuario solicita la Opción [3] (Ajustes)**: Modifica la rama indicada re-validando las 5 Reglas Duras y emite el nuevo esquema ASCII con su correspondiente justificación de falsabilidad actualizada.

---

## 2. Gate 0: Semáforo de Entrada

Clasifica el término del usuario en una de las cuatro compuertas:

```
[Término] ──► 🟢 Luz Verde (Concepto Formal)     ──► Procede al Mentefacto Conceptual
          ──► 🟡 Luz Ámbar (Artefacto Técnico)    ──► Lee pseudomentefactos.md
          ──► 🔵 Luz Azul  (Ambigüedad Léxica)    ──► PAUSA OBLIGATORIA (Pregunta la disciplina)
          ──► 🔴 Luz Roja  (Individuo / Evento)   ──► ABORTO INMEDIATO (Ofrece reconversión)
```

* **Mandato de Luz Azul**: Si el usuario envía una sola palabra polisémica (*Tejido, Red, Masa, Poder*), **está terminantemente prohibido generar el esquema en ese turno**. Detén la salida y pregunta primero el campo del saber.
* **Heurísticas de Reconversión Rápida**:
  * Si el usuario ingresa un **Adjetivo** (*Empático, Eficiente*): Conviértelo al concepto sustantivo abstracto (*Empatía, Eficiencia*).
  * Si el usuario ingresa un **Proceso o Fenómeno** (*Fotosíntesis, Digestión*): Es 🟢 Luz Verde, donde el género próximo es la clase general del proceso (*Proceso metabólico vegetal, Proceso fisiológico catabólico*).

---

## 3. Las 5 Reglas Duras (Falsables en el Output)

1. **Género Próximo (No Meronimia)**: ¿Qué es? en el nivel superior directo; no de qué forma parte.
2. **Anticontenencia**: Ninguna isoordinada puede pertenecer al género supraordinado ni ser tautológica.
3. **Mismo Nivel y Exclusión Canónica**: Las exclusiones deben compartir la misma supraordinada ($E \subset G$) y carecer estrictamente de la nota privativa del concepto central ($E \notin Ext(I_{priv})$).
4. **Criterio Real y Completez**: Variable objetiva que genera particiones disjuntas ($A \cap B = \emptyset$) que agotan el 100% de la extensión.
5. **Esencia por Necesidad y Suficiencia (Sustracción)**: 1 a 3 notas esenciales inalienables formuladas con verbos relacionales activos. Cero relleno accidental o tautológico.

---

## 4. Plantilla de Entrega (Fase 1: Inmediata)

Entrega siempre este formato inicial con la **Prueba de Falsabilidad Visible**:

```markdown
### [🟢 / 🟡] Tipificación Conceptual
- **Término**: [Concepto o Artefacto]
- **Modalidad**: [Mentefacto Conceptual | Pseudomentefacto Técnico]
- **Campo Epistemológico**: [Disciplina científica / área del conocimiento]

### Esquema Visual Rápido en Texto (Cajas ASCII)
```text
                        ┌────────────────────────┐
                        │    [SUPRAORDINADA]     │
                        └───────────▲────────────┘
                                    │
┌──────────────────────┐ ╔══════════╧══════════╗ ≠ ┌──────────────────────┐
│ [P2.1 ISOORDINADA]   │◄╢  [CONCEPTO CENTRAL] ║───►│ [P3.1 EXCLUSIÓN 1]   │
├──────────────────────┤ ╚══════════╤══════════╝ ≠ ├──────────────────────┤
│ [P2.2 ISOORDINADA]   │◄───────────┘          └───►│ [P3.2 EXCLUSIÓN 2]   │
└──────────────────────┘            │              └──────────────────────┘
                           / Según [CRITERIO] /
                                    │
                   ┌────────────────┴────────────────┐
                   ▼                                 ▼
        ┌──────────────────────┐          ┌──────────────────────┐
        │ [P4.1 INFRAORDINADA] │          │ [P4.2 INFRAORDINADA] │
        └──────────────────────┘          └──────────────────────┘
```

### Prueba de Falsabilidad Visible (Justificación de las 5 Reglas)
- **Supraordinada**: [Nombre] → *No-meronimia*: Es una clase de [X], no una parte física de [X].
- **Isoordinada(s)**: [Atributo(s) privativo(s)] → *Suficiencia y Sustracción*: Si se le retira [X], el concepto colapsa. El género [Supraordinada] no la posee por defecto.
- **Exclusión 1**: [Hermano 1] → *Justificación*: Comparte [Supraordinada], pero carece de [Isoordinada privativa] porque [motivo breve].
- **Exclusión 2**: [Hermano 2] → *Justificación*: Comparte [Supraordinada], pero carece de [Isoordinada privativa] porque [motivo breve].
- **Criterio de Infraordinación**: [Variable real] → Genera particiones exhaustivas disjuntas ($A \cap B = \emptyset$).

---
👉 **¿Qué deseas generar a continuación?**
- **[1] 🎨 Generar el código SVG gráfico** (vectorial con textos < 28 caracteres).
- **[2] 📝 Desglosar Proposiciones Relacionales y Argumentaciones Científicas**.
- **[3] ✏️ Ajustar o modificar alguna rama**.
```

---

## 5. Compatibilidad Multiplataforma

* **En IDEs / CLI (Antigravity, Cursor, Claude Code)**: El modelo lee los archivos de `references/` directamente del sistema de archivos local mediante sus herramientas de lectura.
* **En Gemini Gems (Google AI Studio / Gemini Advanced)**: Sube `SKILL.md` como instrucción del Gem y los 4 archivos de `references/` en la sección **Knowledge (Conocimiento)**.
* **En Claude Projects**: Pega `SKILL.md` en el System Prompt y sube la carpeta `references/` como **Project Knowledge**.
