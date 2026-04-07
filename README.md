# 🧪 Práctica: Pruebas Unitarias con JUnit 5 en VS Code

Este proyecto forma parte de una práctica avanzada de **Entornos de Desarrollo**. El objetivo principal es demostrar la capacidad de configurar, desarrollar y testear aplicaciones Java utilizando **Visual Studio Code** y **Maven**, prescindiendo de herramientas automáticas de otros IDEs como IntelliJ.

---

## 🎯 Objetivos de la Práctica
* **Configuración Manual:** Crear y estructurar un proyecto Java desde cero usando asistentes de Maven.
* **Gestión de Dependencias:** Configurar correctamente el archivo `pom.xml` para integrar frameworks de terceros.
* **Calidad de Software:** Aplicar el paradigma de **Pruebas Unitarias** para asegurar que la lógica de negocio es robusta.
* **Dominio de VS Code:** Manejar el panel de *Testing*, *CodeLens* y herramientas de *Depuración*.

---

## 📂 Estructura del Proyecto

Siguiendo el estándar de Maven, el proyecto se organiza de la siguiente manera:

| Ubicación | Archivo | Descripción |
| :--- | :--- | :--- |
| `src/test/java/entornos` | `CalculadoraRiesgo.java` | Lógica principal del programa. |
| `src/test/java/entornos` | `CalculadoraRiesgoTest.java` | Suite de pruebas unitarias. |
| `/` | `pom.xml` | Archivo de configuración de Maven y dependencias. |

---

## 🛠️ Configuración y Desarrollo

### 1. Inicialización
El proyecto fue generado mediante el comando `Java: Create Java Project` > `Maven` > `maven-archetype-quickstart`, definiendo los siguientes identificadores:
- **GroupId:** `entornos`
- **ArtifactId:** `test-vscode`

### 2. Configuración de JUnit 5
Se modificó el archivo `pom.xml` para sustituir versiones antiguas por **JUnit Jupiter**, permitiendo el uso de anotaciones modernas:

```xml
<dependency>
    <groupId>org.junit.jupiter</groupId>
    <artifactId>junit-jupiter-api</artifactId>
    <version>5.10.0</version>
    <scope>test</scope>
</dependency>
