# Actividad3ED
Actividad UML 

----------------------------------------------------

CASOS DE USO

![casos_de_uso drawio](https://github.com/user-attachments/assets/36be46ba-26ad-4153-86dd-9b6c58390fd5)

Explicación:
Decidí darle dos entidades para darle más sentido al diseño. Por una parte,
tenemos al usuario común que busca crear un torneo y registrar a su equipo favorito.

Por otro lado, tenemos a un encargado de administrar los resultados de los encuentros,
actualizar la tabla de clasificaciones, emparejar a los diferentes equipos, etc.
Pienso que con estos dos roles que interactúan con el sistema y sus acciones, es
suficiente para mantenerlo funcionando.

Cada caso de uso representa las acciones que se pueden tomar, unas que son obligatorias representadas
con 'include'  como: verificar si el torneo existe, y otras opciones con 'extend' como: ver información de...

He intentado utilizar una cantidad adecuada de casos de uso para no sobrecargar el diagrama, en mi opinión,
con los que están ahí es suficiente para lograr su cometido, entenderse de la manera más breve posible.

----------------------------------------------------

DIAGRAMA DE CLASES

Guía hecha en una nota para su posterior implementación a diagrama:

![Captura de pantalla 2025-04-20 172243](https://github.com/user-attachments/assets/bab37e97-8684-4cb9-b5a4-ee0971fd8e78)


![diagrama_clases drawio](https://github.com/user-attachments/assets/fcd035f9-26c8-4d6d-ba4f-531684a8b4f9)

En la parte superior he subido una nota que hice para guiarme al hacer luego el diagrama de clases, lo usé como
referencia para el modelado, más no terminó siendo exactamente igual.

Aquí agregué cinco clases: Torneo, Partida, Premio, Equipo y Jugadores.
Empezando con torneo, le di sus atributos correspondientes privados con un método llamado 'existencia',
es un método simple que hace, como dice la palabra, corroborar la existencia del mismo.
Tiene una relación de agregación con partida y premio, dado que en mi razonamiento, ambos pueden existir
sin la necesidad de formar parte de manera forzosa de un torneo.

Las clases 'Partida' y 'Premio' tienen sus atributos correspondientes, con la diferencia de que 'Partida' tiene
un método llamado 'registrarResultado' y 'Premio' no tiene ninguno.

A la derecha tenemos a las clases 'Equipo' y 'Jugadores', ambos tienen una relación de segregación, dado que
jugadores pertenece a un equipo, pero no tiene que hacerlo de manera obligatoria para existir. En mi razonamiento,
los jugadores existen perfectamente sin un equipo. Ambos tienen sus atributos privados.
Equipo tiene un método llamado 'existencia', que al igual que torneo, solamente confirma la existencia del mismo.
Jugadores tiene un método 'competir', que es lo que van a hacer principalmente en el torneo.

----------------------------------------------------

CONCLUSIONES

He intentado hacer tanto el diagrama de clases como el de casos de uso de la manera mas entendible posible, sin
agregar demasiadas cosas que puedan hacer más difícil su comprensión, ya que lo que buscamos es llevar un mensaje claro 
de cómo queremos que se lleve a cabo un proyecto.
Pienso que las relaciones, clases creadas en el diagrama de clases y los actores, casos de uso en el diagrama de casos de
uso, están bien justificados según mi razonamiento.

