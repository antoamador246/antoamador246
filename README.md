Algoritmo hotel
	escribir "bienvenido al hotel los dos carnanes"
	Escribir "sabemos que tenia munchas mas opciones para venir a mazatlan y estamos encantados que haya elijido nuestro hotel para hospedarse. esperamos que se lleve una buena impresion de nuestro hotel"
	escribir "cuantos dias se hospedara en este hotel"
	leer num_dias 
	escribir "en este mes tenemos distintos descuentos dependiendo de la habitacion que desee"
	escribir "seleccione que tipo de habitacion desea"
	escribir "1-habitacion sencilla cuenta con un 5% de descuento y cuenta con acceso al bufet una vez al dia"
	escribir"2-habitacion matrimonial cuenta con un 15% de descuento y tiene incluido bufet para dos personas una vez al dia"
	escribir"3-habitacion de doble recamara matrimonial cuenta con 20% de descuento, tiene vista al mar y acceso a alberca y acceso a el bufet para cuatro personas una vez al dia"
	escribir"4-suite cuenta con un 25% de descuento, acceso a desayuno y al bufet, cuenta con balcon privado con vista al mar y acceso a la alberca"
	Repetir
		Leer hab
		Si hab<1 O hab>4 Entonces
				Escribir Sin Saltar "no contamos con este tipo de habitaciones"
			FinSi
	Hasta Que hab>=1 Y hab<=4
	Si hab=1 Entonces
		precio=400
		subtotal=400*.5
		subtotal_1=400-subtotal
	FinSi
    Si hab = 2 Entonces
        precio=500
		subtotal=500*.15
		ALGORITMO DE UN HOTEL:
    subtotal_1=500-subtotal
    FinSi
    Si hab = 3 Entonces
        precio=550
		subtotal=550*.20
		subtotal_1=550-subtotal
	fin si 
	Si hab=4 Entonces
		precio=900
		subtotal=900*.25
		subtotal_1=900-subtotal
	Fin Si
	Si num_dias>1 o num_dias<5 Entonces
		subtotal_2=subtotal_1*.5
		subtotal_2=subtotal_1-subtotal_2
	SiNo
		Si um_dias>6 o num_dias<8  Entonces
			subtotal_2=subtotal_1*.8
			subtotal_2=subtotal_1-subtotal_2
		SiNo
			Si um_dias>9 o num_dias<12 Entonces
				subtotal_2=subtotal_1*.15
				subtotal_2=subtotal_1-subtotal_2
			SiNo
				
			Fin Si
		Fin Si
	Fin Si
	total=num_dias*subtotal_2
    Escribir "precio: " precio
	Escribir "descuento: " subtotal_2
    Escribir "total: " total 
FinAlgoritmo
Este en un algoritmo para la reservacio de un hotel  para tener un mejor controo del hotel
