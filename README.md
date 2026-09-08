# Registro Multimedia de Equipo

Aplicación Android desarrollada en **Java** para la actividad práctica de aula.
Equipo de **23 integrantes**.

> Este README lo completa **P22**. La plantilla completa está en la guía `Guia_Registro_Multimedia_23_integrantes.docx` (en la raíz de este repositorio).

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
2. Solo **P19** escribe en `MainActivity.java`. Solo **P3** escribe en `activity_main.xml`. Los demás entregan su parte en un archivo de texto.
3. Nunca cambies los nombres de los `id` del XML (`checkJava`, `ratingBar`, `recyclerIntegrantes`...). El código de tus compañeros depende de ellos.

## Estructura del repositorio

```
registro-multimedia-equipo/
├── entregas/        <- cada uno sube aquí, en su propia carpeta
│   ├── P01/ ... P23/
├── app_final/       <- SOLO P19: la app terminada en ZIP
├── capturas/        <- SOLO P21: capturas y evidencias
└── README.md
```

## Quién hace qué

| N° | Nombre | Equipo | Tarea | Archivo del que es dueño |
|---|---|---|---|---|
| P01 | | Estructura base | Creador del proyecto | `Proyecto completo (base inicial)` |
| P02 | | Estructura base | Dependencias del proyecto | `build.gradle.kts (Module :app)` |
| P03 | | Estructura base | Permiso y esqueleto de pantalla | `AndroidManifest.xml + activity_main.xml` |
| P04 | | Controles de selección | CheckBox y RadioButton (XML) | `Bloque XML para activity_main.xml` |
| P05 | | Controles de selección | Spinner y lista de carreras | `Bloque XML + res/values/strings.xml` |
| P06 | | Controles de selección | Lógica Java de los controles | `Métodos Java (se pegan en MainActivity)` |
| P07 | | Valoración y progreso | RatingBar y ProgressBar (XML) | `Bloque XML para activity_main.xml` |
| P08 | | Valoración y progreso | Cálculo del avance | `Método Java (se pega en MainActivity)` |
| P09 | | Valoración y progreso | Listeners que disparan el avance | `Método Java (se pega en MainActivity)` |
| P10 | | Lista dinámica | Modelo de datos | `Integrante.java` |
| P11 | | Lista dinámica | Tarjeta del listado | `item_integrante.xml + bloque RecyclerView` |
| P12 | | Lista dinámica | Adapter y ViewHolder | `IntegranteAdapter.java` |
| P13 | | Audio | Clase de grabación | `GrabadorAudio.java` |
| P14 | | Audio | Permiso en tiempo de ejecución | `Métodos Java (se pegan en MainActivity)` |
| P15 | | Audio | Botones de audio y prueba real | `Bloque XML + método Java` |
| P16 | | Diseño, validaciones y resumen | Identidad visual y recursos | `res/values/colors.xml + res/drawable/` |
| P17 | | Diseño, validaciones y resumen | Validación del formulario | `Método Java (se pega en MainActivity)` |
| P18 | | Diseño, validaciones y resumen | Resumen estadístico del equipo | `Método Java (se pega en MainActivity)` |
| P19 | | Integración y QA | Integrador (arma la app) | `MainActivity.java` |
| P20 | | Integración y QA | Tester / control de calidad | `Informe de pruebas` |
| P21 | | Integración y QA | Evidencias y exposición | `Carpeta de evidencias` |
| P22 | | Documentación y repositorio | Documentación del proyecto | `README.md del repositorio` |
| P23 | | Documentación y repositorio | Administrador del repositorio | `Repositorio de GitHub` |

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
