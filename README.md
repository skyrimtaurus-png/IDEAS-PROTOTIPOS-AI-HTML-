# Corpus de Conocimiento Estructurado en Español para IA

Colección curada y organizada de **48 corpus y ontologías en español** (~3.74 MB en total), diseñada para entrenamiento de modelos de lenguaje ligeros, sistemas neuro-simbólicos, recuperación semántica (RAG), grafos de conocimiento y razonamiento causal.

---

## Resumen General

| Bloque | Carpeta | Archivos | Contenido principal | Formatos |
| :--- | :--- | :---: | :--- | :--- |
| **01. Corpus Temáticos** | [`01_corpus_tematicos/`](01_corpus_tematicos/) | 31 | Fundamentos multidisciplinares, dinámica de sistemas complejos y catálogos funcionales (6,639 entradas) | `.txt`, `.jsonl` |
| **02. Enciclopedia Temática** | [`02_enciclopedia_tematica/`](02_enciclopedia_tematica/) | 8 | 8 tomos enciclopédicos desde cosmología hasta ingeniería e inventos (324 entradas) | `.txt` |
| **03. Conocimiento Ontológico** | [`03_conocimiento_ontologico/`](03_conocimiento_ontologico/) | 9 | Ontología físico-causal (625 nodos raíz y 1,536 relaciones), currículo de primaria (108 relaciones) y operadores relacionales/dinámicos | `.json`, `.csv`, `.md` |

---

## Estructura del Repositorio

```text
.
├── README.md
├── 01_corpus_tematicos/
│   ├── fundamentos/             # 01–20: diálogo, lógica, gramática, ciencias, código, circuitos y grafos
│   ├── sistemas_y_procesos/     # 21–26: procesos causales en finanzas, fluidos, fisiología, química, software y logística
│   └── catalogos_funcionales/   # 27–31: catálogos funcionales de entidades, componentes y mecanismos por dominio
├── 02_enciclopedia_tematica/    # 8 tomos enciclopédicos estructurados por áreas del saber
└── 03_conocimiento_ontologico/
    ├── causal_fisico/           # Grafo atómico físico-causal (JSON/CSV), diccionario canónico y compendio
    ├── curricular_primaria/     # Ontología pedagógica 1.º–5.º de Primaria (JSON/CSV) y workflow curricular
    └── operadores_semantica/    # Díadas relacionales monosémicas y modificadores dinámicos de segundo orden
```

---

## 01. Corpus Temáticos ([`01_corpus_tematicos/`](01_corpus_tematicos/))

### 1.1 Fundamentos y Ciencias ([`fundamentos/`](01_corpus_tematicos/fundamentos/))

Veinte corpus base que cubren lenguaje, razonamiento, ciencias exactas y naturales, cultura general, programación e ingeniería.

