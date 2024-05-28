# Entrevista desarrollador IOs

Este repo tiene como objetivo proporcionar un listado de preguntas para desarrolladores de IOS

## Tipos de Datos y Colecciones

- ¿Cómo se declara y utiliza un `Array` en Swift? Proporcione un ejemplo de cómo agregar, eliminar y acceder a elementos.
- ¿Qué es un `Set` en Swift y en qué casos lo usarías en lugar de un `Array`?

## Opcionales

- ¿Qué es un opcional en Swift y por qué son útiles? Proporcione un ejemplo de cómo declarar y desempaquetar un opcional de forma segura.
- ¿Qué es el desempaquetado forzado y en qué situaciones se debería evitar?
- ¿Cómo se usa la sentencia guard let para desempaquetar opcionales? ¿Cuáles son las ventajas de usar guard let sobre if let?
- ¿Qué es el operador nil-coalescing (??) y cómo se usa? Proporcione un ejemplo.
- ¿Cuáles son las diferencias entre el uso del operador nil-coalescing y el desempaquetado forzado?
- ¿Cómo se define una función que retorna un opcional? Proporcione un ejemplo.
- ¿Cómo manejas los valores opcionales que se retornan de una función?
- ¿Cuáles son las ventajas y desventajas de usar propiedades opcionales en comparación con propiedades implícitamente desempaquetadas?
- Mejora de Código Existente:

```swift
let name: String? = "John Doe"
if name != nil {
    print("Hello, \(name!)")
} else {
    print("Hello, Guest")
}
```

- Escribe una línea de código que imprima el nombre de la calle de forma segura utilizando encadenamiento opcional.
```swift
struct User {
    var address: Address?
}

struct Address {
    var street: String?
}

let user: User? = User(address: Address(street: "Main Street"))
```

## Condicionales y Bucles

- Explique cómo se utilizan las sentencias `if` y `switch` en Swift. Proporcione ejemplos de cada uno.
- ¿Cómo se implementan los bucles `for`, `while` y `repeat-while` en Swift? Proporcione un ejemplo para cada uno.

## Guard y Defer

- ¿Qué es una sentencia `guard` y cuándo la usarías? Proporcione un ejemplo.
- ¿Qué es la sentencia `defer` y cómo puede ser útil en la gestión de recursos?

## Funciones

- ¿Cómo se declara una función en Swift? Proporcione un ejemplo que incluya parámetros y un valor de retorno.
- ¿Qué es una función anidada y cómo se usa en Swift?

## Closures

- Explique qué es un closure en Swift y proporcione un ejemplo de cómo se declara y utiliza.
- ¿Qué es la captura de valores en closures y cómo afecta el comportamiento del closure?

## Clases y Estructuras

- ¿Cuáles son las principales diferencias entre una `class` y una `struct` en Swift?
- ¿Cuándo preferirías usar una estructura sobre una clase y viceversa?
- ¿Cuándo preferirías usar una estructura sobre una clase y viceversa en SwiftUI?
- ¿Cómo se definen métodos en una clase y una estructura? ¿Existen diferencias en la forma en que los métodos se comportan en ambas?
- ¿Cómo se implementa la herencia en Swift? Proporcione un ejemplo de una clase base y una clase derivada.
- ¿Por qué las estructuras no soportan herencia en Swift?
- ¿Cuáles son las diferencias en la conformidad a protocolos entre clases y estructuras?
- ¿Cómo se diferencian las clases y las estructuras en términos de semántica de copia y referencia?
- Proporcione un ejemplo que demuestre cómo las instancias de clase comparten referencias y cómo las instancias de estructuras se copian por valor.
- ¿Qué es un deinitializer en Swift y cómo se usa en una clase?
- ¿Por qué las estructuras no tienen deinitializers?
- ¿Cómo se declaran y utilizan las propiedades computadas en una clase y una estructura?
- ¿Cuándo usarías una propiedad computada sobre una propiedad almacenada?
- ¿Cómo haces que una clase o una estructura sean equatables en Swift? Proporcione un ejemplo.

## Protocolos y Delegación

- ¿Qué es un protocolo en Swift y cómo se define? Proporcione un ejemplo de un protocolo y una clase que lo implemente.
- ¿Cómo funciona el patrón de delegación en Swift? Proporcione un ejemplo.

## Manejo de Memoria

- ¿Qué diferencia hay entre `weak` `unowned` y `strong`?

## Manejo de Errores

- ¿Cómo se manejan los errores en Swift? Explique el uso de `do-catch` y `throws`.
- ¿Qué es un `guard` con manejo de errores y cómo se usa?

## Concurrencia y Multithreading

- ¿Qué es Grand Central Dispatch (GCD) y cómo se utiliza para manejar tareas en segundo plano en Swift?
- ¿Cómo se utilizan los dispatch queues para gestionar tareas concurrentes?

## Generics

- ¿Qué son los genéricos en Swift y cómo se definen? Proporcione un ejemplo de una función genérica.
- ¿Cuáles son las ventajas de utilizar genéricos en el código Swift?

## Extensions y Protocol Extensions

- ¿Qué son las extensiones en Swift y cuándo se utilizan? Proporcione un ejemplo.
- ¿Cómo funcionan las extensiones de protocolos y qué beneficios aportan?
- ¿Cuáles son las limitaciones de las extensiones en comparación con la modificación directa de la declaración de una clase o estructura?

## Ejemplos Prácticos

- ¿Cómo implementarías una funcionalidad de búsqueda en una lista de elementos en Swift? Proporcione un pseudocódigo o una implementación simplificada.
- Describa cómo implementaría un cargador de imágenes asíncrono en una aplicación iOS usando Swift.







