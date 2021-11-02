# Kredi Sr. Backend Developer
## Contenidos

- [General](#general)
- [Reglas](#reglas)
- [Recomendaciones](#recomendaciones)
- [Ruby quiz](#ruby-quiz)
- [Challenges](#challenges)

## General

Somos [Kredi](https://www.kredi.mx), Una fintech Mexicana enfocada en creditos hipotecarios en LatAm,Nos enfocamos en el desarrollo de software para procesos financieros críticos,nuestra meta es ofrecer al cliente la mejor experiencia al solicitar un crédito hipotecario a la vez que reducimos el tiempo de espera entre la solicitud y la formalización del crédito, nuestro equipo de desarrollo está enfocado en entrefar código de calidad, usable, legible, principios [S.O.L.I.D.](https://www.honeybadger.io/blog/ruby-solid-design-principles/#:~:text=The%20SOLID%20design%20principle%20includes,Liskov%20Substitution%20Principle), y las mejores prácticas en la industria.

A continuación presentamos un pequeño cuestionario para nuestra posición como Desarrollador de Software Backend Sr., te invitamos a seguir las recomendaciones para poder llevar a acabo esta prueba.

## Reglas

No hay reglas ;) desarrollar software debe ser algo que lleves en la sangre, que te motive y que te diviertas, que pienses en tu código como el trabajo en equipo, más personas trabajarán contigo.

## Recomendaciones

- **Por favor no menciones el nombre de la empresa en tu repositorio de entrega**
- Sé honesto, no copies de stackoverflow, a veces como programadores hacemos eso, pero esta vez queremos evaluar tu proceso de razonamiento, la forma en que planteas una solución a un problema así como la calidad de código.
- Haz uso de las mejores prácticas, usa nombres de variables entendibles, checa tu indentación, legibilidad del código, DRY, S.O.L.I.D., patrones de diseño, etc.
- Usa convenciones de código de ruby y ruby on rails
- Escribe pruebas de tu código, no sólo en terminal, te recomendamos usar RSpec.
- Publica tu código en `Github || Gitlab` preferentemente en un repositorio público, si no te es posible, usa un repositorio privado pero asegurate de invitar al Hiring manager.
- Pon cuidado en la descripción de tus commits, preferentemente en inglés técnico.
- Nos emociona ver que publiquen el proyecto en heroku, ver funcionar tu mini-proyecto es de las mejores experiencias que hemos tenido.
- Si requieres de ayuda o tienes dudas, por favor no dudes en comunicarte con el hiring manager.
- Evita que tu aplicación incurra en consultas n+1.


# Instrucciones

Cuestionario (Parte I):

A continuación te presentamos cinco preguntas sobre conocimientos generales de ruby, la idea es que podamos tener una llamada y juntos resolvamos las preguntas, queremos ver como analizas y resuelves problemas, descuida, te aseguramos que pediremos que hagas reverse de árboles binarios y esas cosas.


## Part I
### Ruby Quiz

Please add a file called `quiz.md` to your repo with your answers:

#### 1. Write a function that returns product of all numbers of an array/range

```ruby
>> product([1, 4, 21])
=> 84
>> product([-4, 2.3e12, 77.23, 982, 0b101])
=> -3.48863356e+18
>> product([-3, 11, 2])
=> -66
>> product([8, 300])
=> 2400
>> product([234, 121, 23, 945, 0])
=> 0
>> product(1..5)
=> 120
```

#### 2. Compare if two strings are anagrams (assume input consists of ASCII alphabets only)

```ruby
>> anagram?('Tap', 'paT')
=> true
>> anagram?('beat', 'table')
=> false
>> anagram?('beat', 'abet')
=> true
>> anagram?('seat', 'teal')
=> false
>> anagram?('god', 'Dog')
=> true
```

#### 3. Compare if two strings are same irrespective of case

```ruby
>> compare('nice', 'nice')
=> true
>> compare('how', 'who')
=> false
>> compare('GoOd DaY', 'gOOd dAy')
=> true
>> compare('foo', 'food')
=> false
```

#### 4. Write a function that sorts the keys in a hash by the length of the key as a string. For instance, the hash:

```ruby
{ abc: 'hello', another_key: 123, 4567 => 'third' }
```

should result in:

```ruby
["abc", "4567", "another_key"]
````


#### 5. Explain the difference between calling `super` and `super()` methods (OOP)


# Challenges

There are different challenges, please solve the challenge your recruiter asked you to solve.


### [Challenge 1: Url shortener](a1/README.md)

### [Challenge 2: Project Management Tool](a2/README.md)

<br/>
<br/>

### Happy coding! :)