<!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->

- [Entrevista desarrollador IOs](#entrevista-desarrollador-ios)
   * [Tipos de Datos y Colecciones](#tipos-de-datos-y-colecciones)
   * [Opcionales](#opcionales)
   * [Condicionales y Bucles](#condicionales-y-bucles)
   * [Guard y Defer](#guard-y-defer)
   * [Funciones](#funciones)
   * [Closures](#closures)
   * [Clases y Estructuras](#clases-y-estructuras)
   * [Protocolos y Delegación](#protocolos-y-delegación)
   * [Manejo de Memoria](#manejo-de-memoria)
   * [Manejo de Errores](#manejo-de-errores)
   * [Concurrencia y Multithreading](#concurrencia-y-multithreading)
   * [Generics](#generics)
   * [Extensions y Protocol Extensions](#extensions-y-protocol-extensions)
   * [Ejemplos Prácticos](#ejemplos-prácticos)

<!-- TOC end -->

<!-- TOC --><a name="entrevista-desarrollador-ios"></a>
# Entrevista desarrollador IOs

Este repo tiene como objetivo proporcionar un listado de preguntas para desarrolladores de IOS

<!-- TOC --><a name="tipos-de-datos-y-colecciones"></a>
## Tipos de Datos y Colecciones

- ¿Cómo se declara y utiliza un `Array` en Swift? Proporcione un ejemplo de cómo agregar, eliminar y acceder a elementos.
- ¿Qué es un `Set` en Swift y en qué casos lo usarías en lugar de un `Array`?

<!-- TOC --><a name="opcionales"></a>
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

<!-- TOC --><a name="condicionales-y-bucles"></a>
## Condicionales y Bucles

- Explique cómo se utilizan las sentencias `if` y `switch` en Swift. Proporcione ejemplos de cada uno.
- ¿Cómo se implementan los bucles `for`, `while` y `repeat-while` en Swift? Proporcione un ejemplo para cada uno.
- ¿Cómo se declara y utiliza un bucle for-in en Swift? Proporciona un ejemplo.
- ¿Cuál es la diferencia entre un bucle `for-in` y un bucle for clásico?
- ¿Cuándo es más apropiado usar un bucle `while` en lugar de un bucle `for`?
- ¿Cómo se utiliza la sentencia `break` para salir de un bucle en Swift? Proporciona un ejemplo.
- ¿Qué hace la sentencia `continue y cómo se usa en un bucle? Proporciona un ejemplo.

<!-- TOC --><a name="guard-y-defer"></a>
## Guard y Defer

- ¿Qué es una sentencia `guard` y cuándo la usarías? Proporcione un ejemplo.
- ¿Qué es la sentencia `defer` y cómo puede ser útil en la gestión de recursos?

<!-- TOC --><a name="funciones"></a>
## Funciones

- ¿Cómo se declara una función en Swift? Proporcione un ejemplo que incluya parámetros y un valor de retorno.
- ¿Qué es una función anidada y cómo se usa en Swift?
- ¿Cómo se definen valores por defecto para los parámetros de una función en Swift? Proporcione un ejemplo.
- ¿Cuándo es útil usar valores por defecto en los parámetros de una función?
- ¿Qué es un parámetro in-out en Swift y cómo se usa? Proporcione un ejemplo.
- ¿Cuáles son los beneficios de usar funciones anidadas?
- ¿Qué es la sobrecarga de funciones en Swift? Proporcione un ejemplo.
- ¿Qué es una función recursiva y cómo se usa en Swift? Proporcione un ejemplo de una función recursiva que calcule el factorial de un número.
- ¿Cuáles son los riesgos asociados con las funciones recursivas y cómo se pueden mitigar?

<!-- TOC --><a name="closures"></a>
## Closures

- Explique qué es un closure en Swift y proporcione un ejemplo de cómo se declara y utiliza.
- ¿Qué es la captura de valores en closures y cómo afecta el comportamiento del closure?

<!-- TOC --><a name="clases-y-estructuras"></a>
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

<!-- TOC --><a name="protocolos-y-delegación"></a>
## Protocolos y Delegación

- ¿Qué es un protocolo en Swift y cómo se define? Proporcione un ejemplo de un protocolo y una clase que lo implemente.
- ¿Cómo funciona el patrón de delegación en Swift? Proporcione un ejemplo.
- ¿Cómo se hace que una clase, estructura o enumeración cumpla con un protocolo? Proporcione un ejemplo.
- ¿Es posible que una clase o estructura cumpla con múltiples protocolos? Proporcione un ejemplo.
- ¿Cuáles son las diferencias entre las propiedades requeridas y opcionales en un protocolo?
- ¿Cómo se declaran los métodos requeridos en un protocolo y cómo se implementan en una clase que adopta ese protocolo?
- Implemente un protocolo Vehicle que tenga una propiedad numberOfWheels y un método drive(). Luego, cree dos clases Car y Bicycle que adopten este protocolo.

<!-- TOC --><a name="manejo-de-memoria"></a>
## Manejo de Memoria

- ¿Qué diferencia hay entre `weak` `unowned` y `strong`?

<!-- TOC --><a name="manejo-de-errores"></a>
## Manejo de Errores

- ¿Cómo se manejan los errores en Swift? Explique el uso de `do-catch` y `throws`.
- ¿Qué es un `guard` con manejo de errores y cómo se usa?
- ¿Cómo se define un tipo de error en Swift? Proporcione un ejemplo.
- ¿Cómo se declara una función que puede lanzar errores en Swift? Proporcione un ejemplo.
- ¿Cómo llamas a una función que lanza errores usando try?
- ¿Cómo se usa un bloque do-catch para manejar errores en Swift? Proporcione un ejemplo.
- ¿Cómo se manejan múltiples tipos de errores en un bloque do-catch?
- ¿Qué es la propagación de errores y cómo se implementa en Swift? Proporcione un ejemplo.
- ¿Cómo se usa el operador `try?` y en qué casos es útil?
- ¿Cómo se convierte un error en otro tipo de error en Swift? Proporcione un ejemplo.
- ¿Cómo defines un error personalizado en Swift? Proporcione un ejemplo
- ¿Qué beneficios tienen los errores personalizados en comparación con los errores genéricos?
- Mejora de Código Existente:

```swift
func fetchData() -> String {
    if let data = try? loadData() {
        return data
    } else {
        return "Default Data"
    }
}
```

<!-- TOC --><a name="concurrencia-y-multithreading"></a>
## Concurrencia y Multithreading

- ¿Qué es Grand Central Dispatch (GCD) y cómo se utiliza para manejar tareas en segundo plano en Swift?
- ¿Cómo se utilizan los dispatch queues para gestionar tareas concurrentes?

<!-- TOC --><a name="generics"></a>
## Generics

- ¿Qué son los genéricos en Swift y cómo se definen? Proporcione un ejemplo de una función genérica.
- ¿Cuáles son las ventajas de utilizar genéricos en el código Swift?

<!-- TOC --><a name="extensions-y-protocol-extensions"></a>
## Extensions y Protocol Extensions

- ¿Qué son las extensiones en Swift y cuándo se utilizan? Proporcione un ejemplo.
- ¿Cómo funcionan las extensiones de protocolos y qué beneficios aportan?
- ¿Cuáles son las limitaciones de las extensiones en comparación con la modificación directa de la declaración de una clase o estructura?

<!-- TOC --><a name="ejemplos-prácticos"></a>
## Ejemplos Prácticos

- ¿Cómo implementarías una funcionalidad de búsqueda en una lista de elementos en Swift? Proporcione un pseudocódigo o una implementación simplificada.
- Describa cómo implementaría un cargador de imágenes asíncrono en una aplicación iOS usando Swift.







