FORMAT: 1A
HOST: http://polls.apiblueprint.org/

# Custodia

Esta es la documentaci�n y dise�o de la API referente al proceso de custodia de ejemplo para la actividad 16. Esta API tiene como finalidad registrar los cr�ditos, l�neas de cr�dito y tarjetas de cr�dito en la base de datos del sistema de custodia.

## Cr�ditos [/creditos]

### Ingresar cr�dito [POST /creditos]

Permite registrar un cr�dito en el sistema de custodia.

+ Request (application/json)

        {
            "Cr�dito": [
                 "idCredito": 3,
                 "idCliente": 2,
                 "montoCredito": 18500000,
                 "moneda": "CLP"
            ]
        }

+ Response 201 (application/json)

    + Body

            {
               "estado": true,
               "resultado": "Cr�dito almacenado correctamente."
            }

## L�neas de cr�dito [/lineascredito]

### Ingresar l�nea de cr�dito [POST /lineascredito]

Permite registrar una l�nea de cr�dito en el sistema de custodia.

+ Request (application/json)

        {
            "L�nea_Cr�dito": [
                 "idLinea": 1,
                 "idCliente": 2,
                 "montoLinea": 50000000,
                 "moneda": "CLP"
            ]
        }

+ Response 201 (application/json)

    + Body

            {
               "estado": true,
               "resultado": "L�nea de cr�dito almacenada correctamente."
            }

## Tarjetas de cr�dito [/tarjetascredito]

### Ingresar tarjeta de cr�dito [POST /tarjetascredito]

Permite registrar una tarjeta de cr�dito en el sistema de custodia.

+ Request (application/json)

        {
            "Tarjeta_Cr�dito": [
                 "idTarjeta": 1,
                 "idCliente": 2,
                 "montoApertura1": 50000000,
                 "moneda1": "CLP",
                 "montoApertura2": 0,
                 "moneda2": "USD"
            ]
        }

+ Response 201 (application/json)

    + Body

            {  
               "estado": true,
               "resultado": "Tarjeta de cr�dito almacenada correctamente."
            }