| # | Archivo | Descripción | Formato | Entradas |
| :-: | :--- | :--- | :---: | :---: |
| 01 | [`01_Identidad_Dialogo_y_Prudencia.txt`](01_corpus_tematicos/fundamentos/01_Identidad_Dialogo_y_Prudencia.txt) | Diálogo pragmático, honestidad epistémica, método científico, falacias y resolución de elipsis | `.txt` (`\|` y declarativo) | 29 |
| 02 | [`02_Sinonimos_Antonimos_y_Logica.txt`](01_corpus_tematicos/fundamentos/02_Sinonimos_Antonimos_y_Logica.txt) | Sinónimos, antónimos directos, oposiciones conceptuales y relaciones lógicas | `.txt` (`:` y declarativo) | 1,527 |
| 03 | [`03_Gramatica_Sintaxis_y_Espanol.txt`](01_corpus_tematicos/fundamentos/03_Gramatica_Sintaxis_y_Espanol.txt) | Gramática española, categorías gramaticales, sintaxis y concordancia | `.txt` (`\|` y declarativo) | 477 |
| 04 | [`04_Matematicas_Aritmetica_y_Algebra.txt`](01_corpus_tematicos/fundamentos/04_Matematicas_Aritmetica_y_Algebra.txt) | Aritmética, lógica numérica, secuencias y fundamentos de álgebra | `.txt` (`\|` y declarativo) | 492 |
| 05 | [`05_Ciencias_Fisica_Quimica_y_Meteorologia.txt`](01_corpus_tematicos/fundamentos/05_Ciencias_Fisica_Quimica_y_Meteorologia.txt) | Física básica, química, astronomía y meteorología en estilo sujeto-verbo-objeto | `.txt` | 116 |
| 06 | [`06_Biologia_Anatomia_y_Salud.txt`](01_corpus_tematicos/fundamentos/06_Biologia_Anatomia_y_Salud.txt) | Biología celular, células madre, genética básica y anatomía humana | `.txt` | 128 |
| 07 | [`07_Programacion_HTML_Web_e_Ingenieria.jsonl`](01_corpus_tematicos/fundamentos/07_Programacion_HTML_Web_e_Ingenieria.jsonl) | Preguntas y respuestas de programación, desarrollo web (HTML/CSS/JS) e ingeniería de software (`q`, `a`, `lang`, `intent_key`, `axiom_preview`) | `.jsonl` | 186 |
| 08 | [`08_Geografia_Historia_y_Cultura_General.txt`](01_corpus_tematicos/fundamentos/08_Geografia_Historia_y_Cultura_General.txt) | Geografía física y política, historia básica, sociedad y cultura general | `.txt` (`\|` y declarativo) | 116 |
| 09 | [`09_Causalidad_Cotidiana_y_Sentido_Comun.txt`](01_corpus_tematicos/fundamentos/09_Causalidad_Cotidiana_y_Sentido_Comun.txt) | Axiomas de causalidad física cotidiana, propiedades de materiales y contrafactuales | `.txt` | 44 |
| 10 | [`10_Musica_Armonia_y_Workflows.txt`](01_corpus_tematicos/fundamentos/10_Musica_Armonia_y_Workflows.txt) | Teoría musical, acordes, escalas, notación ABC y arquitectura de workflows | `.txt` | 27 |
| 11 | [`11_Quimica_General_Organica_e_Inorganica.txt`](01_corpus_tematicos/fundamentos/11_Quimica_General_Organica_e_Inorganica.txt) | Estructura atómica, química inorgánica, química orgánica y estequiometría | `.txt` | 102 |
| 12 | [`12_Fisica_Avanzada_Electromagnetismo_y_Optica.txt`](01_corpus_tematicos/fundamentos/12_Fisica_Avanzada_Electromagnetismo_y_Optica.txt) | Cinemática y dinámica vectorial, electromagnetismo, ondas, óptica y física moderna | `.txt` | 76 |
| 13 | [`13_Matematicas_Avanzadas_Estadistica_y_Calculo.txt`](01_corpus_tematicos/fundamentos/13_Matematicas_Avanzadas_Estadistica_y_Calculo.txt) | Metrología (SI), cálculo, álgebra lineal, probabilidad y estadística | `.txt` | 78 |
| 14 | [`14_Biologia_Avanzada_Genetica_y_Medicina.txt`](01_corpus_tematicos/fundamentos/14_Biologia_Avanzada_Genetica_y_Medicina.txt) | Neurobiología, fisiología humana avanzada, genética molecular y medicina de urgencias | `.txt` | 65 |
| 15 | [`15_Geografia_Mundial_Politica_y_Fisica.txt`](01_corpus_tematicos/fundamentos/15_Geografia_Mundial_Politica_y_Fisica.txt) | Países, capitales, orografía, hidrografía y climatología mundial | `.txt` | 33 |
| 16 | [`16_Historia_Universal_y_Pensamiento_Humano.txt`](01_corpus_tematicos/fundamentos/16_Historia_Universal_y_Pensamiento_Humano.txt) | Historia universal desde la Antigüedad, filosofía, pensamiento ético y economía | `.txt` | 41 |
| 17 | [`17_Ingenieria_de_Software_Redes_y_Ciberseguridad.jsonl`](01_corpus_tematicos/fundamentos/17_Ingenieria_de_Software_Redes_y_Ciberseguridad.jsonl) | Preguntas y respuestas de redes (OSI/TCP-IP), arquitectura de software y ciberseguridad (`q`, `a`) | `.jsonl` | 21 |
| 18 | [`18_Sentido_Comun_Practico_y_Resolucion_de_Problemas.txt`](01_corpus_tematicos/fundamentos/18_Sentido_Comun_Practico_y_Resolucion_de_Problemas.txt) | Sentido común práctico, metrología cotidiana y resolución de problemas diarios | `.txt` | 25 |
| 19 | [`19_Teoria_de_Circuitos_Redes_Flujos_y_Kirchhoff.txt`](01_corpus_tematicos/fundamentos/19_Teoria_de_Circuitos_Redes_Flujos_y_Kirchhoff.txt) | Topología de circuitos, leyes de Kirchhoff y redes de flujo | `.txt` | 32 |
| 20 | [`20_Procesos_Estocasticos_Grafos_y_Fisica_Estadistica.txt`](01_corpus_tematicos/fundamentos/20_Procesos_Estocasticos_Grafos_y_Fisica_Estadistica.txt) | Dualidad redes eléctricas–cadenas de Markov, grafos laplacianos y física estadística | `.txt` | 32 |

