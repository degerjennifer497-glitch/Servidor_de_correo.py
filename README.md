




UNIVERSIDAD NACIONAL Guillermo Brown 

Tecnicatura Universitaria en Programación

ASIGNATURA: Estructura de Datos

CICLO LECTIVO: 2025

Trabajo Práctico :” Cliente de Correo electrónico”


Docente:
Bianco Angel Leonardo

Alumnos:
Deger Jennifer Pamela,Benitez Agustin Ariel

Lineamientos generales:

El siguiente trabajo consiste en emular un sistema de correo electrónico que sea capaz de enviar y recibir mensajes utilizando el paradigma de programación orientado a objetos.Para ello hemos decido utilizar 4 clases principales (Interfaz, servidor, mensaje y usuario)
Cuyo funcionamiento estaremos detallando a continuación:

Interfaz: Decidimos crear la clase interfaz como plantilla que heredará la clase usuario y los distintos tipos de clase usuario que podría llegar a haber en el futuro. En ella definimos los métodos que creemos que deberá tener cualquier usuario que utilice esta plataforma, los cuales son: Enviar mensaje, recibir mensaje, mostrar bandeja de entrada y mostrar bandeja de salida.

Servidor: La clase servidor se encarga de articular las clases Mensaje y Usuario. Nos provee de un Menú para crear los usuarios y los guarda en una lista para luego poder acceder a ellos y utilizar sus correspondientes atributos.

Mensaje: La clase mensaje nos provee de un formato para crear los mensajes que posteriormente se estarán enviando entre los usuarios.

Usuario: Esta clase nos permite definir los parámetros que deben tener los clientes en el correo. Definimos los atributos nombre, correo y contraseña con la característica privada puesto que creemos que se trata de información confidencial del cliente de modo que los encapsulamos y posteriormente procedimos a crear a partir de decoradores los métodos  getters y setters para acceder y/o modificar estos atributos en caso de que sea necesario. Y además hereda los métodos de interfaz (que nos permiten enviar mensajes, recibir mensaje, ver bandeja de entrada y salida). 

Ejecución de el programa:

El programa al ser ejecutado,ofrece un menú donde el usuario podrá seleccionar alguna de las siguientes opciones que deberán ser ingresadas manualmente :

  Menú Principal:
  
1_ Crear usuario: Al seleccionar la opción 1 (uno) el programa solicitará al usuario tres datos que serán utilizados para darle identidad  dentro del mismo y por lo tanto serán almacenados. Los datos solicitados son nombre, correo y contraseña y serán solicitados en ese orden bajo la leyenda; “Decime tu nombre” para el dato nombre; “Decime tu correo” para almacenar Correo; “contraseña (debe tener al menos 6 caracteres,un número, mayusculas y minusculas” donde el programa aclara el formato que debe tener la contraseña. (En caso de que la contraseña no cumpla con este formato se ejecuta un bucle con la leyenda “La contraseña no cumple con los requisitos. Intente nuevamente” , este bucle sólo se rompe en caso de que el usuario cargue correctamente la contraseña). Al finalizar la carga el programa imprimirá en pantalla  “El usuario fue agregado correctamente” a modo de aviso y nos retorna inmediatamente al menú principal.

2_ Iniciar sesión: En caso de seleccionar la opción 2 (dos) el programa solicita al usuario correo y contraseña para acceder a su cuenta, cabe aclarar que en caso de no tener una cuenta creada se recomienda primero crear una siguiendo los pasos de la opción 1 (uno) (de lo contrario el programa fallará impidiendo al usuario ejecutar cualquiera de las opciones que detallaremos a continuación, destacamos que en caso de continuar con el proyecto nuestra intención será corregir esas fallas para que el programa funcione de manera más fluida). En caso de que el cliente tenga un usuario creado entonces el programa pedirá los parámetros: correo y contraseña, que deberán ser cargados correctamente o no será posible el acceso a la cuenta (en caso de no cargar los datos correctamente podría fallar al ejecutar cualquiera de las siguientes funciones). Al acceder a la cuenta se ejecuta lo que denominamos como “Menú del usuario”, el cual estaremos detallando en el apartado “Menu del usuario”.

3_ Salir: Al seleccionar la opción 3 (tres) el programa detendrá su ejecución.

   Menú del usuario:
   
Este menú se ejecuta inmediatamente después que el cliente inicia la sesión, funciona muy similar al menú principal (se ofrecen opciones numeradas y el cliente debe ingresar un número de acuerdo a la opción que desea seleccionar) con la diferencia de que se ofrecen otras funcionalidades las cuales serán detalladas a continuación:

1_ Enviar Mensaje: Al ingresar el número 1 (uno) el programa solicitará al usuario la dirección de correo electrónico del destinatario, esta dirección debe pertenecer y coincidir de manera estricta a  la de un usuario existente en el programa (De lo contrario se imprimirá en pantalla la leyenda “Destinatario no encontrado” y seremos retornados al Menú del usuario). Una vez  ingresado el correo electrónico del destinatario de manera satisfactoria, se solicitará ingresar el asunto del mensaje y luego el contenido del mensaje, finalizada esta acción el mensaje será enviado y retornaremos inmediatamente al menú del usuario.

2_ Ver bandeja de entrada: Si se ingresa el número 2 (dos) el programa imprime los mensaje que hemos recibido (De no haber recibido ningún mensaje se imprime en pantalla “No hay mensajes”)  y nos retorna al menú del usuario. 

3_ Ver bandeja de salida: En caso de ingresar el número 3(tres) de forma muy similar a la opción 2 se nos muestra en pantalla los mensajes que hemos enviado.

4_ Salir: Al seleccionar la opción 4 (cuatro) regresamos al Menú principal.



<img width="1103" height="1008" alt="image" src="https://github.com/user-attachments/assets/1fad7e53-ddd1-4272-b501-e4dea8be2f46" />
