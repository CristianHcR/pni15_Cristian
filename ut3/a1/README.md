
# UT3-A1 Ejercicios modelo OSI.


#### 1. ¿Qué niveles OSI son los niveles de soporte de red?
    
  - Los siguientes niveles o capas la capa/nivel 1: ***capa física,*** la capa/nivel 2:***capa de enlace de datos,*** la capa/nivel 3:***capa de red.***  
    
#### 2. ¿Qué niveles OSI son los niveles de soporte de usuario?
    
  - Los siguientes niveles o capas la capa/nivel 5: **capa sesión,** la capa/nivel 6: **la capa presentación** y la capa/nivel 7: **capa de aplicación.**
    
#### 3. ¿Cómo están OSI e ISO relacionadas entre sí?
    
   - **ISO** es la organización creadora del modelo de referencia **ISO.**
    
#### 4. Enumere los niveles del modelo OSI.
    
 - Se divide en los siguientes niveles:
 
  1.  Nivel físico.
  
  2.  Nivel de enlace de datos.
 
  3. Nivel de red.
 
  4. Nivel de transporte.
 
  5. Nivel de sesión.
 
  6. Nivel de presentación.
 
  7. Nivel de aplicación.
    
#### 5. ¿Cómo pasa la información de un nivel OSI al siguiente?
    
 - En lado del **emisor** este envía los datos de los niveles superiores a los inferiores y en cada nivel  se le añade a esos datos una cabecera propia del protocolo y en el lado del **receptor** ocurre lo mismo pero de forma inversa es decir, va desde los niveles inferiores a los superiores y en cada nivel se va retirando esa dicha cabecera.      
    
#### 6. ¿Qué son las cabeceras y cola y cómo se añaden y se quitan?
    
  - Las **cabeceras** y las **colas** son los datos que se añaden en cada uno de los niveles por los protocolos correspondientes. Se **añaden** según descienden los datos de nivel en el lado del emisor, y se **quitan** según van ascendiendo los niveles en el lado de receptor. 
    
#### 7. ¿Cuáles son las responsabilidades del nivel físico?
    
 - Este es el responsable de caracterizar los medios materiales/físico para la comunicación ya sean las placas, cables, conectores, etc.Se encarga de poner los bits en el medio de transmisión a lo largo de un canal de comunicación, de cuantos microsegundos dura un bit, y que voltaje representa un 1 y cuantos un 0.
    
#### 8. ¿Cuáles son las responsabilidades del nivel de enlace?
    
 - Este es responsable de la detección y correción de errores. También se encarga del direccionamiento físico y define una unidad de intercambio de datos la cual se conoce con el nombre de **Frame** o **Trama**.
    
#### 9. ¿Cuáles son las responsabilidades del nivel de red?
    
 - Este es el responsable del enrutamiento de los paquetes a través de la red interconectada de los routers, y define una unidad de intercambio de datos llamada **Paquete**. 
    
#### 10. ¿Cuáles son las responsabilidades del nivel de transporte?
    
  - Este es el reponsable de proveer comunicación entre las entidades finales, realizar control de flujo y define una unidad de intercambio de datos llamada **Segmento**.
    
#### 11. El nivel de transporte crea una conexión entre el origen y el destino. ¿Cuáles son los tres eventos involucrados en la conexión?
    
 - Establecimiento de la conexión.
 - Transferencia de datos.
 - Liberación de la conexión.
    
#### 12. ¿Cuál es la diferencia entre una dirección de punto en servicio, una dirección lógica y una dirección fisica?
    
- **Dirección en punto de servicio**: la cabecera del nivel de transporte debe además incluir un tipo de dirección denominado dirección de punto de servicio (o dirección de puerto).
- **Direccionamiento lógico**: el nivel de red añade una cabecera al paquete que viene del nivel superior que, entre otras cosas, incluye las direcciones lógicas del emisor y el receptor.
- **Direccionamiento físico**: el nivel de enlace de datos añade una cabecera a la trama para definir la dirección física del emisor (dirección fuente) y/o receptor (dirección destino) de la trama.
    
#### 13.¿Cuáles son las responsabilidades del nivel de sesión?
 
 - Este es el responsable de establecer, coordinar y terminar las conversaciones entre aplicaciones.
 
#### 14. ¿Cuáles son las responsabilidades del nivel de presentación?
    
- Este es el responsable de garantizar que la información que envía la capa de aplicación de un sistema pueda ser leída por la capa de aplicación de otro. De ser necesario, la capa de presentación traduce entre varios formatos de datos utilizando un formato común.
    
#### 15. ¿Cuál es el objetivo de la traducción en el nivel de presentación?
    
- EL objetivo es traducir la información dependiente del emisor a un formato común. 
    
#### 16. Indique alguno de los servicios proporcionados por el nivel de aplicación.
    
 - Algunos de los servicios que proporciona este nivel son el **correo electrónico**, **FTP**("*protcolo de transferencia de ficheros*"), **Telnet**("*Herramienta para arreglar fallos a distancia mediante un terminal*"),**Etc**  ..., etc.
    
#### 17. ¿Cómo se relacionan los niveles de la familia del protocolo TCP/IP con los niveles del modelo OSI?
    
 ![image](https://user-images.githubusercontent.com/90834685/138727455-007b9521-4e7f-4d31-855c-80c21feb6e0d.png)

#### 18. El nivel____________ decide la localización de los puntos de sincronización.

 transporte
 
 **sesión**
 
 presentación
 
 aplicación

#### 19. En el nivel _______________, la unidad de datos se denomina trama.

 físico
 
 **enlace de datos**
 
 red
 
 transporte

#### 20. Los servicios de correo y de directorio están disponibles a los usuarios de la red a través del nivel:

enlace de datos

sesión

transporte

**aplicación**

#### 21. A medida que los paquetes de datos se mueven  de los niveles inferiores a los superiores las cabeceras son:

añadidas

**eliminadas**

recolocadas

modificadas


