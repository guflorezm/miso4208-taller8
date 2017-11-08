# miso4208-taller8
Repositorio Taller 8 MISO-4208

## Ejecución Netflix SimianArmy

Se realizaron doce ejecuciones de los monkeys, de las cuales dos lograron terminar instancias EC2 con el chaos monkey

A continuación se anexan imagenes de la traza que generó la terminación de la instancia

![chaosMonkeytraza](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/traza-chaos1.png)

Se anexan imagenes de la consola de AWS para las instancias terminadas

![AWSchaosMonkey1](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/consola-aws-chaos1.png)

![AWSchaosMonkey2](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/consola-aws-chaos2.png)

Se anexan imagenes del API REST del chaos monkey 

![APIRESTchaosJSON1](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/api-rest-chaos-json.png)

![APIRESTchaosJSON2](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/api-rest-chaos-json2.png)

![APIRESTchaosDatos](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/api-rest-chaos-datos.png)

![APIRESTchaosCabecera](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/api-rest-chaos-cabecera.png)

Se anexa imagen del correo recibido por un chaos monkey

![chaosMonkeyMail](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/chaos-mail1.png)

En las ejecuciones en que chaos monkey no terminó instancias por lo regular se dieron normalmente y casi siempre las trazas, consola de AWS y correos lucian de la siguiente forma

![janitorTraza](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/traza-janitor1.png)

![consolaAWSconformity](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/consola-aws-conformity.png)

![APIRESTJanitor](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/api-rest-janitor.png)

![conformityMail](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/conformity-mail1.png)

## Trazas

En el siguiente enlace se pueden observar las trazas de las ejecuciones

https://github.com/guflorezm/miso4208-taller8/tree/master/trazas-ejecucion

## Correos

En el siguiente enlace se pueden observar los correos recibidos de las ejecuciones agrupados por monkey

https://github.com/guflorezm/miso4208-taller8/tree/master/correos

## Propiedades 

En el siguiente enlace se pueden observar los archivos de configuracion de propiedades de los monkeys

https://github.com/guflorezm/miso4208-taller8/tree/master/properties

Se hicieron cambios en algunas propiedades como:

simianarmy.scheduler.frequency = 1

Se cambió la frecuencia a 2, 3 y 4 y se dejaron ejecutando por 2 horas pero siempre lo realizaba una vez, al parecer no tiene efecto la frecuencia y tambien se cambió en cada uno de los archivos de propiedades de los monkeys

simianarmy.aws.email.region=us-west-2

simianarmy.chaos.notification.sourceEmail = gerflomo@gmail.com

simianarmy.chaos.notification.global.receiverEmail = gu.florez@uniandes.edu.co

simianarmy.calendar.isMonkeyTime = true

simianarmy.conformity.summaryEmail.to = gu.florez@uniandes.edu.co

simianarmy.conformity.notification.sourceEmail = gerflomo@gmail.com

simianarmy.conformity.cluster.monkey-target.ownerEmail = gu.florez@uniandes.edu.co

simianarmy.janitor.enabled = true

simianarmy.janitor.notification.sourceEmail = gerflomo@gmail.com

simianarmy.janitor.summaryEmail.to = gu.florez@uniandes.edu.co

Se modificó la policy del usuario SimianArmy de AWS para agregarle el permiso de DeleteAttributes por un error que generaba el conformity monkey

![policyAWS](https://github.com/guflorezm/miso4208-taller8/blob/master/imagenes/policy-aws.png)

## Reporte descripción monkeys

En el siguiente enlace se puede observar el PDF del reporte de descripción de los monkeys 

https://github.com/guflorezm/miso4208-taller8/blob/master/reporte-descripcion/SimianArmy-Descripcion%20Monkeys.pdf












