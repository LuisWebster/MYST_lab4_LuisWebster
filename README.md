# MYST_lab4_LuisWebster
Análisis Fundamental - Mercado FOREX USD/MXN

	Instrucciones Laboratorio 4
	(Análisis Fundamental en Mercado Forex)
	Elegir 1 indicador económico
		* Con volatilidad media o alta
			o Cuantificable
			o Descarga todo el archivo histórico de sus valores (desde la pagina FXStreet)
			o Para los siguientes pasos utiliza las últimas 36 observaciones.
		* Clasifica las observaciones de los comunicados según el siguiente criteritio
			o A Actual >= Consensus >= Previous
			o B Actual >= Consensus < Previous
			o C Actual < Consensus >= Previous
			o D Actual < Consensus < Previous
		* Descargar precios, en intervalos de 1min, de los 15 min antes y 15 min despues de cada ocasión en la que se hizo el comunicado del indicador económico. De tal manera que deberás de contar, para cada fecha en la que se comunicó el indicador, un data frame con 15 renglones anteriores (1 por cada periodo de 1 min con los precios OHLC), el renglon donde sucedió el comunicado, y 15 renglones posteriores.
	
	NOTA: Revisar 3 veces los Husos horarios y fechas.
		* Calcular 3 métricas para cada vez que sucede cada uno de los escenarios (tomando en cuenta todos los datos que recabaste).
			o Volatilidad en “Pips” Con precios de cierre
				* Desviación estándar de la diferencia de precios de cierre expresada en pips
			o Dirección de movimiento del precio, la diferencia entre el precio de cierre del primer periodo de 1 min antes del comunicado y el precio de cierre del último minuto.
			o Volatilidad en “Pips” calculada mediante la diferencia entre Máximo y Mínimo en la vela del comunicado.
