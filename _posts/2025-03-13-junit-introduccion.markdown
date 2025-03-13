---
layout: post
title:  "Introducción a las Pruebas con JUnit"
date:   2025-03-12 
categories: jekyll deployment github
---

![JUnit](../assets/images/JUnit.svg)

JUnit es un framework de pruebas para Java que permite escribir y ejecutar pruebas automatizadas de manera sencilla. En esta guía, aprenderás cómo crear pruebas unitarias con JUnit.

## 1. Configuración de JUnit

Antes de comenzar, asegúrate de tener JUnit en tu proyecto. Si usas **Maven**, agrega la siguiente dependencia en tu `pom.xml`:

```xml
<dependencies>
    <dependency>
        <groupId>org.junit.jupiter</groupId>
        <artifactId>junit-jupiter-api</artifactId>
        <version>5.9.0</version>
        <scope>test</scope>
    </dependency>
</dependencies>
```

Para **Gradle**, agrega:

```gradle
dependencies {
    testImplementation 'org.junit.jupiter:junit-jupiter:5.9.0'
}
```

## 2. Creando una Prueba con JUnit

A continuación, crearemos una prueba para una clase sencilla de matemáticas:

```java
public class Calculadora {
    public int suma(int a, int b) {
        return a + b;
    }
}
```

Ahora escribimos la prueba usando JUnit:

```java
import static org.junit.jupiter.api.Assertions.assertEquals;
import org.junit.jupiter.api.Test;

class CalculadoraTest {
    @Test
    void testSuma() {
        Calculadora calc = new Calculadora();
        int resultado = calc.suma(2, 3);
        assertEquals(5, resultado, "La suma de 2 + 3 debe ser 5");
    }
}
```

## 3. Ejecutando las Pruebas

Para ejecutar las pruebas, puedes usar:

- **Maven**: `mvn test`
- **Gradle**: `gradle test`
- **IDE (IntelliJ, Eclipse, VS Code)**: Click derecho en la clase de prueba y selecciona "Run".

## 4. Anotaciones Comunes en JUnit

JUnit proporciona varias anotaciones útiles:

- `@Test`: Define un método de prueba.
- `@BeforeEach`: Ejecuta código antes de cada prueba.
- `@AfterEach`: Ejecuta código después de cada prueba.
- `@BeforeAll`: Se ejecuta antes de todas las pruebas (debe ser estático).
- `@AfterAll`: Se ejecuta después de todas las pruebas (debe ser estático).

Ejemplo:

```java
import org.junit.jupiter.api.BeforeEach;
import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.*;

class CalculadoraTest {
    private Calculadora calc;

    @BeforeEach
    void setUp() {
        calc = new Calculadora();
    }

    @Test
    void testSuma() {
        assertEquals(5, calc.suma(2, 3));
    }
}
```

## Conclusión

JUnit es una herramienta poderosa para escribir pruebas automatizadas en Java. Con este conocimiento básico, puedes mejorar la calidad de tu código y prevenir errores antes de que lleguen a producción.

¡Empieza a probar tu código con JUnit hoy! 🚀

