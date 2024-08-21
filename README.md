# Mensaje en Código Morse
## Descripción 👇
Esta aplicación tiene como función facilitar la comunicación privada :old_key: entre 2 o quizá más personas.Pues tiene un aspecto que lo hace algo particular y especial, y es que codifica los mensajes, convirtiéndolos a CÓDIGO MORSE.

El diseño está inspirado en mensajes secretos entre parejas, por ello usamos colores rosados y blancos, que son colores suaves.

Es un programa en el cuál ocupamos CSS y Javascript. Javascript se encarga de la interacción con la página, de que sea posible la codificación de texto a CÓDIGO MORSE.

Quizá podríamos agregarle una que otra función, como la de copiar texto. 

## Modo de Uso 
El modo de uso de la aplicación es fácil y sencillo.

Para codificar texto a Código morse debemos seguir los siguientes pasos:
  1. Pulsar sobre "Escribe tu mensaje aquí"
  2. Escribir o pegar su mensaje, teniendo en cuenta que no se puede hacer el uso de tildes, mayúsculas y puntos, pues podrían ser confundidos en el código.
  3. Presionar el botón que indica "Convertir a Código Morse"
Y listo! con eso obtendrías tu texto en Código Morse   :closed_lock_with_key:

Para decodificar Código Morse a texto debemos seguir los siguientes pasos:
  1. Pulsar sobre "Escribe el código Morse aquí"
  2. Escribir o copiar el código morse, tratando de percatarse que esté correctamente escrito, en caso de escribirlo a mano.
  3. Presionar el botón que indica "Decodificar a Texto"
Y listo! con eso obtendrás el código morse convertido a Texto   :unlock:

## 
Esta aplicación está especialmente dirigida y diseñada para parejas :kiss: , para permitirles comunicarse de manera secreta y más reservada :zany_face:.
Pero es apto para todo público.

Esperamos que la aplicación les sea útil :hugs:

otra explicacion de cual es la funcion que tiene el codigo 😉:)

Objetos morseCode y reverseMorseCode

- morseCode: Este objeto contiene las equivalencias entre caracteres alfabéticos y numéricos y sus respectivos códigos Morse.
- reverseMorseCode: Este objeto contiene las equivalencias inversas, es decir, de códigos Morse a caracteres alfabéticos y numéricos.

Conversión de texto plano a código Morse

1. Se selecciona el botón convert y se agrega un evento de clic.
2. Se obtiene el texto plano del usuario a través del elemento plain-text.
3. Se convierte el texto a minúsculas para asegurarse de que la conversión sea correcta.
4. Se itera sobre cada carácter del texto plano.
5. Si el carácter está en el objeto morseCode, se agrega su código Morse equivalente a la variable morseMessage.
6. Si el carácter no está en el objeto morseCode, se agrega un signo de interrogación (?) a la variable morseMessage.
7. Se utiliza la función typeEffect para simular un efecto de escritura en la salida del código Morse.

Función typeEffect

1. Se crea una función typeEffect que se llama recursivamente cada 50 milisegundos.
2. Se agrega cada carácter del código Morse a la salida morse-output utilizando outputElement.innerText.
3. Se incrementa el índice i para avanzar en la cadena de código Morse.

Conversión de código Morse a texto plano

1. Se selecciona el botón decode y se agrega un evento de clic.
2. Se obtiene el código Morse del usuario a través del elemento morse-code.
3. Se divide el código Morse en palabras utilizando el carácter / como separador.
4. Se itera sobre cada palabra y se divide en caracteres individuales utilizando el espacio como separador.
5. Si un carácter Morse está en el objeto reverseMorseCode, se agrega su equivalenteches alfabético o numérico a la variable decodedMessage.
6. Si un carácter Morse no está en el objeto reverseMorseCode, se agrega un signo de interrogación (?) a la variable decodedMessage.
7. Se muestra el mensaje decodificado en el elemento text-output.
