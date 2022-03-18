
<center>

# PACKET TRACERT II


</center>

***Nombre:*** Cristian M. Hdez Cruellas

***Curso:*** 1º de Ciclo Superior de Administración de Sistemas Informáticos en Red.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Conclusiones](#id5)


#### ***Introducción***. <a name="id1"></a>

 Utilizaremos el programa de packet tracert que es un programa que simula intalaciones de infracturas en red.  

#### ***Objetivos***. <a name="id2"></a>

En esta práctica realizaremos unos ejercicios de prácticos de packet tracert para comprender mejor su funcionamiento.

#### ***Material empleado***. <a name="id3"></a>

Utilizamos el programa de packet tracert. 

#### ***Desarrollo***. <a name="id4"></a>


***Ejercicio 5. Direccionamiento IP.***

Partiendo de una configuración de 3 switchs y 15 equipos, comprobar la comunicación 
entre los equipos mediante el uso de direcciones IP y máscaras.

***Paso 1.*** Insertar tres switchs 2950‐24 con los nombres SW01, SW02 y SW03, con la 
siguiente configuración:

| Switch origen |Puerto origen | Switch destino | Puerto destino |   |   |   |
|---------------|--------------|----------------|--------------|---|---|---|
| SW01| 2 | SW02 | 1          |                                   |   |   |   |
| SW01| 3 | SW03 | 1          |                                   |   |   |   |

***Paso 2.*** Insertar los 15 equipos con la siguiente configuración:

| Nombre | IP            | Máscara         | Switch | Puerto | último octeto | subredes | ip válidas                    | Pc al que se conecta          |
|--------|---------------|-----------------|--------|--------|---------------|----------|-------------------------------|-------------------------------|
| PC01   | 192.168.1.101 | 255.255.255.0   | SW01   | 11     | 00000000      | 1        | 192.168.1.1-192.168.1.254     | pc05,pc07,pc09,pc15           |
|  PC02  | 192.168.1.121 | 255.255.255.248 |  SW02  |   11   |    11111000   |    32    | 192.168.1.1-192.168.1.7       | Ninguno                       |
|        |               |                 |        |        |               |          | 192.168.1.9-192.168.1.15      |                               |
|        |               |                 |        |        |               |          | 192.168.1.17-192.168.1.23     |                               |
|        |               |                 |        |        |               |          | 192.168.1.25-192.168.1.31     |                               |
|        |               |                 |        |        |               |          | 193.168.1.33-192.168.1.39     |                               |
|        |               |                 |        |        |               |          | 192.168.1.41-192.168.1.47     |                               |
|        |               |                 |        |        |               |          | 192.168.1.49-192.168.1.55     |                               |
|        |               |                 |        |        |               |          | 192.168.1.57-192.168.1.63     |                               |
|        |               |                 |        |        |               |          | 192.168.1.65-192.168.1.71     |                               |
|        |               |                 |        |        |               |          | 192.168.1.73-192.168.1.79     |                               |
|        |               |                 |        |        |               |          | 192.168.1.81-192.168.1.87     |                               |
|        |               |                 |        |        |               |          | 192.168.1.89-192.168.1.95     |                               |
|        |               |                 |        |        |               |          | 192.168.1.97-192.168.1.103    |                               |
|        |               |                 |        |        |               |          | 192.168.1.105-192.168.1.111   |                               |
|        |               |                 |        |        |               |          | 192.168.1.113-192.168.1.119   |                               |
|        |               |                 |        |        |               |          | 192.168.1.121-192.168.1.127   |                               |
|        |               |                 |        |        |               |          | 192.168.1.129-192.168.1.135   |                               |
|        |               |                 |        |        |               |          | 192.168.1.137-192.168.1.143   |                               |
|        |               |                 |        |        |               |          | 192.168.1.145-192.168.1.151   |                               |
|        |               |                 |        |        |               |          | 192.168.1.153-192.168.1.159   |                               |
|        |               |                 |        |        |               |          | 192.168.1.161-192.168.1.167   |                               |
|        |               |                 |        |        |               |          | 192.168.1.169-192.168.1.175   |                               |
|        |               |                 |        |        |               |          | 192.168.1.177-192.168.1.183   |                               |
|        |               |                 |        |        |               |          | 192.168.1.185-192.168.1.191   |                               |
|        |               |                 |        |        |               |          | 192.168.1.193-192.168.1.199   |                               |
|        |               |                 |        |        |               |          | 192.168.1.201-192.168.207     |                               |
|        |               |                 |        |        |               |          | 192.168.1.209-192.168.1.215   |                               |
|        |               |                 |        |        |               |          | 192.168.1.217-192.168.1.223   |                               |
|        |               |                 |        |        |               |          | 192.168.1.1.225-192.168.1.231 |                               |
|        |               |                 |        |        |               |          | 192.168.1.233-192.168.1.239   |                               |
|        |               |                 |        |        |               |          | 192.168.1.241-192.168.1.247   |                               |
|        |               |                 |        |        |               |          | 192.168.1.249-192.168.1.254   |                               |
| PC03   | 192.168.1.140 | 255.255.255.192 | SW03   | 11     | 11000000      | 4        | 192.168.1.1-192.168.1.63      | pc04, pc11                    |
|        |               |                 |        |        |               |          | 192.168.1.65-192.168.1.127    |                               |
|        |               |                 |        |        |               |          | 192.168.1.129-192.168.1.191   |                               |
|        |               |                 |        |        |               |          | 192.168.1.193-192.168.1.254   |                               |
| PC04   | 192.168.1.160 | 255.255.255.128 | SW01   | 12     | 10000000      | 2        | 192.168.1.1-192.168.1.127     | pc03,pc09,pc10,pc11,pc16      |
|        |               |                 |        |        |               |          | 192.168.1.129-192.168.1.254   |                               |
| PC05   | 192.168.1.1   | 255.255.255.0   | SW02   | 12     | 00000000      | 1        | 192.168.1.1-192.168.1.254     | pc01,pc06,pc07,pc09,pc15      |
| PC06   | 192.168.1.11  | 255.255.255.224 | SW03   | 12     | 11100000      | 8        | 192.168.1.1-192.168.1.31      | pc05,pc13                     |
|        |               |                 |        |        |               |          | 192.168.1.33-192.168.1.63     |                               |
|        |               |                 |        |        |               |          | 192.168.1.65-192.168.1.95     |                               |
|        |               |                 |        |        |               |          | 192.168.1.96-192.168.1.127    |                               |
|        |               |                 |        |        |               |          | 192.168.1.129-192.168.1.159   |                               |
|        |               |                 |        |        |               |          | 192.168.1.161-192.168.1.191   |                               |
|        |               |                 |        |        |               |          | 192.168.1.193-192.168.1.224   |                               |
|        |               |                 |        |        |               |          | 192.168.1.225-192.168.1.254   |                               |
| PC07   | 192.168.1.111 | 255.255.255.128 | SW01   | 13     | 10000000      | 2        | 192.168.1.1-192.168.1.127     | pc13                          |
|        |               |                 |        |        |               |          | 192.168.1.1.-192.168.1.254    |                               |
| PC08   | 192.168.1.200 | 255.255.255.240 | SW02   | 13     | 11110000      | 16       | 192.168.1.1-192.168..1.15     | pc09                          |
|        |               |                 |        |        |               |          | 192.168.1.17-192.168.1.31     |                               |
|        |               |                 |        |        |               |          | 192.168.1.33-192.168.1.47     |                               |
|        |               |                 |        |        |               |          | 192.168.1.49-192.168.1.63     |                               |
|        |               |                 |        |        |               |          | 192.168.1.65-192.168.1.79     |                               |
|        |               |                 |        |        |               |          | 192.168.1.81-192.168.1.95     |                               |
|        |               |                 |        |        |               |          | 192.168.1.97-192.168.1.111    |                               |
|        |               |                 |        |        |               |          | 192.168.1.113-192.168.1.127   |                               |
|        |               |                 |        |        |               |          | 192.168.1.129-192.168.1.143   |                               |
|        |               |                 |        |        |               |          | 192.168.1.145-192.168.1.159   |                               |
|        |               |                 |        |        |               |          | 192.168.1.161-192.168.1.175   |                               |
|        |               |                 |        |        |               |          | 192.168.1.177-192.168.1.191   |                               |
|        |               |                 |        |        |               |          | 192.168.1.193-192.168.1.207   |                               |
|        |               |                 |        |        |               |          | 192.168.1.209-192.168.1.223   |                               |
|        |               |                 |        |        |               |          | 192.168.1.225-192.168.1.239   |                               |
|        |               |                 |        |        |               |          | 192.168.1.241-192.168.1.254   |                               |
| PC09   | 192.168.1.201 | 255.255.255.0   | SW03   | 13     | 00000000      | 1        | 192.168.1.1-192.168.1.254     | pc04,pc08,pc10,pc15           |
| PC10   | 192.168.1.248 | 255.255.255.128 | SW01   | 14     | 10000000      | 2        | 192.168.1.1-192.168.1.127     | pc04,pc09,pc15                |
|        |               |                 |        |        |               |          | 192.168.1.1.-192.168.1.254    |                               |
| PC11   | 192.168.1.144 | 255.255.255.192 | SW02   | 14     | 11000000      | 4        | 192.168.1.1-192.168.1.63      | pc03,pc04                     |
|        |               |                 |        |        |               |          | 192.168.1.65-192.168.1.127    |                               |
|        |               |                 |        |        |               |          | 192.168.1.129-192.168.1.191   |                               |
|        |               |                 |        |        |               |          | 192.168.1.193-192.168.1.254   |                               |
| PC12   | 192.168.1.211 | 255.255.255.240 | SW03   | 14     | 11110000      | 16       | 192.168.1.1-192.168..1.15     | pc15                          |
|        |               |                 |        |        |               |          | 192.168.1.17-192.168.1.31     |                               |
|        |               |                 |        |        |               |          | 192.168.1.33-192.168.1.47     |                               |
|        |               |                 |        |        |               |          | 192.168.1.49-192.168.1.63     |                               |
|        |               |                 |        |        |               |          | 192.168.1.65-192.168.1.79     |                               |
|        |               |                 |        |        |               |          | 192.168.1.81-192.168.1.95     |                               |
|        |               |                 |        |        |               |          | 192.168.1.97-192.168.1.111    |                               |
|        |               |                 |        |        |               |          | 192.168.1.113-192.168.1.127   |                               |
|        |               |                 |        |        |               |          | 192.168.1.129-192.168.1.143   |                               |
|        |               |                 |        |        |               |          | 192.168.1.145-192.168.1.159   |                               |
|        |               |                 |        |        |               |          | 192.168.1.161-192.168.1.175   |                               |
|        |               |                 |        |        |               |          | 192.168.1.177-192.168.1.191   |                               |
|        |               |                 |        |        |               |          | 192.168.1.193-192.168.1.207   |                               |
|        |               |                 |        |        |               |          | 192.168.1.209-192.168.1.223   |                               |
|        |               |                 |        |        |               |          | 192.168.1.225-192.168.1.239   |                               |
|        |               |                 |        |        |               |          | 192.168.1.241-192.168.1.254   |                               |
| PC13   | 192.168.1.25  | 255.255.255.128 | SW01   | 15     | 10000000      | 2        | 192.168.1.1-192.168.1.127     | pc07                          |
|        |               |                 |        |        |               |          | 192.168.1.1.-192.168.1.254    |                               |
| PC14   | 192.168.1.33  | 255.255.255.224 | SW02   | 15     | 11100000      | 8        | 192.168.1.1-192.168.1.31      |                               |
|        |               |                 |        |        |               |          | 192.168.1.33-192.168.1.63     |                               |
|        |               |                 |        |        |               |          | 192.168.1.65-192.168.1.95     |                               |
|        |               |                 |        |        |               |          | 192.168.1.96-192.168.1.127    |                               |
|        |               |                 |        |        |               |          | 192.168.1.129-192.168.1.159   |                               |
|        |               |                 |        |        |               |          | 192.168.1.161-192.168.1.191   |                               |
|        |               |                 |        |        |               |          | 192.168.1.193-192.168.1.224   |                               |
|        |               |                 |        |        |               |          | 192.168.1.225-192.168.1.254   |                               |
| PC15   | 192.168.1.222 | 255.255.255.0   | SW03   | 15     | 00000000      | 1        | 192.168.1.1-192.168.1.254     | pc01.pc04,pc05,pc09,pc10,pc12 |

#### ***Conclusiones***. <a name="id5"></a>

En esta parte debemos exponer las conclusiones que sacamos del desarrollo de la prácica.