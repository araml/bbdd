# Preguntas final de bbdd

## 13/10/15


1. [Qué es una transacción?](#1-qué-es-una-transacción)
2. [Qué es el problema de falsa  sumarización y cómo lo soluciona el locking binario?](#2-cuál-es-el-problema-de-la-falsa-sumarización-y-cómo-lo-soluciona-el-locking-binario)
3. [~~Qué es la Consistencia Eventual?~~ Ver propiedades BASE #189](#189-decir-qué-son-las-propiedades-base)
4. Qué datos almacena el System  Catalog sobre las Foreign Keys?  
5. Dar una restricción de integridad  referencial y mostrar cómo se la asegurar en el Modelo Relacional.  
6. Dadas las transacciones T1 =  {R1(A),R1(B),W1(B),W1(A)}, T2 = {R1(A), W1(A)}. Dar un historial  serial y otro serializable (pero no serial) [Venía con trampa]    
7. Definir lo qué es el Data mining y dar dos utilidades.    
8. Nombrar dos componentes del DBMS y  explicar para qué sirven.    
9. Qué permisos pueden concederse  sobre las tablas?    
10. Cómo puede comprobarse que una  dependencia funcional X->Y no puede inferirse dee un conjunto de dependencias F?   
11. Dado un sistema que tiene una  caída y usa un log con actualizaciones inmediatas. Si antes del fallo se tienen las siguientes tres transacciones:  
    1. T1 escribe y commitea   
    2. T2 solo lee    
    3. T3 escribe pero no commitea   
    4. Indicar qué transacciones deben hacer UNDO, cuáles REDO y cuáles nada para recuperar el sistema.  
12. Dar dos casos distintos donde el optimizador de consultas elija hacer un Full Scan.    
13. Cuál es la diferencia entre los índices clustered y  unclustered?


## 04/08/14

14. ¿Qué es el rollback de una transacción? (1 punto)    
15. Dos diferencias y similitudes entre lockeo optimista y pesimista (2 puntos)  
16. [~~Qué es el problema de falsa sumarización (2 puntos)~~ Ver pregunta 2](#2-cuál-es-el-problema-de-la-falsa-sumarización-y-cómo-lo-soluciona-el-locking-binario)
16. Demuestre que X define funcionalmente a Y si y sólo si Y  pertenece a la clausura de X (3 puntos)  
17. {NROPEDIDO, CODART, NOMART, CANTPEDIDO, PRECIO, CODEMP,  NOMEMP, FECHA}. (1.5 puntos)    
    1. Dar una dependencia funcional total.    
    2. Dar una dependencia funcional parcial.    
    3. Dar una dependencia funcional transitiva.
18. ¿Qué es el dominio de un atributo? Dar un ejemplo. (1 punto)   
De un ejemplo de una relción binaria. (1 punto)   
19. ¿Qué 3 datos es necesario mantener en el catálogo para  optimizar por costos? ¿Cuál es su utilidad? (2 puntos)   
20. ¿Qué es la seguridad independiente de una base de datos? (1 punto) 
21. Una transacción no llega a hacer commit. Trabaja con  actualización inmediata. ¿Cómo queda la base de datos después?  (como estaban antes de la transacción / como están después / no  se puede saber). (2 puntos)   
22. ¿Qué se utiliza del system catalog a la hora de validar una query? (2 puntos)  
23. ¿Qué es el clustering? De dos problemas a donde se aplique. (2 puntos)  
24. ¿Por qué es importante para un DBA saber cómo va a creecer una tabla? (1 punto)

## 11/04/14

26. Defina la durabilidad de una transacción y dé un ejemplo  donde se aplique esta propiedad.  
28. Dado el siguiente conjunto de operaciones T1 = {R1(A);R1(D);W1(A);W1(D)} T2={R2(A);W2(A)}. Indique el schedule  serial correspondiente yuno serializable (no serial).  
28. [~~Falsa sumarización. Como resuelve este problema el lockeo binario?~~ Ver pregunta 2](#2-cuál-es-el-problema-de-la-falsa-sumarización-y-cómo-lo-soluciona-el-locking-binario)
29. Suponga la siguiente relacion {CODEMP, TEL1, TEL2, TEL3}. En  qué forma normal se encuentra? Justifique  
29. Como puede probarse que una dep. funcional es falsa en un cierto conjunto de DFs? 
30. Defina clave primaria. Que operaciones de DML controla esta restricción?   
32. Defina independencia lógica y explique como se vincula con los niveles de arqutectura de las BDs.   
33. Cual es el costo de acceder a buscar un rango de valores si se tiene un indice hash que aplica al criterio de busqueda?  
34. Como pueden utilizarse las vistas para aumentar la seguridad de la BD?   
35. Se tiene una BD con actualizacion inmediata (undo/redo).  Muestre un grafico en que situación tenia que estar T2 para que el  dbms tuviera que hacer undo 
36. Dos usos que le da el compilador al System Catalog.   
37. Que es un Data Warehouse? Cual es su utilidad?   
38. Porque es necesario para un DBA conocer la forma en que se van a incrementar los registros de una tabla?


## 06/03/14

39. T1 efectúa lectura sucia sobre un valor de T2. Luego se hace rollback de T2 y la Base de Datos fuerza rollback de T1. ¿Qué  propiedad de las transacciones se aplicó para forzar rollback de T1? (2 puntos)   
40. T1: {R1(A),W1(A),R1(B),W1(B)} T2: {R2(A),W2(A)}. Dar H  serial y una serializable (Que no sea serial) (2 puntos)   
41. [~~Explique problema de actualización perdida. ¿Cómo resuelve este problema el lockeo binario? (2 puntos)~~ Ver #81](#81-explicar-detalladamente-el-problema-de-falsa-actualización-como-fue-una-traducción-espantosa-dio-la-posibilidad-de-elegir-entre-lost-update-o-dirty-read)
42. ¿Cuándo dos conjuntos de dependencias funcionales son  equivalentes? (1 punto) 
43. Sea la relación R: {codigoDepto,nroAmbiente,codigoBarrio,descripcionBarrio,largoAmbiente,anchoAmbiente}  Dar una dependencia funcional transitiva, una parcial, una total. Indicar cuál es la clave de la relación. (3 puntos)    
44. Defina la operación de project de álgebra relacional. ¿Cómo se traduce en un SQL esta operación? (1.5 puntos)   
45. Mencione dos componentes del DBMS y explique su funcionamiento. (2 puntos)  
46. Mencione y ejemplifique dos heurísticas que utiliza el optimizador de consultas. (2 puntos)   
47. Mencione dos permisos existentes sobre los usuarios de una Base de Datos. (1 punto)    
48. Se tiene Base de Datos con update diferido. Muestre gráfico en qué situación tenía que estar T2 para que el DBMS tuviera que  hacer redo. (2 puntos)  
49. Indique tres datos referidos a las tablas se guarda en el  System Catalog. (1.5 puntos)  
50. Mencione algoritmo de aprendizaje supervisado y explique  brevemente su objetivo. (2 puntos).   
51. Indique tres usos que la Base de Datos le da al System  Catalog (1.5 puntos)

## 26/12/13

52. De un ejemplo que involucre mas de una instruccion SQL donde  sea necesario utilizar una transacción. (1 punto)   
53. Describa detalladamente dos pruebas que haria sobre un  sistema para comprobar detalladamente el funcionamiento del lockeo. (2 puntos)   
54. Definicion de forma normal de Boyce Codd. (1 punto)   
55. Definicion de dependencia funcional parcial. De un ejemplo. (1 punto)   
56. Definir clave foranea. ¿Qué operaciones de SQL controlan esta restriccion? (2 puntos)   
57. ¿Cual es la diferencia entre una agregación y una relacion ternaria? (2 puntos)   
58. ¿Cuando un indice se llama secundario? (1 punto)   
59. ¿Como pueden utilizarse los stored procedures para aumentar  la seguridad de una base de datos? ¿Por que? (2 puntos)   
60. ¿Cual es la diferencia entre Commit y Checkpoint? (1.5 puntos)   
61. Detalle el uso que le da el DBMS al System Catalog en el  momento de hacer un insert en una tabla. (2 puntos)   
62. ¿Cuales son las formas clasicas que tienen los modelos de DW? (2 puntos)   
63. ¿Que es una dimension en el modelo de un DW? (2 puntos)   
64. Mencione y explique dos parametros que necesita conocer el DBA sobre una tabla a la hora de crearla. (1 punto)   
65. ¿Cuales son los niveles de aislamiento de SQL? ¿Qué  problema de control de concurrencia resuelve cada uno? (2 puntos) 
66. ¿Qué es una descomposicion de una relacion? ¿Cuando es la  misma sin pérdidas de dependencias funcionales? (2 puntos)   
67. ¿Cual es el costo de acceder por igualdad en una consulta  si se tiene un indice B+ Clustered que aplica al criterio de  busqueda? Expliquelo. (2 puntos)

## 13/09/13

68. ¿Que es la seguridad integrada de una BD?  
69. ¿Que es DDL? De un ejemplo de una instrucción SQL de este grupo
70. Muestre dos usos que el compilador DDL le da al system catalog  
71. De dos similitudes y dos diferencias entre lockeo binario y  shared lock  
72. De dos similitudes y dos diferencias entre lockeo pesimista y optimista
72. T1 commiteo, T2 solo leyo, T3 escribio pero no llego a commitear. ¿Que hay que hacer con c/u (undo, redo o nada)?   
73. ¿Para que le sirve a un DBA conocer la cantidad inicial de  registros de una tabla?
74. ¿Que es data mining? Dar dos aplicaciones de estas técnicas   
75. Demostrar que X --> Y <=> Y es subconjunto de X+   
76. Dar dos propiedades algebraicas sobre la selección que  sirvan en la optimizac 
77. Nombre las 4 operaciones básicas de las transacciones  
78. ¿Que es una relación en el contexto de la teoría relacional? Ejemplifique.  
79. ¿Que es un cubrimiento minimal de un conjunto de  dependencias? ¿Que utilidad tiene?  


## 06/08/13  
80. Qué es el system log? Para qué se utiliza?  
81. [Explicar detalladamente el problema de falsa actualización (como fue una traducción espantosa dio la posibilidad de elegir entre lost update o dirty read)](#81-explicar-detalladamente-el-problema-de-falsa-actualización-como-fue-una-traducción-espantosa-dio-la-posibilidad-de-elegir-entre-lost-update-o-dirty-read)
82. Cuando un schedule es recuperable?  
83. Enunciar las reglas adicionales de amstrong  
84. Cuando se dice que una descomposición es sin pérdida de información? Dar un ejemplo de descomposición con pérdida  
85. Definir la operación de proyección del álgebra relacional y dar 2 propiedades   
86. Qué es DML? Dar un ejemplo de instrucción SQL de esta  categoría  
87. Dar 2 reglas de Álgebra relacional que involucren al JOIN  que puedan usarse para optimización de consultas  
88. Qué permisos pueden asignarse en una tabla?  
89. El enunciado era muy largo pero esencialmente preguntaba sobre qué puede asegurarse si tenemos undo/redo, la base se cae y una transacción no hizo commit acerca de los datos en disco, si quedan los viejos, los nuevos, no puede asegurarse nada  
90. Qué instrucciones DDL actualizan el system catalog?   
91. Qué es clustering? Dar 2 ejemplos de uso donde pueda aplicarse  
92. Dar 2 ventajas y desventajas en el uso de stored procedures

## 30/07/13

93. Defina detalladamente el problema de la falsa sumarizacion (2 puntos)   
94. Defina equivalencia de dos transaccions (1? punto)
95. Dada la siguiente relación {NROPEDIDO; CODART, NOMART,  CANTPEDIDA, PRECIO, CODEMP. NOMEMP., FECHA}. Indicar:   
    1. Una dependencia funcional completa     
    2. Una dependencia funcional parcial.     
    3. Una dependencia funcional transitiva.( 1.5 puntos)   
96. ¿Que es un plan de ejecucion?(1)   
97. Defina super clave y cual es la diferencia con la clave candidata(?)   
98. De dos restricciones que modelen cosas del mundo real que haya en el modelo de entidad relacion y como se implementan en la base (2 puntos)  
99. Defina lo que es un select en algebra relacional y de 2 propiedades (1? puntos) 
100. Algo con GRANT (1 punto)
101. ¿Cómo se recupera la BD con undo/redo?(2 puntos) 
102. Instruccion para actualizar el catalog(1 punto)
103. 2 operaciones que se realice(o haga, no me acuerdo bien la palabra) el DW ( algo asi era la pregunta, no me la acuerdo bien, yo  lo defini lo que era un DW y para que se usaba y me puso 0/2  puntos)(2 puntos)  
104. ¿Por qué el DBA tiene que conocer el crecimiento de la base?(1 punto)

## 11/04/12

105. Defina la durabilidad de una transacción y de un ejemplo donde se aplique esta propiedad (1 punto)  
106. [Defina grafo de precedencia y enuncie el teorema de  serializabilidad. Por qué es importante este teorema en el control de concurrencia?(2.5 puntos)](#106-defina-grafo-de-precedencia-y-enuncie-el-teorema-de--serializabilidad-por-qué-es-importante-este-teorema-en-el-control-de-concurrencia)
107. Indique y explique dos diferencias entre el lockeo binario y  el shared-lock ( o lockeo ternario).(2 puntos)  
108. Defina la clausura de un atributo. Escriba la definición de  clave candidata en función de la clausura.(1.5 puntos)  
109. Dada la siguiente relación  {NROPEDIDO; CODART, NOMART, CANTPEDIDA, PRECIO, CODEMP. NOMEMP.,  FECHA}. Indicar: (1.5 puntos) 
110. Una dependencia funcional  completa    
111. Una dependencia funcional  parcial.      
112. Una dependencia funcional transitiva.  Ej 17.
113. Cuál es la diferencia entre una clave primaria y un índice único? (1 punto) 
114. Indique los tres niveles que tiene la arquitectura de una base de datos. jemplifique (1.5 puntos).  
115. Mencione dos reglas del álgebra relacional que toma en cuenta la optimización por reglas. Ejemplifique su uso (2 puntos)   
116. De un ejemplo de cómo funciona el recovery en el caso de una caída abrupta de la base de datos por un corte de luz si la  misma utiliza redo logging? (2 puntos)
117. Detalle el uso que el DBMS le da al system catalog en el momento de crear una tabla (1 punto) 
118. ¿Por qué es necesario para un DBA conocer la cantidad de  registros que inicialmente va a tener una tabla? (1 punto)    
119. ¿Cuándo una entidad se considera débil? De un ejemplo (1.5  puntos)  
  
## 13/12/19  

120. Enunciar los métodos para resolver un JOIN y explicar uno  de ellos.  
121. Mencione y explique dos diferencias entre OLTP y OLAP.  
122. ¿Cuáles son las 3 "Vs" de Big Data? Explicarlas brevemente.  
123. ¿Cuándo se dice que una transacción "lee" de  otra? ¿Cómo se relaciona con la recuperabilidad de los schedules?  
124. ¿Cuándo se utilizan las entidades débiles en un DER? Dar  un ejemplo.  
125. Diferencia entre integración de datos e intercambio de  datos.  
126. ¿Cuál es la principal diferencia entre el DBA y el  administrador de datos? 
127. ¿Qué es el gobierno de datos? ¿Cómo se relaciona con la  calidad de datos?
128. Explicar la UNDO rule. ¿Por qué es importante?  
129. ¿Qué optimizaciones puede hacer una base de datos paralela al recibir una query?  
130. ¿Cuándo se dice que una base de datos distribuida es  homogénea?    
131. ¿Cuál es la función del scheduler?  
132. Mencione un nivel de aislamiento de SQL para transacciones.  ¿Qué implica? 
133. ¿Cuáles son los permisos que se le puede asignar a un  usuario sobre una tabla de la base de datos?   
134. [¿Qué es el teorema CAP?](#134-qué-es-el-teorema-cap)  
135. ¿Qué propiedades debe cumplir un conjunto de atributos  para ser una clave candidata?    
136. ¿Qué propiedades son deseables en una descomposición de  una relación?  
137. ¿Una relación que está en 2FN está también en 3FN?  Justificar.  
138. Enunciar los axiomas de Armstrong.

## 17/07/19

139. ¿Cuándo una historia es completa?  
140. ¿Cuándo se dice que una transacción lee de otra? ¿Cómo  se relaciona esto con la recuperabilidad de los schedules?  
141. Enunciar la Undo Rule y la Redo Rule.  
142. Dar dos similitudes y dos diferencias entre las propiedades  de las transacciones en bases de datos relacionales y no-SQL.  
143. Mostrar un ejemplo donde un chequeo de integridad podría  provocar el rollback de una transacción. ¿Cón qué propiedad de  las transacciones se relaciona?  
144. Dar los dos modelos existentes de Open Data y describir  brevemente cada uno de ellos.  
145. ¿Puede una superclave no ser clave candidata? Justificar.  
146. ¿Puede la clausura de un conjunto de atributos ser el  conjunto vacío?  
147. ¿Cuándo se dice que una descomposición de una relación  es sin pérdida de información?  
148. Mencionar dos heurísticas que puede aplicar el optimizador  de queries. 
149. Dar los dos modelos más comunes para una base de datos de  tipo Data Warehouse. Describirlos brevemente.    
150. ¿Cuándo se dice que una transacción es distribuida?
151. ¿Qué tipos de paralelismo puede aplicar un motor de bases  de datos distribuidas al resolver una query?  
152. ¿Qué es un índice hash? Describir su estructura física.  
153. ¿Cuántas formas distintas existen de pasar un DER a un  modelo relacional?  
154. ¿Qué es un administrador de datos?  
155. ¿Cuál es la diferencia entre integración de datos e  intercambio de datos?
156. ¿Qué es una ontología?

## 12/18

157. {idEmpleado, nombreEmpleado, nroDepto, costoDepto}  ¿Dependencias fucionales? ¿En que FN está?    
158. CK vs SK    
159. 2NF vs 3NF    
160. 2 atributos => 3NF    
161. Explicar una db no-sql y ejemplificar.    
162. ¿Qué es una BD distribuída? Enumerar condiciones que debe  cumplir.
163. Fragmentación horizontal. ¿Qué es? Armar la tabla usando  AR.  
164. Historia serial vs serializable    
165. Comparar índice denso vs no denso en términos de  almacenamiento físico. 
166. Explicar Ehrenfeucht–Fraïssé    
167. Nombre 2 propiedades de AR que sean usadas para optimización  
168. Que garantiza la independencia física?  

## 06/12/18

169. Dos heurísticas de optimización y ejemplos
170. Data Warehouse vs bases relacionales, diferencias
171. Una query dónde no se pueda usar INLJ (no se pueda usar el join que usa índices, sin importar que estructuras tengas)
172. Diferencias entre Select de SQL y selección de álgebra relacional
173. Dame un ejemplo de una agregación
174. Una historia donde se produzca un abort, pero que se evite si se usa control multiversion
175. Dar dos tipos de control de concurrencia y compararlos (ventajas y desventajas)
176. [~~Para que sirve el grafo de seriabililidad y como se construye.~~ Ver #106](#106-defina-grafo-de-precedencia-y-enuncie-el-teorema-de--serializabilidad-por-qué-es-importante-este-teorema-en-el-control-de-concurrencia)
177. ¿Qué es un algoritmo de clustering?
178. ¿Qué es un administrador de datos?
179. Diferencia entre 3FN y BCNF
180. Diferencia entre consistencia en relacionales y NoSQL
181. ¿Qué es el Quantifier Rank?
182. ¿Qué es Open Data? Dar los dos tipos de ... [no sé qué]
183. Diferencias entre optimización de querys en bases de datos paralelas y distribuidas
184. Dar un ejemplo de uso de extensiones orientadas a objetos que proveen las bases de datos (tipos de datos custom objetosos)
185. ¿Que es una superclave?
186. Te daba una relación y tenías que dar una clave (superclave) que no sea clave candidata

## 01/08/17

187. Definir clausura con dependencias funcionales. Dar el algoritmo para calcular la clausura
188. Decir en qué caso CRT no es igual al álgebra relacional.
189. [Decir qué son las propiedades BASE.](#189-decir-qué-son-las-propiedades-base)
190. Qué es Data Mining y para qué se usa.
191. ¿Qué son las bases distribuidas de sitio primario? Dar ventajas y desventajas.
192. ¿Que es una agregación? Dar un ejemplo.
193. Definir la fórmula de búsqueda en rango para B+ clustered.
194. Si tengo una relación con 2 atributos, ¿puede pasar que no esté en 3FN? Justificar.
195. ¿Qué es base de datos Stream? Dar un ejemplo.
196. ¿Qué usa Ehrenfreucht-Fraissé para explicar el poder de expresividad de la lógica de 1er orden?
197. Definir el problema de lost update y dar un ejemplo.
198. ¿Qué son las réplicas 2P2 en bases de datos distribuídas? Dar ventajas y desventajas.

## 15/05/17
 
199. Describir la fórmula de la cantidad resultante de tuplas en la búsqueda por rango.
200. Describir qué ocurre al realizarse un read con un sistema de control de concurrencia por timestamp y por multi-versión.
201. Existe una relación de inclusión entre clave primaria, clave candidata y superclave? Justifique.
202. Cuándo se puede decir que una BD distribuida es homogénea?
203. Dada la siguiente relación {númeroEmpleado, nombreEmpleado, númeroDepartamento, costoDepartamento}, qué dependencias funcionales son válidas? Decir en qué forma normal se encuentra la relación.
204. Mencionar dos mecanismos de limpieza de datos.
205. Cómo serían las historias que un mecanismo de control de concurrencia entregaría si se quisiera cumplir estrictamente con la condición de aislamiento?
206. Cuál es la diferencia entre agregación e interrelación ternaria? Justifique.
207. [Describa brevemente las bases de datos orientadas a grafos.](#207-describa-brevemente-las-bases-de-datos-orientadas-a-grafos)
208. Dar una heurística de optimización y las propiedades algebraicas que se utilizan para aplicarla.
209. Qué diferencia existe entre una historia serial y una serializable? Ejemplifique.
210. Que garantiza la independencia física de las bases de datos?
211. Cuál es la diferencia respecto a almacenamiento físico entre un índice denso y uno no denso?

## 25/04/17

212. Una clave candidata es siempre una superclave?
213. Definir dependencia funcional.
214. Dada R = {A, B, C, D}, A es clave primaria, y además se tiene A->C, B->D. En qué forma normal está R?
215. Qué es un índice no denso? Ejemplifique.
216. Explicar el concepto de fragmentación mixta.
217. Explicar la fórmula que calcula el costo de encontrar un valor utilizando un índice non clustered?
218. Cómo asegura el control de concurrencia por timestamping multiversión la recuperabilidad?
218. Dar una historia ACA que no sea serial.
220. Con qué propiedad de las transacciones está relacionada la necesidad de evitar rollbacks en cascada?
221. Enunciar las leyes de Armstrong.
222. Dar dos propiedades del álgebra relacional que se puedan utilizar en optimización de consultas. Ejemplifique.
223. Qué es un DER? Para qué se utiliza?
224. Dar una extensión del modelo relacional con objetos. Ejemplificar.

## 02/03/17

225. Clave candidata en funcion de la clausura
226. diferencia entre relacion e interrelacion
227. ejercicio practico donde te daba la relacion y te pedia que des un ejemplo de una descomposion con perdida de informacion. Justificar
228. Funcionamiento de un indice primaro (decia otra cosa, yo interprete eso, el otro que rindio interpreto indice denso).
229. Que es un administrador de datos y dos diferencias con un DBA.
230. Costo del indice hash.
231. Que es un scheduler ACA y dar ejemplo
232. Porque el DBA admite scheduler ACA?
233. [Bases NO-SQL porque se dicen 'schemaless?
     Ejemplificar.](#233-bases-no-sql-porque-se-dicen-schemaless-ejemplificar)
234. Explicar bases de datos distribuidas homogeneas.
235. Que pasos se realizan en multiversion cuando llega un read(x)
236. 2 heuristicas de optimizacion. Ejempliique.
237. Cuando se dice que una transaccion lee de otra.
238. Algoritmos no supervisados. Ejemplifique.

## 24/02/17

239. Definir clave candidata en términos de clausuras de dependencias funcionales
240. Definir cubrimiento minimal
241. Sea R=(A,B,C,D) AB es clave primaria, A -> C y B -> D son dependencias funcionales, en qué forma normal se encuentra? Justifique
242. Que es un índice denso
243. Cuál es el costo de acceder a un índice hash
244. Defina historia serializable y dé un ejemplo de una que lo sea.
245. Por qué es importante que una historia sea serializable?
246. Defina consistencia eventual.
247. En una base distribuida, que significa que sea homogénea?
248. En un control de concurrencia multiversion, qué controles suceden cuando se ejecuta read(x)
249. De al menos dos optimizaciones de querys
250. Qué significa que una transacción lea de otra? Dé un ejemplo
251. Defina qué es agregación
252. Dé alguna extension de objetos en las bases relacionales, ejemplifique.

## ?/12/16

253. Diferencia entre FNBC y 3FN
254. Sea R=(numEmpkeado, nombre Empleado, numDepto, nomDepto) hacer una descomposición que no sea SPI. Y justificar
255. Diferencia entre índice primario y secundario
256. Que es un índice no denso(hacer ejemplo)
257. Explicar que es una long duration transaction
258. Que es la consistencia eventual y la diferencia con la tradicional
259. Dar dos capacidades de las bases de datos geográficas
260. Explicar un ejemplo de un atributo identificatorio
261. Que es un plan de ejecución
262. Dos diferencias y dos similitudes entre lock binario y concurrencia de control multiversion
263. Explicar project en álgebra relacional. Dar un ejemplo y una sentencia SQL
264. Diferencia entre checkpoint quiescente y no quiescente
265. Cuando dos operaciones son conflictivas
266. Cuando un atributo no está en clausura de otro

## 2023-03-10
267. Que es una agregación? Dar un ejemplo
268. cuánto vale T', si busco A=a
269. Que es una base de datos stream?
270. que son los algoritmos supervisados y no supervisados
271. Que es data mesh. Cuáles son sus 4 principios. Explicarlos.
272. Que es Open data? Dar las dos definiciones ( aquí la idea era explicar cómo se hizo conocido en América latina y en Europa)

# Respuestas

## 13/10/15

### 1. ¿Qué es una transacción?
Una transacción es un conjunto de instrucciones que se ejecutan formando una unidad lógica de procesamiento. En criollo todas las instrucciones dentro de la transacción ocurren como si fuese un conjunto atómico.

**Formalmente** una transacción es un conjunto de operaciones {read/write/abort/commit} sobre un conjunto de data items tal que forman una relación de ordenamiento < cumpliendo las siguientes propiedades
1. Si hay un abort no hay un commit y si no hay un commit hay un abort
2.  Si hay un abort o commit entonces cualquier operación < abort/commit
3. Si hay un write o un read entonces read < write ó write < read.

### 2. ¿Cuál es el problema de la falsa sumarización y cómo lo soluciona el locking binario?

El problema de la **falsa sumarización** ocurre cuando hay una transacción modificando varios data items y otra se mete en el medio haciendo una sumarización y obteniendo un resultado erróneo. Por ejemplo considerar las siguientes transacciones (X = 0, y = 100):

	r1(x), t1(x += 100), w1(x), t2(sum = 0), r2(x), t2(sum += x), r2(y), t2(sum += y),
    t1(y -= 100), r1(y)

Esperaríamos que sum sea 100 pero en realidad es 200 porqué T2 leyó Y antes que se le restara 100.

El locking binario lo soluciona porque T1 puede pedir locks sobre todos los items que tiene que updatear evitando que T2 se meta en el medio y lea valores en el medio de las modificaciones.


## 04/08/14
### 13. ¿Qué es el rollback de una transacción? (1 punto) 


## 11/04/14
## 06/03/14
## 26/12/13
## 06/08/13 

### 81. Explicar detalladamente el problema de falsa actualización (como fue una traducción espantosa dio la posibilidad de elegir entre lost update o dirty read) 

**Lost update (falsa actualización):** Ocurre cuando tenemos dos writes concurrentes al mismo data item, básicamente dos transacciones leen el mismo data item lo modifican o no y lo vuelven a escribir, una pisando el update el otro. Por ejemplo considerar estas transacciones T1, T2 (nota escribo ti(..) para indicar que la transacción i está modificando el data item x pero este es el mismo entre las 2 o más transacciones): 

    r1(x), t1(x = x + 1), r2(x), t2(x = x + 2), w1(x), w2(x)

Al final de esto tenemos que X = X + 2 y n X = X + 3, efectivamente perdimos el update de T1.

**Dirty read**: Este problema ocurre cuando tenemos una (o más) transacciones que leen un item modificado por otra que luego fue abortada, esencialmente leyendo un valor que tendría que haber sido rollbackeado. Por ejemplo

    r(x), t1(x = x + 1), w(x), r2(x), a1, // T2 hace algo con x	

Nota: los dirty reads se arreglan con un schedule cascadeless (ACA)

## 11/04/12

### 106. Defina grafo de precedencia y enuncie el teorema de  serializabilidad. Por qué es importante este teorema en el control de concurrencia?  

Un grafo de precedencia (también llamado de seriabilidad) es un grafo que se 
arma a partir de las operaciones de varias historias(transacciones) para saber 
cuando hay conflictos.
El teorema de seriabilidad nos dice que si el grafo resultante no tiene ciclos 
la historia se puede serializar (es decir hay una historia serial equivalente).

Para armarlo se hace lo siguiente: 

1. Definir un nodo por cada transaccion 
2. Un arco entre nodos si tienen una operación en conflicto (el arco va del nodo
   cuya operación ocurre antes hacía el otro).

Recordar que los conflictos eran si dado un item ocurría uno atras del otro un
write/read, read/write o write/write entre dos transacciones.


## 13/12/19  

### 134. ¿Qué es el teorema CAP?  

El teorema CAP nos dice que de las siguientes tres propiedades solo podemos
tener dos:

1. **Consistency:** Todos los nodos del sistema ven exactamente los mismos valores de los datos en
el mismo momento. 

2. **Availability:** El sistema no puede dejar de estar funcional. Cada interacción con el sistema
devuelve una respuesta (sin errores) independientemente del estado de cada nodo
individual. No necesariamente la respuesta tiene el write más reciente. 

3. **Partitioning tolerance:** El sistema no falla si se cae un nodo, se pierden y o retrasan los mensajes.

## 06/12/18


## 01/08/17

### 189. Decir qué son las propiedades BASE.

Recordemos que el teorema CAP nos decia que podíamos tener a lo sumo 2 de las 
siguientes 3 propiedades: Consistencia (C), Alta disponibilidad (A) y Tolerancia 
a las particiones (P). 

De las bases de datos no-SQL además salen unas propiedades llamadas BASE que son:

**B**asic **A**vailability: disponibilidad (en terminos del teorema CAP), se
garantiza alta disponiblidad dejando de lado consistencia, fallas en algun nodo 
no dejan no operacional a la base de datos, incluso devolviendo resultados 
inconsistentes. 

**S**oft state: la base de datos puede cambiar de estado incluso sin input, se
abandona el manejo de consistencia y este es responsabilidad del desarrollador.
Esto viene de la siguiente propiedad, a medida que hagamos operaciones no
necesariamete la bbdd esta en un estado final y nos puede dar resultados
distintos.

**E**ventual consistency: relacionado al item anterior, la base de datos 
eventualmente va a llegar a un estado consistente mientras no reciba nuevos 
inputs. Esto significa que incluso puede ejecutar varias transacciones sin
necesariamente haber llegado a un punto consistente después de cada una (cosa
que ACID si lo hacía).


Ver [Historia CAP y término BASE](#Referencias)

## 15/05/17
 
### 207. Describa brevemente las bases de datos orientadas a grafos.

Una base de datos orientada a grafos como su nombre lo indica es una base de
datos definida como nodos y ejes de un grafo donde los ejes son relaciones
tipadas y además ambos (nodos y relaciones) pueden tener propiedades.

A diferencia de las otras bbdd noSQL las bases de grafos **si** cumplen las 
propiedades ACID.

## 02/03/17

### 233. Bases NO-SQL porque se dicen 'schemaless'? Ejemplificar.

En una DB SQL tenemos que especificar el schema de la tabla, es decir que
elementos y tipos pueden ser guardados en la misma y no podemos
insertar/modificar o borrar algo que no cumpla esas reglas (sin contar por
supuesto un alter o operación del estilo). En cambio las DB noSQL no tienen que 
enforzar un esquema, en ese sentido son schemaless el schema en si pasa a ser un
problema del desarrollador y no de la DB. 

Por ejemplo podemos considerar una DB key-value en la cual con una key podemos
acceder a un valor que puede ser cualquier cosa, por ejemplo videos, imagenes
texto etc, sin necesariamente describirlo en un schema. Un ejemplo podría ser
MongoDB (key-document) o Cassandra (key-value). En mongoDB se guardan cosas 
JSON-style sin tener un schema fijo, por ejemplo podriamos guardar lo siguiente 

    { 
        name : “Joe”, age : 30, interests : ‘football’ 
    }   
    { 
        name : “Kate”, age : 25 
    }

Y asi es fácil tambien expandirlo agregando campos a medida que sea necesario
sin mantener una consistencia con el resto, en algún sentido es como un
documento que podemos expandir dinámicamente.


# Referencias

1. [Historia CAP y término BASE](https://www.julianbrowne.com/article/brewers-cap-theorem/)


