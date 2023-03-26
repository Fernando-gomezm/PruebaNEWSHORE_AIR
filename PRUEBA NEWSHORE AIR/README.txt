La siguiente dirección es la correspondiente al API de la prueba, 
(https://localhost:5001/api/vuelos/BusquedaVuelos/) para realizar la consulta 
se debe ingresar EJ: MDE/CTG después del último slash, lo que se tomaría como
origen y destino, en ese mismo orden.

El puerto de localhost puede variar dependiendo el ordenador, este se mostrará 
en un símbolo del sistema después de abrir el ejecutable.

Estos serían trayectos que se pueden consultar teniendo en cuenta el API consumida:
	- MZL/MDE
	- MZL/CTG
	- PEI/BOG
	- CTG/CAN
	- BOG/MAD
	- BOG/MEX




PROBLEMAS RESUELTOS:

1 - Modelado de clases:
	Se realizó el modelamiento correspondiente a como se indicaba en el 
	instructivo, con sus llamadas entre los objetos modelados.

2 - Consumo REST API:
	Se consume satisfactoriamente la API proporcionada en el instructivo, 
	para posteriormente darle uso en las consultas.

3 - Obtener Ruta:
	Al ingresar el origen y destino en la ruta del API, se puede obtener
	la información correspondiente a dicha consulta. EJ:
	
	https://localhost:5001/api/vuelos/BusquedaVuelos/MDE/CTG

	Al usar la anterior dirección, se obtiene como respuesta:

	{
    	 "id": 0,
    	 "origin": "MDE",
    	 "destination": "CTG",
    	 "price": 200,
    	 "flights": [
        	{
            	 "id": 0,
            	 "origin": "MDE",
            	 "destination": "CTG",
            	 "price": 200,
            	 "transport": {
                		"id": 0,
                		"flightCarrier": "CO",
                		"flightNumber": "8009"
            		}
        	}
    	    ]
	}


PROBLEMAS SIN SOLUCIONAR:
4 - Persistencia/Acceso Datos