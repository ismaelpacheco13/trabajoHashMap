# HashMap Java

## Concepto
El HashMap designa claves únicas para los valores correspondientes que se pueden recuperar en cualquier punto dado.

## Características

<img src="https://www.edureka.co/blog/wp-content/uploads/2019/09/img-recreate-01-1.jpg" alt="Par clave-valor">

- Los valores se pueden almacenar en un mapa formando un par clave-valor. El valor se puede recuperar usando la clave pasándola al método correcto.

- Si no existe ningún elemento en el Map, se arrojará una excepción "NoSuchElementException".

- HashMap almacena solo referencias de objetos. Por eso, es imposible utilizar tipos de datos primitivos como double o int. Hay que usar la clase envoltorio en su lugar (Integer o Double).

## Uso de HashMap en Java
Para declarar un HashMap en Java deberemos de instanciarlo de alguna de estas dos formas:

```java
HashMap <String, Object> map = new HashMap <String, Object> ();
HashMap x = new HashMap ();
```

***Métodos:***
Los métodos más empleados para esta clase son los siguientes:
- get (object key): devuelve un valor asociado a una clave especificada.

- put (object key, string value): almacena el valor especificado y lo asocia a la clave especificada.

## Ejemplo de HashMap
Este sería un ejemplo de implementación de HashMap en Java:

```java
import java.util.HashMap;
import java.util.Map;

public class Ejemplo_HashMap {
  public static void main (String[] args) {
    HashMap x = new HashMap();
    
    x.put("Nombre", "Ismael");
    x.put("Apellido", "Pacheco");
    x.put("Estudios", "Desarrollo de Aplicaciones Multiplataforma");
    x.put("Prueba", "Para eliminar");
  }
}
```

Si por ejemplo quisieramos eliminar algun elemento del HashMap simplemente utilizariamos remove(clave):

```java
x.remove("Prueba"); // Con esto se eliminaría el valor "Para eliminar" asociado a la clave "Prueba"
```

Podemos obtener todos los valores existentes en el HashMap mediante:
```java
System.out.println(x.values());
```

En nuestro caso devolvería los siguientes valores:
> [Ismael, Pacheco, Desarrollo de Aplicaciones Multiplataforma, Para eliminar]

Podemos hacer lo mismo para obtener todas las claves mediante:
```java
System.out.println(x.keySet());
```

En nuestro caso devolvería las siguientes claves:
> [Nombre, Apellido, Estudios, Prueba]

> :star: Si te ha gustado este resumen dale una estrellita al [repositorio](https://github.com/ismaelpacheco13/trabajoHashMap)