### 1.2 Sistemas Complejos y Procesos Especializados ([`sistemas_y_procesos/`](01_corpus_tematicos/sistemas_y_procesos/))

Seis corpus de alta densidad técnica (1,646 proposiciones) redactados con estructura causal uniforme: **entidad + acción + condición (`ante`) + mecanismo (`mediante`) + resultado (`para` / efecto)**.

| # | Archivo | Dominio | Proposiciones |
| :-: | :--- | :--- | :---: |
| 21 | [`21_Economia_Finanzas_Banca_Tesoreria_y_Riesgo.txt`](01_corpus_tematicos/sistemas_y_procesos/21_Economia_Finanzas_Banca_Tesoreria_y_Riesgo.txt) | Liquidez, solvencia, banca, tesorería, amortización y gestión de riesgo | 280 |
| 22 | [`22_Mecanica_Fluidos_Termodinamica_Motores_y_Electronica_Potencia.txt`](01_corpus_tematicos/sistemas_y_procesos/22_Mecanica_Fluidos_Termodinamica_Motores_y_Electronica_Potencia.txt) | Mecánica de fluidos, válvulas, termodinámica, motores y electrónica de potencia | 275 |
| 23 | [`23_Fisiologia_Celular_Bioquimica_Inmunologia_y_Patologia.txt`](01_corpus_tematicos/sistemas_y_procesos/23_Fisiologia_Celular_Bioquimica_Inmunologia_y_Patologia.txt) | Homeostasis, fisiología celular, bioquímica, inmunología y patología | 265 |
| 24 | [`24_Fisicoquimica_Transferencia_Materiales_y_Procesos_Quimicos.txt`](01_corpus_tematicos/sistemas_y_procesos/24_Fisicoquimica_Transferencia_Materiales_y_Procesos_Quimicos.txt) | Adsorción, transferencia de masa/calor, ciencia de materiales y procesos químicos | 275 |
| 25 | [`25_Sistemas_Distribuidos_Concurrencia_Almacenamiento_y_Resiliencia.txt`](01_corpus_tematicos/sistemas_y_procesos/25_Sistemas_Distribuidos_Concurrencia_Almacenamiento_y_Resiliencia.txt) | Circuit breakers, concurrencia, tolerancia a fallos, almacenamiento y resiliencia | 276 |
| 26 | [`26_Logistica_Redes_Ecologia_y_Regulacion_Sistemas_Complejos.txt`](01_corpus_tematicos/sistemas_y_procesos/26_Logistica_Redes_Ecologia_y_Regulacion_Sistemas_Complejos.txt) | Cuellos de botella, logística, redes, ecología y regulación de sistemas complejos | 275 |

### 1.3 Catálogos Funcionales por Dominio ([`catalogos_funcionales/`](01_corpus_tematicos/catalogos_funcionales/))

Cinco catálogos técnicos (1,346 fichas) que describen **qué hace cada componente o entidad**, bajo qué condición opera, mediante qué mecanismo y con qué efecto.

| # | Archivo | Dominio del catálogo | Fichas |
| :-: | :--- | :--- | :---: |
| 27 | [`27_Catalogo_Funcional_Instrumentos_Contratos_y_Figuras_Financieras.txt`](01_corpus_tematicos/catalogos_funcionales/27_Catalogo_Funcional_Instrumentos_Contratos_y_Figuras_Financieras.txt) | Instrumentos financieros, contratos y figuras corporativas | 268 |
| 28 | [`28_Catalogo_Funcional_Componentes_Maquinas_Hidraulica_y_Potencia.txt`](01_corpus_tematicos/catalogos_funcionales/28_Catalogo_Funcional_Componentes_Maquinas_Hidraulica_y_Potencia.txt) | Componentes eléctricos, maquinaria, hidráulica y sistemas de potencia | 270 |
| 29 | [`29_Catalogo_Funcional_Tejidos_Receptores_Organelos_y_Fisiologia.txt`](01_corpus_tematicos/catalogos_funcionales/29_Catalogo_Funcional_Tejidos_Receptores_Organelos_y_Fisiologia.txt) | Tejidos biológicos, receptores sensoriales, organelos y procesos fisiológicos | 270 |
| 30 | [`30_Catalogo_Funcional_Aparatos_Laboratorio_Materiales_y_Fenomenos.txt`](01_corpus_tematicos/catalogos_funcionales/30_Catalogo_Funcional_Aparatos_Laboratorio_Materiales_y_Fenomenos.txt) | Instrumentos de laboratorio, materiales y fenómenos físico-químicos | 270 |
| 31 | [`31_Catalogo_Funcional_Arquitectura_Hardware_Redes_y_Estructuras_Datos.txt`](01_corpus_tematicos/catalogos_funcionales/31_Catalogo_Funcional_Arquitectura_Hardware_Redes_y_Estructuras_Datos.txt) | Arquitectura de hardware, protocolos de red y estructuras de datos | 268 |

