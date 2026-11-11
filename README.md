# Actividad 4: Manejo de Excepciones y Archivos en Java (GUI)

Repositorio correspondiente al desarrollo de la **Actividad 4** de la asignatura **Programación Orientada a Objetos**. Todos los ejercicios han sido implementados en **Java** haciendo uso de interfaces gráficas de usuario mediante la librería **Java Swing**[cite: 9].

---

## 📋 Información Académica

* **Institución:** Universidad Nacional de Colombia[cite: 9]
* **Asignatura:** Programación Orientada a Objetos (2026-2S)[cite: 9]
* **Docente:** Walter Hugo Arboleda Mazo[cite: 9]
* **Texto Guía:** *Ejercicios de Programación Orientada a Objetos con Java y UML* — Leonardo Bermón Angarita (Universidad Nacional de Colombia)[cite: 9]

---

## 🚀 Ejercicios Desarrollados

El proyecto resuelve los 5 ejercicios solicitados del **Capítulo 6** del texto guía, integrando validación de entradas, captura de excepciones estándar y personalizadas, y modelado UML (Diagramas de Clases y Casos de Uso)[cite: 9]:

### 1. Ejercicio Página 400 — Manejo Básico de Excepciones (`try-catch`)
* **Descripción:** Implementación de operaciones aritméticas básicas (división) con captura de excepciones de ejecución (`ArithmeticException` por división entre cero y `NumberFormatException` por entradas no numéricas).
* **Componentes principales:** Interfaz gráfica en Swing con alertas modales (`JOptionPane`) para informar errores al usuario sin detener la ejecución del programa.

### 2. Ejercicio Página 406 — Lanzamiento de Excepciones (`throw` / `throws`)
* **Descripción:** Implementación de la clase `Vendedor` con reglas de negocio estrictas sobre el atributo `edad` (no puede ser negativa, mayor a 120 años, ni menor a 18 años).
* **Componentes principales:** Método estático de validación que lanza instancias de `IllegalArgumentException` antes de permitir la creación del objeto.

### 3. Ejercicio Página 412 — Captura Múltiple y Cálculos Numéricos
* **Descripción:** Implementación de la clase `CalculosNumericos` para el cálculo de logaritmo neperiano, raíz cuadrada, pendiente de una recta, punto medio, raíces de una ecuación cuadrática y conversión de base 10 a base $b$[cite: 7].
* **Componentes principales:** Selector dinámico de operaciones (`JComboBox`) y manejo de múltiples bloques `catch` para gestionar excepciones matemáticas (`ArithmeticException`), de argumentos (`IllegalArgumentException`) y de formato (`NumberFormatException`).

### 4. Ejercicio Página 418 — Validación de Campos (`EquipoMaratónProgramación`)
* **Descripción:** Registro y validación de equipos participantes en una maratón de programación mediante la clase `EquipoMaratonProgramacion`[cite: 8].
* **Componentes principales:** Verificación de campos obligatorios no vacíos, restricción de longitud de caracteres, prohibición de dígitos numéricos en nombres de equipo/universidad y control de rango de integrantes (2 a 3 programadores)[cite: 8].

### 5. Ejercicio Página 427 — Lectura y Escritura de Archivos
* **Descripción:** Gestión de persistencia en archivos de texto plano (`.txt`) mediante flujos de entrada y salida (`FileReader`, `BufferedReader`, `FileWriter`, `BufferedWriter`).
* **Componentes principales:** Uso de bloques `try-with-resources` y captura específica de `FileNotFoundException` (cuando el archivo solicitado no existe) e `IOException` (fallos de lectura/escritura).

---

## 🛠️ Requisitos y Ejecución

* **JDK:** Java Development Kit 8 o superior.
* **IDE recomendado:** Visual Studio Code (con *Extension Pack for Java*) o NetBeans / IntelliJ IDEA.

### Pasos para ejecutar en local:
1. Clonar este repositorio:
   ```bash
   git clone <URL_DE_TU_REPOSITORIO>
