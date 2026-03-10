# Proyecto Extraordinaria — Taller de Programación 2025-26

UPM · ETSISI · Taller de Programación - Convocatoria Extraordinaria

Aplicación en Java para la organización de recetas y planificación de comidas semanales.

---

## Descripción

Este proyecto consiste en implementar una aplicación de consola que permita al usuario:

- Gestionar un **libro de recetas** (agregar, buscar, editar y eliminar recetas).
- Cada receta contiene un **nombre**, una lista de **ingredientes** y una lista de **instrucciones**.
- Planificar las **comidas de la semana** asignando recetas a cada día.
- **Guardar y cargar** tanto el libro de recetas como el plan semanal en ficheros de texto.

---

## Estructura del proyecto

```text
src/
├── main/java/
│   ├── Main.java               # Punto de entrada de la aplicación
│   ├── Receta.java             # Representa una receta (nombre, ingredientes, instrucciones)
│   ├── LibroDeRecetas.java     # Colección de recetas con búsqueda, carga y guardado
│   ├── PlanificadorSemanal.java# Plan de comidas de lunes a domingo
│   ├── InterfazUsuario.java    # Menú interactivo por consola
│   └── Utilidades.java         # Lectura robusta de teclado (cadenas, números, días)
└── test/java/
    ├── RecetaTest.java
    ├── LibroDeRecetasTest.java
    ├── PlanificadorSemanalTest.java
    ├── InterfazUsuarioTest.java
    └── UtilidadesTest.java
```

---

## Tecnologías

- **Java 22**
- **Maven** (gestión de dependencias y build)
- **JUnit Jupiter 5.8.1** (tests unitarios)

---

## Cómo ejecutar

### Compilar y ejecutar tests

```bash
mvn test
```

### Compilar y ejecutar la aplicación

```bash
mvn compile
mvn exec:java -Dexec.mainClass="Main"
```

---

## Formato del fichero de recetas

Cada receta se almacena con el siguiente formato:

```text
Nombre de la receta
ingrediente 1
ingrediente 2
...
INSTRUCCIONES
Paso 1
Paso 2
...
-----
```

El separador `INSTRUCCIONES` divide ingredientes de pasos, y `-----` marca el fin de cada receta.

---

## Autor

Luis hernares sera
Daniel Aparisi Lozano

Proyecto para la convocatoria extraordinaria de **Taller de Programación** — UPM ETSISI 2025-26.