---

## 02. Enciclopedia Temática ([`02_enciclopedia_tematica/`](02_enciclopedia_tematica/))

Ocho tomos enciclopédicos concisos en formato `Concepto : Definición técnica` organizados por secciones (324 entradas totales).

| Tomo | Archivo | Áreas cubiertas | Entradas |
| :-: | :--- | :--- | :---: |
| 01 | [`ENCARTA_TOMO_01_Cosmos_Tierra_y_Geologia.txt`](02_enciclopedia_tematica/ENCARTA_TOMO_01_Cosmos_Tierra_y_Geologia.txt) | Cosmología, astrofísica, Sistema Solar, geofísica y meteorología | 59 |
| 02 | [`ENCARTA_TOMO_02_Materia_Elementos_y_Quimica_Industrial.txt`](02_enciclopedia_tematica/ENCARTA_TOMO_02_Materia_Elementos_y_Quimica_Industrial.txt) | Monografías de elementos químicos, materia y procesos industriales | 31 |
| 03 | [`ENCARTA_TOMO_03_Reino_Animal_Vegetal_y_Evolucion.txt`](02_enciclopedia_tematica/ENCARTA_TOMO_03_Reino_Animal_Vegetal_y_Evolucion.txt) | Taxonomía biológica, reinos animal/vegetal, ecología y evolución | 74 |
| 04 | [`ENCARTA_TOMO_04_Cuerpo_Humano_Fisiologia_y_Medicina.txt`](02_enciclopedia_tematica/ENCARTA_TOMO_04_Cuerpo_Humano_Fisiologia_y_Medicina.txt) | Sistemas del cuerpo humano, fisiología y medicina clínica | 41 |
| 05 | [`ENCARTA_TOMO_05_Geografia_Universal_Paises_y_Orografia.txt`](02_enciclopedia_tematica/ENCARTA_TOMO_05_Geografia_Universal_Paises_y_Orografia.txt) | Atlas político, países, orografía e hidrografía mundial | 40 |
| 06 | [`ENCARTA_TOMO_06_Historia_Universal_Edades_e_Hitos.txt`](02_enciclopedia_tematica/ENCARTA_TOMO_06_Historia_Universal_Edades_e_Hitos.txt) | Prehistoria, civilizaciones antiguas, edades históricas e hitos globales | 26 |
| 07 | [`ENCARTA_TOMO_07_Filosofia_Leyes_Economia_y_Sociedad.txt`](02_enciclopedia_tematica/ENCARTA_TOMO_07_Filosofia_Leyes_Economia_y_Sociedad.txt) | Epistemología, metafísica, ética, derecho, economía y sociedad | 30 |
| 08 | [`ENCARTA_TOMO_08_Tecnologia_Ingenieria_e_Inventos.txt`](02_enciclopedia_tematica/ENCARTA_TOMO_08_Tecnologia_Ingenieria_e_Inventos.txt) | Hitos tecnológicos, ingeniería, energía e inventos clave | 23 |

---

## 03. Conocimiento Ontológico ([`03_conocimiento_ontologico/`](03_conocimiento_ontologico/))

Representaciones formales y estructuradas para grafos de conocimiento, razonamiento causal y extracción semántica.

