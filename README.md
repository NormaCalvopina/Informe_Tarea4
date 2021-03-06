# Informe_Tarea4

Nombre: Norma Calvopiña 

NRC: 4117

Resolución de ejercicios Capitulo 7 y 8 del Libro de Floyd (Octava edición)

### Circuitos en Serie-Paralelo (Capitulo 7)
### Teoremas de Circuitos y Conversiones (Capitulo 8)

### 1. OBJETIVOS


#### Objetivos Generales

Combinar el circuito en Serie y en Paralelo dentro del mismo circuito y aplicar los métodos de análisis aprendidos para circuitos en serie y circuitos en paralelo, además incluir el divisor de voltaje con carga resistiva, la red en escalera, y el puente Wheatstone

Conocer el concepto del método de superposición, teorema de Thévenin, Teorema de Norton, conversiones de fuente; para resolver los ejercicios planteados en los capítulo 7 y 8, además se deberá aplicar algunos métodos estudiados anteriormente para desarrollar correctamente cada problema.


#### Objetivos Específicos


- Analizar circuitos en serie-paralelo

- Identificar las relaciones serie-paralelo

- Analizar divisores de voltaje con carga 

- Determinar el efecto de carga de un voltímetro en un circuito 

- Realizar conversiones de fuente y aplicar el teorema de superposición al análisis de circuitos

-  Aplicar el teorema de Thévenin para simplificar un circuito para su análisis


### 2. MARCO TEORICO

## Circuitos en Serie-Paralelo (Capitulo 7)

