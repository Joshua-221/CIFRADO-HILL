# Proyecto: Implementación del Cifrado Hill

## Información del Estudiante

- **Nombre:** Joshua Cruz  
- **Grupo:** C  
- **Cuatrimestre:** Primero  
- **Carrera:** TSU en Desarrollo e Innovación de Software  
- **Materia:** Matemáticas para Computación  
- **Profesor:** Jorge Javier Pedrozo Romero  

---

## Descripción del Proyecto

Este proyecto consiste en la creación de una aplicación web que implementa el algoritmo clásico de cifrado Hill.  
Su propósito es demostrar el uso práctico de matrices, determinantes e inversos modulares en el área de seguridad informática básica.

La aplicación permite:
- Encriptar mensajes utilizando una matriz clave 2×2.
- Desencriptar mensajes usando la matriz inversa.
- Validar entradas, manejar caracteres incorrectos y aplicar relleno cuando sea necesario.

### Tecnologías utilizadas

- **HTML5:** estructura de la interfaz.  
- **CSS3:** diseño visual y distribución.  
- **JavaScript:** implementación del algoritmo matemático y manejo de la interacción del usuario.

---

## Instrucciones de Uso

No es necesario instalar ningún software.  
Basta con abrir **index.html** en cualquier navegador moderno.

**1. Ingresar el mensaje:**  
Escribe un texto de máximo 30 caracteres.

**2. Ingresar la matriz clave:**  
Completa los cuatro valores numéricos que forman la matriz 2×2:


**3. Encriptar:**  
Haz clic en el botón **"Encriptar"** para obtener el mensaje cifrado.

**4. Desencriptar:**  
Presiona **"Desencriptar"** para recuperar el texto original.

---

## Explicación Matemática del Cifrado Hill

El sistema trabaja con el alfabeto inglés (A=0, B=1, …, Z=25) bajo aritmética modular **mod 26**.

### Conversión del mensaje  
Las letras del mensaje se convierten a valores numéricos.  
Si el número de caracteres es impar, se agrega una *X* para completar el par.

### Encriptación  
Para cada par de letras se aplica:

\[
C = K \cdot P \mod 26
\]

Donde:
- **K** es la matriz clave
- **P** es el vector del par de letras
- **C** es el vector cifrado resultante

### Desencriptación  
Requiere la matriz inversa de K en módulo 26:

1. Calcular determinante → \( det = ad - bc \)  
2. Obtener inverso modular de det  
3. Formar la matriz adjunta  
4. Multiplicar adjunta por el inverso modular  
5. Aplicar mod 26 y corregir números negativos  

Si la matriz no tiene inverso modular, se notifica al usuario.

---

## Commits realizados

Estructura HTML base
Implementación del cifrado en JavaScript
Diseño inicial de estilos en CSS
Cálculo de matriz inversa y desencriptado
Mejoras visuales y organización del formulario


---

## Agradecimientos

- Profesor **Jorge Javier Pedrozo Romero** por la guía teórica.  
- Compañeros del grupo C por el apoyo durante el desarrollo.  

---

## Contacto

- **GitHub:** Joshua-221  

Proyecto desarrollado por **Joshua Cruz** — 2025.