### 3.1 Ontología Físico-Causal ([`causal_fisico/`](03_conocimiento_ontologico/causal_fisico/))
- [`conocimiento_ontologico_causal.json`](03_conocimiento_ontologico/causal_fisico/conocimiento_ontologico_causal.json) — Compendio estructurado (v3.0) con **625 nodos atómicos raíz** (`nodos_atomicos_raiz`) y **1,536 relaciones físico-causales** con sujeto base, condición, relación, objeto, consecuencia, representación formal y nodos vinculados.
- [`conocimiento_ontologico_causal.csv`](03_conocimiento_ontologico/causal_fisico/conocimiento_ontologico_causal.csv) — Versión tabular equivalente de las 1,536 relaciones causales.
- [`DICCIONARIO_ONTOLOGICO_ATOMICO.md`](03_conocimiento_ontologico/causal_fisico/DICCIONARIO_ONTOLOGICO_ATOMICO.md) — Vocabulario canónico de nodos raíz atómicos (*Head Entities*) de sentido común para indexación de grafos.
- [`LIBRO_DE_CONOCIMIENTO_ONTOLOGICO_Y_FISICO.md`](03_conocimiento_ontologico/causal_fisico/LIBRO_DE_CONOCIMIENTO_ONTOLOGICO_Y_FISICO.md) — Manifiesto de arquitectura atómica, correcciones semánticas e índice temático.

### 3.2 Ontología Curricular de Primaria ([`curricular_primaria/`](03_conocimiento_ontologico/curricular_primaria/))
- [`ontologia_curricular_primaria.json`](03_conocimiento_ontologico/curricular_primaria/ontologia_curricular_primaria.json) — **108 relaciones pedagógicas** estructuradas de **1.º a 5.º de Primaria** en 5 materias (*Español, Matemáticas, Ciencias Naturales, Ciencias Sociales e Inglés*).
- [`ontologia_curricular_primaria.csv`](03_conocimiento_ontologico/curricular_primaria/ontologia_curricular_primaria.csv) — Versión tabular equivalente de las 108 relaciones curriculares.
- [`WORKFLOW_CURRICULAR_PRIMARIA.md`](03_conocimiento_ontologico/curricular_primaria/WORKFLOW_CURRICULAR_PRIMARIA.md) — Pipeline pedagógico progresivo en espiral y matriz completa por grado y materia.

### 3.3 Operadores Semánticos y Modificadores ([`operadores_semantica/`](03_conocimiento_ontologico/operadores_semantica/))
- [`ejes_relacionales_p8.json`](03_conocimiento_ontologico/operadores_semantica/ejes_relacionales_p8.json) — Ontología declarativa monosémica con **14 díadas relacionales** (28 operadores topológicos, cuantitativos y de fase) y **7 pares macro bipolares** con prefijos y léxico auditado.
- [`modificadores_segundo_orden.json`](03_conocimiento_ontologico/operadores_semantica/modificadores_segundo_orden.json) — Ontología declarativa monosémica con **8 díadas de modificadores dinámicos de segundo orden** (reversibilidad, cinemática temporal agudo vs. crónico, etc.).

---

## Formatos y Ejemplo Rápido de Carga en Python

Los archivos utilizan codificación **UTF-8** y convenciones limpias fáciles de parsear:
- **`.txt`**: líneas con `#` indican títulos o secciones; según el corpus, las líneas de datos son oraciones declarativas, pares `Pregunta | Respuesta` o definiciones `Concepto : Definición`.
- **`.jsonl`**: un objeto JSON por línea con campos `q` (pregunta) y `a` (respuesta), más metadatos opcionales en el archivo `07`.
- **`.json` / `.csv`**: esquemas directos listos para `json.load`, `csv.DictReader` o `pandas`.

```python
import csv
import json
from pathlib import Path

# 1. Leer cualquier corpus .txt ignorando comentarios y líneas vacías
def cargar_txt(ruta: str) -> list[str]:
    return [
        linea.strip()
        for linea in Path(ruta).read_text(encoding="utf-8").splitlines()
        if linea.strip() and not linea.strip().startswith("#")
    ]

# 2. Leer corpus .jsonl (ej. programación o redes)
def cargar_jsonl(ruta: str) -> list[dict]:
    with open(ruta, encoding="utf-8") as f:
        return [json.loads(linea) for linea in f if linea.strip()]

# 3. Leer ontología físico-causal en JSON o CSV
ontologia = json.loads(
    Path("03_conocimiento_ontologico/causal_fisico/conocimiento_ontologico_causal.json")
    .read_text(encoding="utf-8")
)
print(f"Nodos raíz: {len(ontologia['nodos_atomicos_raiz'])} | Relaciones: {len(ontologia['relaciones'])}")

with open("03_conocimiento_ontologico/curricular_primaria/ontologia_curricular_primaria.csv", encoding="utf-8-sig") as f:
    primaria = list(csv.DictReader(f))
print(f"Relaciones curriculares de primaria: {len(primaria)}")
```
