
# 📝 Práctica: PR-Eclipse-01-PrimerPrograma

## Objetivo

* Crear y ejecutar un proyecto Java en Eclipse.
* Practicar la escritura básica en Java (clases, `main`, instrucciones).
* Usar comentarios y mantener el código legible.
* Aplicar refactorización y formateo automático.
* Entregar el proyecto completo en GitHub.

---

## 1. Crear proyecto, paquete y clase

1. `File → New → Java Project`.

   * **Project name**: `PrimerPrograma`.
   * Desactiva **Create module-info.java file** (no trabajamos con módulos todavía).
   * Pulsa *Finish*.
2. En **src**, crea un **paquete** llamado `tema2_eclipse`.
3. Dentro del paquete, crea una **clase** llamada `MyFirstProgramme`.

   * Marca la casilla para añadir el método `public static void main(String[] args)`.

---

## 2. Escribir el primer programa

En el método `main`, escribe (usa la plantilla **sysout**: teclea `sysout` y pulsa `Ctrl + Espacio`):

```java
System.out.println("¡Mi primer programa!");
```

Ejecuta el programa con el botón verde ▶️ o `Run → Run`.
La consola debe mostrar:

```
¡Mi primer programa!
```

Añade más salidas:

```java
System.out.println("Reglas básicas de Java:");
System.out.println("1) Distingue MAYÚSCULAS y minúsculas");
System.out.println("2) Cada instrucción termina con ;");
```

---

## 3. Usar comentarios

* **Comentario de una línea**:

```java
// Este programa imprime mensajes en consola
```

* **Comentario de varias líneas**:

```java
/* 
   Autor: (escribe tu nombre)
   Fecha: (escribe la fecha)
*/
```

💡 Atajo: comentar/descomentar rápidamente → **Ctrl+Shift+C** o **Ctrl+7**.

---

## 4. Refactorización (Rename)

* Crea una variable:

```java
int totalMensajes = 0;
totalMensajes++;
System.out.println("Mensajes impresos: " + totalMensajes);
```

* Selecciona `totalMensajes` → **Alt+Shift+R** (o botón derecho → Refactor → Rename).
  Renómbrala a `contadorMensajes`. Eclipse actualizará todas las referencias.

* Haz lo mismo con la clase `MyFirstProgramme` → renómbrala a `HelloEclipse`.
  Eclipse renombrará también el archivo `.java`.

---

## 5. Formateo automático

Pega este código mal tabulado:

```java
int x=3;
    System.out.print("Este código no está");
System.out.print(" muy bien ");
            System.out.print("tabulado");
x=7;
System.out.println();
```

Pulsa **Ctrl+Shift+F** (o `Source → Format`).
Eclipse lo corregirá automáticamente con sangrado uniforme:

```java
int x = 3;
System.out.print("Este código no está");
System.out.print(" muy bien ");
System.out.print("tabulado");
x = 7;
System.out.println();
```

---

## 6. Código final (ejemplo orientativo)

```java
package tema2_eclipse;

public class HelloEclipse {

    public static void main(String[] args) {
        // Comentario de una línea: primer programa
        System.out.println("¡Mi primer programa!");

        System.out.println("Reglas básicas de Java:");
        System.out.println("1) Distingue MAYÚSCULAS y minúsculas");
        System.out.println("2) Cada instrucción termina con ;");

        /* Comentario de varias líneas:
           Autor: (alumno)
           Fecha: (hoy)
        */

        int x = 3;
        System.out.print("Este código no está");
        System.out.print(" muy bien ");
        System.out.print("tabulado");
        x = 7;
        System.out.println();

        int contadorMensajes = 0;
        contadorMensajes++;
        System.out.println("Mensajes impresos: " + contadorMensajes);
    }
}
```

---

## 🔄 Entrega

1. Crea un **repositorio público en GitHub** llamado:
   **`PR-Eclipse-01-PrimerPrograma`**.
2. Sube al repositorio la **carpeta completa del proyecto de Eclipse** (con `.project`, `.classpath`, carpeta `src`, etc.).
3. Entrega en Moodle la **URL del repositorio**.

