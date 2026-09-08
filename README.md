# Registro Multimedia de Equipo

Aplicación Android desarrollada en **Java** para la actividad práctica de aula.
Equipo de **23 integrantes**.

> Este README lo completa **P23**. La plantilla completa está en la guía `Guia_Registro_Multimedia_23_integrantes.docx` (en la raíz de este repositorio).

---

## Cómo entregar tu parte (todos)

Cada integrante sube su archivo **únicamente a la carpeta de su número**.

1. Abre la carpeta `entregas/` y entra a la carpeta de tu número (por ejemplo `entregas/P07`).
2. Arriba a la derecha: **Add file → Upload files**.
3. Arrastra tu archivo al recuadro.
4. Abajo, en **Commit changes**, escribe qué subiste. Ejemplo: `P07 bloque RatingBar y ProgressBar`.
5. Botón verde **Commit changes**. Listo.

Para comprobar que quedó: entra a tu carpeta, tu archivo debe aparecer con **tu usuario** y la hora al lado.

## Las 3 reglas que no se rompen

1. Subes **solo a tu carpeta**. Nunca a la de otro, nunca a `app_final/`.
2. Cada archivo tiene **un solo dueño**: `MainActivity.java` es de **P6**, `activity_main.xml` de **P16**, `GrabadorAudio.java` de **P1** e `IntegranteAdapter.java` de **P10**. Si tu tarea es un método suelto, lo entregas en un `.txt` a **P7**.
3. Nunca cambies los nombres de los `id` del XML (`checkJava`, `ratingBar`, `recyclerIntegrantes`...). El código de tus compañeros depende de ellos.

## Estructura del repositorio

```
registro-multimedia-equipo/
├── entregas/        <- cada uno sube aquí, en su propia carpeta
│   ├── P01/ ... P23/
├── app_final/       <- SOLO P6: la app terminada en ZIP
├── capturas/        <- SOLO P22: capturas y evidencias
└── README.md
```

## Quién hace qué

Los grupos están **ordenados por dificultad**: mientras más bajo el número, más pesada la tarea.
Los números bajos (P1–P11) son para quienes más manejan Java; los altos (P19–P23) son los más livianos.

| Grupo | Dificultad | Personas |
|---|---|---|
| G1 · Audio (P1–P5) | 5 de 5 | 5 |
| G2 · Integración (P6–P7) | 5 de 5 | 2 |
| G3 · Lista / RecyclerView (P8–P11) | 4 de 5 | 4 |
| G4 · Valoración y progreso (P12–P14) | 3 de 5 | 3 |
| G5 · Estructura base (P15–P16) | 2 de 5 | 2 |
| G6 · Controles de selección (P17–P18) | 2 de 5 | 2 |
| G7 · Lógica adicional (P19–P20) | 2 de 5 | 2 |
| G8 · Calidad y cierre (P21–P23) | 1 de 5 | 3 |

| N° | Nombre | Dif. | Grupo | Tarea | Archivo del que es dueño |
|---|---|---|---|---|---|
| P01 | | 5/5 | G1 · Audio | Grabación de audio (dueño del archivo) | `GrabadorAudio.java` |
| P02 | | 5/5 | G1 · Audio | Reproducción y liberación de recursos | `Métodos Java (se pegan en GrabadorAudio.java)` |
| P03 | | 5/5 | G1 · Audio | Permiso del micrófono en tiempo de ejecución | `Métodos Java (se pegan en MainActivity)` |
| P04 | | 5/5 | G1 · Audio | Botones de audio y su lógica | `Bloque XML + método Java` |
| P05 | | 5/5 | G1 · Audio | Pruebas de audio en dispositivo | `Informe de pruebas de audio` |
| P06 | | 5/5 | G2 · Integración | Integrador (arma la app) | `MainActivity.java` |
| P07 | | 5/5 | G2 · Integración | Copiloto de integración | `Checklist de métodos recibidos` |
| P08 | | 4/5 | G3 · Lista dinámica (RecyclerView) | Modelo de datos | `Integrante.java` |
| P09 | | 4/5 | G3 · Lista dinámica (RecyclerView) | Tarjeta del listado (CardView) | `item_integrante.xml + bloque RecyclerView` |
| P10 | | 4/5 | G3 · Lista dinámica (RecyclerView) | Adapter (dueño del archivo) | `IntegranteAdapter.java` |
| P11 | | 4/5 | G3 · Lista dinámica (RecyclerView) | ViewHolder y crecimiento de la lista | `Clase interna + método (se pegan en IntegranteAdapter.java)` |
| P12 | | 3/5 | G4 · Valoración y progreso | RatingBar y ProgressBar (XML) | `Bloque XML para activity_main.xml` |
| P13 | | 3/5 | G4 · Valoración y progreso | Cálculo del avance | `Método Java (se pega en MainActivity)` |
| P14 | | 3/5 | G4 · Valoración y progreso | Listeners que disparan el avance | `Método Java (se pega en MainActivity)` |
| P15 | | 2/5 | G5 · Estructura base | Creación del proyecto y dependencias | `Proyecto base + build.gradle.kts` |
| P16 | | 2/5 | G5 · Estructura base | Permiso, esqueleto de pantalla y armado del XML | `AndroidManifest.xml + activity_main.xml` |
| P17 | | 2/5 | G6 · Controles de selección | CheckBox, RadioButton y Spinner (XML) | `Bloque XML + res/values/strings.xml` |
| P18 | | 2/5 | G6 · Controles de selección | Lógica Java de los controles | `Métodos Java (se pegan en MainActivity)` |
| P19 | | 2/5 | G7 · Lógica adicional | Validación del formulario | `Método Java (se pega en MainActivity)` |
| P20 | | 2/5 | G7 · Lógica adicional | Resumen estadístico del equipo | `Método Java (se pega en MainActivity)` |
| P21 | | 1/5 | G8 · Calidad y cierre | Tester / control de calidad | `Informe de pruebas` |
| P22 | | 1/5 | G8 · Calidad y cierre | Evidencias y exposición | `Carpeta de evidencias` |
| P23 | | 1/5 | G8 · Calidad y cierre | Administrador del repositorio, README y diseño visual | `Repositorio de GitHub + colors.xml + README.md` |

## La aplicación

Permite registrar integrantes de un equipo, seleccionar sus tecnologías y jornada,
evaluarlos con estrellas, verlos en una lista de tarjetas y grabar una presentación
de voz en formato M4A.

| Componente | Dónde se usa |
|---|---|
| CheckBox | Tecnologías que maneja el integrante |
| RadioGroup / RadioButton | Selección de jornada |
| Spinner | Lista de carreras |
| RatingBar | Calificación de 1 a 5 estrellas |
| ProgressBar | Avance del formulario (0 % a 100 %) |
| ImageView | Avatar del integrante |
| ScrollView | Desplazamiento de la pantalla |
| RecyclerView + CardView | Lista dinámica de integrantes |
| MediaRecorder / MediaPlayer | Grabación y reproducción de audio |

**Proyecto:** `RegistroMultimedia` · **Paquete:** `com.example.registromultimedia` · **minSdk:** 24 · **Lenguaje:** Java