![image](https://user-images.githubusercontent.com/105259381/176609928-f7613558-355d-43b8-990a-d96a8fa5387a.png)

#### REDES EN ESCALERA

Una red resistiva en escalera es un tipo especial de circuito en serie-paralelo. La red en escalera R/2R se utiliza comúnmente para reducir voltajes a ciertos valores ponderados para conversión de digital a analógica.
Se simplificar escalón por escalón, comenzando en el lado más alejado de la fuente. De este modo, se puede determinar la corriente en cualquier rama o el voltaje en cualquier nodo, como en el ejemplo:

![](https://github.com/NormaCalvopina/Informe_Tarea4/blob/main/fotos/Captura%20de%20pantalla%202022-06-28%20231705.png)

#### PUENTE DE WHEATSTONE

![](https://github.com/NormaCalvopina/Informe_Tarea4/blob/main/fotos/Captura%20de%20pantalla%202022-06-28%20233454.png)

#### PUENTE WHEATSTONE EQUILIBRADO

El puente Wheatstone se encuentra en la condición de puente equilibrado cuando el voltaje de salida (VSALIDA) entre las terminales A y B es igual a cero.

![](https://github.com/NormaCalvopina/Informe_Tarea4/blob/main/fotos/Captura%20de%20pantalla%202022-06-28%20233841.png)

Cuando el puente está equilibrado, los voltajes entre los extremos de R1 y R2 son iguales (V1=V2) y los voltajes entre los extremos de R3 y R4 son iguales (V3=V4)

![](https://github.com/NormaCalvopina/Informe_Tarea4/blob/main/fotos/Captura%20de%20pantalla%202022-06-28%20233925.png)

Sustituyendo V por IR de acuerdo con la ley de Ohm se obtiene

![](https://github.com/NormaCalvopina/Informe_Tarea4/blob/main/fotos/Captura%20de%20pantalla%202022-06-28%20234628.png)

Como I1=I3 e I2 = I4, todos los términos de corriente se cancelan, y permanecen las relaciones de resistor

![](https://github.com/NormaCalvopina/Informe_Tarea4/blob/main/fotos/Captura%20de%20pantalla%202022-06-28%20234641.png)

Se obtiene la siguiente fórmula que permite encontrar el valor del resistor R1 en función de los demás valores de resistor cuando el puente está equilibrado. También se puede encontrar el valor de cualquier otro resistor del mismo modo

![](https://github.com/NormaCalvopina/Informe_Tarea4/blob/main/fotos/Captura%20de%20pantalla%202022-06-28%20234656.png)

#### PUENTE WHEATSTONE DESEQUILIBRADO

![image](https://user-images.githubusercontent.com/105259381/176609759-308addb3-9151-4a8c-9e82-23675db2cef4.png)

#### Un circuito puente para medir temperatura

Si se va a medir temperatura, el transductor puede ser un termistor, el cual es sensible a la temperatura. La resistencia del termistor cambia de manera predecible a medida que cambia la temperatura. Un cambio de temperatura cambia la resistencia del termistor, lo que provoca un cambio correspondiente en el voltaje de salida del puente a medida que se desequilibra. El voltaje de salida es proporcional a la temperatura; por consiguiente, o un voltímetro conectado entre la salida puede ser calibrado para mostrar la temperatura o el voltaje de salida puede ser amplificado y convertido a forma digital para controlar en pantalla la visualización de la temperatura.

##  Teoremas de Circuitos y Conversiones (Capitulo 8)

Fuente de voltaje de CD

La fuente de voltaje de cd idealmente proporciona un voltaje constante a una carga, incluso cuando la resistencia de ésta varía.

La siguiente figura es el muy conocido símbolo empleado para identificar una fuente de voltaje de cd ideal.

![image](https://user-images.githubusercontent.com/105259381/176596588-78d7f4fd-cf11-4ab3-863a-af2412d709d9.png)

En realidad, ninguna fuente de voltaje es ideal; sin embargo, las fuentes de potencia regulada se aproximan a la situación ideal cuando funcionan dentro de la corriente de salida especificada.

#### Carga de la fuente de voltaje

Si RS es muy pequeño comparado con RL, la fuente se aproxima a la situación ideal porque casi todo el voltaje de fuente, VS, aparece entre los extremos de la resistencia más grande, RL. Muy poco voltaje actúa entre los extremos de la resistencia interna, RS. Si RL cambia, la mayor parte del voltaje de fuente permanece entre las terminales de salida en tanto RL sea mucho más grande que RS. Por consiguiente, ocurre un cambio muy pequeño en el voltaje de salida. Mientras más grande es RL, en comparación con RS, menos cambio ocurre en el voltaje de salida.

El voltaje de salida disminuye significativamente conforme la resistencia de la carga se reduce en comparación con la resistencia interna de la fuente.

#### Conversiones de Fuente

![image](https://user-images.githubusercontent.com/105259381/176610218-4a879337-66bd-41c2-ae42-69da5b0ca1e7.png)

#### Teorema de Superposición

En cualquier rama dada de un circuito con múltiples fuentes, la corriente puede calcularse al determinar en esa rama particular las corrientes producidas por cada fuente que actúa sola, con todas las demás fuentes reemplazadas por sus resistencias internas. La corriente total en la rama es la suma algebraica de las corrientes individuales presentes en dicha rama. 

![image](https://user-images.githubusercontent.com/105259381/176600566-207a1b15-4df5-4e58-9481-91b777419f1b.png)


![image](https://user-images.githubusercontent.com/105259381/176601225-24c17faf-f663-415b-a7ba-59c4f3a7a011.png)

![image](https://user-images.githubusercontent.com/105259381/176601542-d16276ae-9107-4ce4-9cfc-17d025a13409.png)

#### Teorema de Thevenin

El teorema de Thevenin proporciona un método para simplificar un circuito a una forma equivalente estándar. Se utiliza para hacer más sencillo el análisis de circuitos complejos.

En un circuito eléctrico, el voltaje equivalente de Thevenin (VTH) es el voltaje de circuito abierto (sin carga) presente entre dos terminales de salida. 
Cualquier componente conectado entre estas dos terminales “ve” efectivamente a VTH en seriecon RTH. Como lo define el teorema de Thevenin.

La resistencia equivalente de Thevenin (RTH) es la resistencia total que aparece entre dos terminales en un circuito dado que tiene todas las fuentes reemplazadas por sus resistencias internas.

Ejemplo de la simplificación de un circuito mediante el Teorema de Thevenin

![image](https://user-images.githubusercontent.com/105259381/176601966-003b438c-a7c9-4874-9a44-310a3bc9e66d.png)

![image](https://user-images.githubusercontent.com/105259381/176602002-861f1dbe-cbe6-4855-8095-03088b1d849e.png)

![image](https://user-images.githubusercontent.com/105259381/176602016-f142a259-b784-4a03-a6b3-45294928331b.png)

![image](https://user-images.githubusercontent.com/105259381/176604937-f97054ef-8e3f-4d5d-bd6b-bd632c4ea626.png)

![image](https://user-images.githubusercontent.com/105259381/176605823-3b315125-3a4c-44e9-9239-1bbcf1acbad4.png)

#### Teorema de Norton

Cualquier resistor de carga conectado entre las terminales de salida de un circuito equivalente Norton tendrá la misma corriente a través de él y el mismo voltaje entre sus terminales como si estuviera conectado a las terminales de salida del circuito original.

![image](https://user-images.githubusercontent.com/105259381/176606440-1436283d-1c29-4c8e-a8e4-40d43ea445ea.png)

#### Teorema de transferencia de potencia máxima 

Para una fuente de voltaje dada, la potencia máxima se transfiere desde una fuente hasta una carga cuando la resistencia de la carga es igual a la resistencia interna de la fuente.

#### Conversiones Delta a Y, y Y a Delta

![image](https://user-images.githubusercontent.com/105259381/176608228-847ce084-72d6-4a95-8437-a35d2cc1f7c9.png)


![image](https://user-images.githubusercontent.com/105259381/176607701-c5e5805f-ca9e-454c-8467-99e031158d22.png)


![image](https://user-images.githubusercontent.com/105259381/176609523-24218135-382f-4003-8b8d-6243e574387c.png)


### 3. EXPLICACIÓN O RESOLUCIÓN DE EJERCICIOS O PROBLEMAS

## Resolución de los ejercicios Capítulo 7 

#### SECCION 7-1 Identificación de relaciones en serie-paralelo

2. Visualice y trace los siguientes circuitos en serie-paralelo:

(a) Una combinación en paralelo de tres ramas, cada rama con dos resistores en serie

![image](https://user-images.githubusercontent.com/105259381/176611231-78fcaf2d-0c1a-4937-ad7a-5dd45a506a5f.png)

(b) Una combinación serie de tres circuitos en paralelo, cada circuito con dos resistores

![image](https://user-images.githubusercontent.com/105259381/176611603-05db50c5-9e1b-4853-bec5-449f609a4079.png)

4. En cada uno de los circuitos de la figura 7-63, identifique las relaciones en serie-paralelo de las resistencias vistas desde la fuente.

![image](https://user-images.githubusercontent.com/105259381/176612088-7480cc9b-e69c-463b-882f-f12b5f4b02e5.png)

![image](https://user-images.githubusercontent.com/105259381/176613060-c20e1a3f-49ba-4239-9c1a-9f308a34ede9.png)

6. Desarrolle un diagrama esquemático de la tarjeta de circuito impreso de doble cara mostrada en la figura 7-65, y marque los valores de resistor.

![image](https://user-images.githubusercontent.com/105259381/176613437-72030207-f51a-4bc7-996d-2c174526c150.png)

![image](https://user-images.githubusercontent.com/105259381/176614145-3e1f19da-b87e-42cb-b068-7bd30d204ebf.png)

####  SECCIÓN 7–2 Análisis de circuitos resistivos en serie-paralelo

8. Un cierto circuito se compone de dos resistores en paralelo. La resistencia total es de 667 Ω. Uno de los resistores es de 1.0kΩ. ¿Cuál es el otro resistor?

![image](https://user-images.githubusercontent.com/105259381/176615761-44157d4f-bfd3-4069-9e4f-897177fb7b0b.png)

10. Repita el problema 9 para cada uno de los circuitos mostrados en la figura 7-63.

![image](https://user-images.githubusercontent.com/105259381/176615824-87fff8d4-8a13-402b-9473-8504e6ba3046.png)

![image](https://user-images.githubusercontent.com/105259381/176615849-163c7019-c8f2-43b3-a6e0-b90e30e2eb81.png)


12. Determine la corriente a través de cada resistor en cada circuito de la figura 7-63; luego calcule cada caída de voltaje.

![image](https://user-images.githubusercontent.com/105259381/176615919-c2c0d73c-adc6-4a96-9c8e-03c9c8cf5b88.png)

Para el literal a 

![image](https://user-images.githubusercontent.com/105259381/176616018-4930071e-0ce7-407c-8717-544f07ec9089.png)

Para el literal b

![image](https://user-images.githubusercontent.com/105259381/176616078-9d4119b0-63e2-455d-8211-7f22d4130fad.png)

Para el literal c

![image](https://user-images.githubusercontent.com/105259381/176616127-547a4e59-fc2b-47c2-a684-c46da2e31d3b.png)

14. Determine la resistencia entre A y B en la figura 7-67 sin la fuente.

![image](https://user-images.githubusercontent.com/105259381/176616589-8d494842-28cd-4c0f-9eea-62bb80779842.png)

El 1,8 kΩ y los dos 1 kΩ están en cortocircuito.

16. Determine el voltaje en cada nodo con respecto a tierra en la figura 7-68.

![image](https://user-images.githubusercontent.com/105259381/176618330-0a50289e-28d9-42da-a730-2f7d2047dfb8.png)

![image](https://user-images.githubusercontent.com/105259381/176618375-417071da-d77e-4dc9-a0d3-2e9ec5006049.png)

18. Determine la resistencia del circuito mostrado en la figura 7-67 como se ve desde la fuente de voltaje

![image](https://user-images.githubusercontent.com/105259381/176619009-02df0916-8a86-4798-a2b3-5d3e078fb481.png)

20. Determine el voltaje, VAB, en la figura 7-69.

![image](https://user-images.githubusercontent.com/105259381/176619738-5eee6374-93b0-4b2a-8694-44059a984213.png)

Resistencia de la rama derecha 

![image](https://user-images.githubusercontent.com/105259381/176619785-bfb4e09f-2ddc-4aad-97a0-f0c4f9d25af0.png)

Resistencia de la rama izquierda

![image](https://user-images.githubusercontent.com/105259381/176619967-fca7f09c-241c-44e4-aa41-8baaa1829549.png)

Resistencia total y Corriente total

![image](https://user-images.githubusercontent.com/105259381/176620041-5c556f95-6ac3-4aa3-8e64-fca199fb969b.png)

Corriente de rama izquierda y derecha 

![image](https://user-images.githubusercontent.com/105259381/176620084-efd9d414-32c3-4839-8db3-c81551e34d63.png)

22. En la figura 7-71, determine la resistencia entre el nodo A y cada uno de los demás nodos (RAB, RAC, RAD, RAE, RAF, y RAG).

![image](https://user-images.githubusercontent.com/105259381/176620934-a9f2ffbd-4852-407f-9d30-ada87b34de1f.png)

![image](https://user-images.githubusercontent.com/105259381/176620988-ceaed8cf-575e-4c35-a78a-e86620c053cd.png)

24. Determine el valor de cada resistor mostrado en la figura 7-73

![image](https://user-images.githubusercontent.com/105259381/176621364-d0372e20-1b23-41d9-aed0-b7df37a999d0.png)

![image](https://user-images.githubusercontent.com/105259381/176621406-8d8e7d12-d4a9-4671-b356-f8c45f849920.png)

![image](https://user-images.githubusercontent.com/105259381/176621442-90a55555-b521-41bd-9863-bd2345839595.png)

#### SECCIÓN 7–3 Divisores de voltaje con cargas resistivas

26. La salida de una batería de 12 V se divide para obtener dos voltajes de salida. Se utilizan tres resistores de 3.3 kΩ para proporcionar dos tomas. Determine los voltajes de salida. Si se conecta una carga de 10 kΩ a la más alta de las salidas, ¿cuál será su valor con carga?

![image](https://user-images.githubusercontent.com/105259381/176623173-121830b7-c28a-4a1a-b6d3-3a9a1719431e.png)

Con una resistencia de 10KΩconectada desde la toma A a tierra:

![image](https://user-images.githubusercontent.com/105259381/176623413-87e827a0-f3e5-407d-90db-fbc8baa72dfb.png)

28. En la figura 7-74, determine el voltaje de salida sin carga entre las terminales de salida. Con una carga de 100 kΩ conectada de A a B, ¿cuál es el voltaje de salida?

![image](https://user-images.githubusercontent.com/105259381/176623830-d0593b59-53c3-426a-8bff-6777d309a8e2.png)

![image](https://user-images.githubusercontent.com/105259381/176819473-2005e659-20ef-4808-89be-e5a56d482334.png)


30. En la figura 7-74, determine la corriente continua extraída de la fuente sin carga entre las terminales de salida. Con una carga de 33 kΩ, ¿cuál es la corriente extraída?

![image](https://user-images.githubusercontent.com/105259381/176623777-49b7b531-81c2-409b-8158-215342980dcb.png)

![image](https://user-images.githubusercontent.com/105259381/176624013-63ebaae0-f5b9-4f6a-9394-25fdb0f671be.png)


32. El divisor de voltaje de la figura 7-75 tiene una carga controlada por interruptor. Determine el voltaje en cada toma (V1, V2 y V3) para cada posición del interruptor

![image](https://user-images.githubusercontent.com/105259381/176624547-18e7f612-51c3-48ba-96fa-a9c2c6e33cbf.png)

![image](https://user-images.githubusercontent.com/105259381/176624496-ff567f3f-b795-4aef-ad3f-f2575b814408.png)

34. Diseñe un divisor de voltaje que produzca una salida de 6 V sin carga y un mínimo de 5.5 V entre los extremos de una carga de 1.0 kΩ . El voltaje de fuente es de 24 V y la corriente extraída sin carga no debe exceder de 100 mA.

![image](https://user-images.githubusercontent.com/105259381/176624945-acd5e0f7-e55f-43c6-9674-9f462e8bd154.png)

#### SECCIÓN 7–4 Efecto de carga de un voltímetro

36. Determine la resistencia interna de un voltímetro de 20,000 kΩ /V en cada uno de los siguientes ajustes de intervalo

![image](https://user-images.githubusercontent.com/105259381/176724415-4ddfe9fb-8272-4f15-828c-b1e86b1f5793.png)

38. Repita el problema 37 si se utiliza el voltímetro para medir voltaje entre los extremos de R4 en el circuito de la figura 7-62(b).

![image](https://user-images.githubusercontent.com/105259381/176718452-43c168eb-0d2c-46c6-aefa-d2ad66416da7.png)

#### SECCIÓN 7–5 Redes en escalera

40. Determine la resistencia total y el voltaje en los nodos A, B y C de la red en escalera mostrada en la figura 7-78.

![image](https://user-images.githubusercontent.com/105259381/176718753-172dcb4d-1d2d-4ff3-81e6-524adb91e848.png)

![image](https://user-images.githubusercontent.com/105259381/176720878-43b4c290-6406-418c-81b7-94cc63493e9f.png)

![image](https://user-images.githubusercontent.com/105259381/176720969-86e32a5f-1d48-4ddd-9c14-3e844cef101b.png)

42. En la figura 7-79, ¿cuál es el voltaje entre los extremos de cada resistor con 10 V entre A y B?

![image](https://user-images.githubusercontent.com/105259381/176721986-31874bca-d2c4-4934-b0bd-65bc63667478.png)

Las corrientes se calcularon en el literal 41 

![image](https://user-images.githubusercontent.com/105259381/176722106-5c178400-cca6-41e1-82a4-39be636cc285.png)

44. Determine VSALIDA para la red R/2R en escalera mostrada en la figura 7-81 para las siguientes condiciones: 

![image](https://user-images.githubusercontent.com/105259381/176722855-b610e497-5169-4702-968f-ec9d4acae681.png)

(a) Interruptor SW2 conectado a +12 V y los demás conectados a tierra

![image](https://user-images.githubusercontent.com/105259381/176723522-9c7c8efb-83af-4f7b-9cfb-4715a02dafb5.png)

(b) Interruptor SW1 conectado a +12 V y los demás conectados a tierra

![image](https://user-images.githubusercontent.com/105259381/176723637-e00f162d-3f22-49f7-8def-feb0cb5c2d67.png)

#### SECCIÓN 7–6 El puente Wheatstone

46. Se conecta un resistor de valor desconocido a un circuito puente Wheatstone. Los parámetros del puente en equilibrio se establecen como sigue: RV   18  y R2/R4   0.02. ¿Cuál es Rx?

![image](https://user-images.githubusercontent.com/105259381/176734890-291f8615-1db8-4b03-bdb0-09b962a12356.png)


48. Determine el voltaje de salida para el puente desequilibrado mostrado en la figura 7-83 a una temperatura de 60°C. La característica de resistencia según la temperatura del termistor se muestra en la figura 7-60.

![image](https://user-images.githubusercontent.com/105259381/176735054-012fb96d-e133-496b-9375-112f4231ab84.png)

![image](https://user-images.githubusercontent.com/105259381/176744549-2588d188-71af-4c87-b317-93f06ba9efb7.png)

![image](https://user-images.githubusercontent.com/105259381/176745174-04be7fef-05a7-43ae-9cbe-49fdd73773ac.png)

#### SECCIÓN 7–7 Localización de fallas

50. ¿Son correctas las lecturas del medidor mostrado en la figura 7-85?

![image](https://user-images.githubusercontent.com/105259381/176745759-5e286ae5-6acb-45fe-9577-6be75734862e.png)

Se vuelve a dibujar el circuito:

![image](https://user-images.githubusercontent.com/105259381/176775162-68e6d4be-dbb5-40f6-b64c-e8dec0ab14cc.png)

![image](https://user-images.githubusercontent.com/105259381/176775360-fa346be7-00a3-404d-88fe-95802944338e.png)

52. Vea los medidores ilustrados en la figura 7-87 y determine si hay una falla en el circuito. Si la hay, identifíquela.


![image](https://user-images.githubusercontent.com/105259381/176778450-c6fd7e3e-e8b3-47bb-8f5b-e2139a9c26ba.png)

![image](https://user-images.githubusercontent.com/105259381/176778418-e1ae5d6c-8e6a-492c-a681-44cd1dd7e3a5.png)

![image](https://user-images.githubusercontent.com/105259381/176784747-c0b62a56-96aa-48b6-8af1-aa3fd6566b65.png)


54. Si en la figura 7-89 R2 se abre, ¿qué voltajes se leerán en los puntos A, B y C?

![image](https://user-images.githubusercontent.com/105259381/176789361-b03968a1-8533-40d7-9480-580c8e065201.png)

Si R2 se abre, VA=15V. VB=0V Y VC=0V


## Resolución de los ejercicios Capítulo 8

#### SECCIÓN 8–3 Conversiones de fuente

2. Convierta las fuentes de voltaje prácticas de la figura 8-67 en fuentes de corriente equivalentes

![image](https://user-images.githubusercontent.com/105259381/176789936-ac6a2d8b-448b-4063-874b-3186dd2ce3a6.png)

![image](https://user-images.githubusercontent.com/105259381/176790511-144ca3b8-f17e-4b81-a4c7-9a05f3a7dba3.png)

4. Trace los circuitos equivalentes de fuentes de voltaje y corriente para la batería tipo D del problema 3

![image](https://user-images.githubusercontent.com/105259381/176792264-a3a0bbce-2077-4ca2-90c7-0656aba672e0.png)

6. Convierta las fuentes de corriente prácticas de la figura 8-68 en fuentes de voltaje equivalentes.

![image](https://user-images.githubusercontent.com/105259381/176792421-c0bbc8a3-a1bc-4b8c-8fd0-a5967760f915.png)

![image](https://user-images.githubusercontent.com/105259381/176792485-4bfa182e-c2cc-41cf-9d32-9fdb8920c15a.png)

#### SECCIÓN 8–4 El teorema de superposición

8. Use el teorema de superposición para determinar la corriente a través, y el voltaje entre, los extremos de la rama R2 de la figura 8-69.

![image](https://user-images.githubusercontent.com/105259381/176793709-2dec8b24-fa32-458d-9b1c-30d78fc0e43c.png)

![image](https://user-images.githubusercontent.com/105259381/176793879-af7cb275-51e9-4ffd-8a5a-abfa575640ca.png)


10. Con el teorema de superposición, determine la corriente de carga en cada uno de los circuitos mostrados en la figura 8-71.

![image](https://user-images.githubusercontent.com/105259381/176796556-547ab8e1-c74d-4e30-8440-6a990cbd7f7d.png)

![image](https://user-images.githubusercontent.com/105259381/176796530-c876cd67-6d7d-4784-acc8-11d0a0a79b9b.png)

![image](https://user-images.githubusercontent.com/105259381/176798663-c636ce5d-286d-493a-aeef-677c7c906a59.png)

![image](https://user-images.githubusercontent.com/105259381/176798687-9060f051-368b-4f13-967c-f9806416c70e.png)

![image](https://user-images.githubusercontent.com/105259381/176798705-c0c8d39f-a42b-495e-af6d-d6320e30bf1c.png)


12. Repita el problema 11 si R2 es de 10 kΩ.

![image](https://user-images.githubusercontent.com/105259381/176798863-d535792f-03ee-40e7-bff1-e21906a1731c.png)

14. Los interruptores mostrados en la figura 8-74 se cierran en secuencia, SW1 primero. Determine la corriente a través de R4 después del cierre de cada interruptor

![image](https://user-images.githubusercontent.com/105259381/176799274-95692d2b-55c5-4162-85a9-7b9bceeb1817.png)

![image](https://user-images.githubusercontent.com/105259381/176800483-18da8b06-ef57-494b-8a1e-da3d3b4955b5.png)

SW1 Cerrado:

![image](https://user-images.githubusercontent.com/105259381/176800521-d523a0b3-2466-40c0-83b5-1df24970a793.png)


SW1 Y SW2 Cerrados 

![image](https://user-images.githubusercontent.com/105259381/176800601-e4a83985-7231-46b1-976c-ea9bb5bd8b8e.png)

![image](https://user-images.githubusercontent.com/105259381/176800618-2028a301-eb24-48dd-8109-f19777b80971.png)

SW1 Y SW2 Y SW3 Cerrados

![image](https://user-images.githubusercontent.com/105259381/176800684-d1179f6e-9942-473c-a93f-376845c14f38.png)

#### SECCIÓN 8–5 Teorema de Thevenin

16. Para cada uno de los circuitos de la figura 8-76, determine el equivalente de Thevenin como se ve desde las terminales A y B.

![image](https://user-images.githubusercontent.com/105259381/176800757-95553012-fce7-4889-a0a0-898328cec34f.png)

Para el circuito a

![image](https://user-images.githubusercontent.com/105259381/176800814-9144973a-3c1a-4274-afcb-ac1e97395b5e.png)

Para el circuito b

![image](https://user-images.githubusercontent.com/105259381/176800882-6008bad7-0fbb-4ec8-861a-407049b856b9.png)

Para el circuito c

![image](https://user-images.githubusercontent.com/105259381/176800926-800e6b7f-426d-405f-a65c-6b1ea77f08e9.png)


Para el circuito d

![image](https://user-images.githubusercontent.com/105259381/176800948-94bb8b6c-e6fb-40fa-a55c-ad53f11613e0.png)


18. Con el teorema de Thevenin, determine el voltaje entre los extremos de R4 en la figura 8-78

![image](https://user-images.githubusercontent.com/105259381/176800972-2a24275d-8b7e-4994-b833-a898bcadc449.png)

Abro la fuente de corriente (hacer cero), elimino R4 y dibujo el circuito

![image](https://user-images.githubusercontent.com/105259381/176803580-a14581b6-f069-4ac6-af1c-3c9ed507ee4b.png)


Determino V1 debido a la fuente de 50V usando el circuito de Thevenin y realizo el dibujo del circuito:

![image](https://user-images.githubusercontent.com/105259381/176803598-62ec5393-cb40-4bca-af02-fd2148ebe983.png)


Hago cero la fuente de voltaje y elimino R4 y realizo el circuito.

![image](https://user-images.githubusercontent.com/105259381/176803633-24e748ae-1835-462c-b1a3-e75bece96fcf.png)


Obtengo V4 debido a la fuente de corriente usando el circuito de Thevenin

![image](https://user-images.githubusercontent.com/105259381/176803661-377225c1-cf88-41ab-8fff-13867c2ecab6.png)


Mediante el método de superposición se combina los voltajes de V4 y obtengo el voltaje total de R4:

![image](https://user-images.githubusercontent.com/105259381/176803692-9443b6f5-9b55-4c6c-940b-5222033c5ab1.png)

20. Determine la corriente que se dirige al punto A cuando R8 es de 1.0 kΩ, 5 kΩ, y 10 kΩ en la figura 8-80.

![image](https://user-images.githubusercontent.com/105259381/176803746-c18be273-20cb-4a6e-bb25-027c3ac78871.png)

![image](https://user-images.githubusercontent.com/105259381/176804226-8b2c245d-245e-4ca8-81a9-0878005efe4b.png)

Para determinar VTH vuelvo a dibujar el circuito:

![image](https://user-images.githubusercontent.com/105259381/176804249-5660ea83-312c-48a3-a810-b1639747ad92.png)


El circuito de Thévenin como se dibujó, la corriente en el punto A se determina para el valor de R8.

![image](https://user-images.githubusercontent.com/105259381/176804267-e16ce23d-0f82-448a-b8d6-65abaf70e141.png)

Para R8=1kΩ:

![image](https://user-images.githubusercontent.com/105259381/176804316-7773314a-4f80-4139-8fc6-c3cd3efcd58c.png)

Para R8=5kΩ:

![image](https://user-images.githubusercontent.com/105259381/176804405-856b94ed-b610-4e60-b016-b94918365719.png)

Para R8=10kΩ:

![image](https://user-images.githubusercontent.com/105259381/176804420-a0749a0a-4669-4abd-a4a5-ec93aacaa8fe.png)

22. Determine el equivalente de Thevenin del circuito mostrado en la figura 8-82 visto desde las terminales A y B.

![image](https://user-images.githubusercontent.com/105259381/176804525-952fd9fb-01ba-4358-9009-ceb5632ada24.png)

![image](https://user-images.githubusercontent.com/105259381/176804635-a40696d9-505f-495a-982d-7f03f8d1dbb6.png)

#### SECCIÓN 8–6 Teorema de Norton

24. Con el teorema de Norton, determine la corriente que circula a través del resistor de carga RL en la figura 8-77.

![image](https://user-images.githubusercontent.com/105259381/176804713-620eeda2-f964-4199-9051-ae73bb57f253.png)


Simplifico el circuito 

![image](https://user-images.githubusercontent.com/105259381/176804799-5e8f30c0-ee0b-4963-bbab-369e6ad7aebc.png)

![image](https://user-images.githubusercontent.com/105259381/176805107-f9f02a33-c33d-4ef1-ab91-240cc738875a.png)

![image](https://user-images.githubusercontent.com/105259381/176805140-84fec7f0-323f-4241-a5dd-a0762d1bb549.png)


26. Con el teorema de Norton, determine la corriente que circula a través de R1 en la figura 8-80 cuando R8= 8 kΩ

![image](https://user-images.githubusercontent.com/105259381/176811705-8bd5bf2a-9d94-443c-8555-ccc089b10558.png)


![image](https://user-images.githubusercontent.com/105259381/176811415-07ba0bd1-f6b2-419b-b6f5-23f7a8710b0b.png)

![image](https://user-images.githubusercontent.com/105259381/176811436-2d06d2e4-d6a8-4e50-a0ed-7e20f1115521.png)

![image](https://user-images.githubusercontent.com/105259381/176811463-0d5f59ac-7fbb-4414-90e7-59cc4a1b9fe8.png)


28. En la figura 8-83, reduzca el circuito entre las terminales A y B a su equivalente Norton.

![image](https://user-images.githubusercontent.com/105259381/176811764-11f845b5-7a47-4205-8ea3-5e202f1d2a79.png)

![image](https://user-images.githubusercontent.com/105259381/176812531-d0b599a7-21d0-40b9-ab06-b85ced96ef40.png)


![image](https://user-images.githubusercontent.com/105259381/176812557-1c1e4bad-b2fc-4579-a8d4-5c100f4fe3de.png)


#### SECCIÓN 8–7 Teorema de transferencia de potencia máxima

30. En cada circuito mostrado en la figura 8-85, se tiene que transferir potencia máxima a la carga RL. Determine el valor apropiado de RL en cada caso.

![image](https://user-images.githubusercontent.com/105259381/176812617-c99ce397-5c52-4f15-abe8-be3886295928.png)

![image](https://user-images.githubusercontent.com/105259381/176812728-f0e7e5ef-0156-4e30-a0cb-48cfb4ce915c.png)


32. ¿Cuánta potencia se suministra a la carga cuando RL es un 10% más alta que su valor para transferencia de potencia máxima en el circuito de la figura 8-86? 

![image](https://user-images.githubusercontent.com/105259381/176812791-20b7c54b-6aa2-40c3-9eb8-b714c4ba5986.png)

![image](https://user-images.githubusercontent.com/105259381/176814123-1a0b1403-3d43-4bf5-b97c-0f018a1683cf.png)

![image](https://user-images.githubusercontent.com/105259381/176814152-9591878b-dad1-4b14-a3e6-7cc9e39b66db.png)


#### SECCIÓN 8–8 Conversiones delta a Y, y Y a delta

34. En la figura 8-88, convierta cada red delta en una red Y

![image](https://user-images.githubusercontent.com/105259381/176814300-119c5c47-cfd7-46bb-b92b-b6005dc1fe30.png)


36. Determine todas las corrientes que circulan en el circuito de la figura 8-90.

![image](https://user-images.githubusercontent.com/105259381/176814343-e01ea20e-e066-4184-bcb3-69c458ce4e6d.png)

Se convierte delta formado por R3, R4 y R5 en una configuracion de estrella

![image](https://user-images.githubusercontent.com/105259381/176814363-3d83a8b4-72e7-4755-96ab-83b8e51d4884.png)


![image](https://user-images.githubusercontent.com/105259381/176814386-04dfc48b-7e6c-4a3d-9a89-d84b1f01a431.png)


![image](https://user-images.githubusercontent.com/105259381/176814416-25b8d2a8-01e4-4aca-a25d-2aa88a2fc4f3.png)

### 4. CONCLUSIONES:

-El teorema de superposición nos ayudó a abordar circuitos que tienen múltiples fuentes. Los teoremas de Thévenin y de Norton son métodos apropiados que nos ayudan a reducir un circuito a una forma equivalente simple con el propósito de facilitar su análisis.

-El teorema de transferencia de potencia máxima sirve para aplicaciones donde es importante que un circuito dado proporcione potencia máxima a una carga. Como se vio en los ejercicios y se aplicó el teorema, un ejemplo de esto es un amplificador de audio que suministra potencia máxima a un altavoz.

-Las conversiones de fuente dentro de los circuitos son de dos tipos, el primero la conversión de una fuente de voltaje en una fuente de corriente, en este caso se deberá dividir el voltaje de la fuente entre la resistencia interna de la fuente que por lo general es igual a cero.

-Para realizar un análisis correcto de un circuito serie- paralelo se debe primero identificar y diferenciar las partes del circuito que se encuentran en paralelo y las que se encuentran en serie, luego se debe aplicar los conocimientos adquiridos en capítulos anteriores para calcular la resistencia, corriente y voltaje totales. 

### 5. VIDEO:

https://youtu.be/HxwKHnsOq9Q

### 6. BIBLIOGRAFÍA:

Floyd, TL (2007). Principios de circuitos electricos. Monterrey: Pearson Educación.




