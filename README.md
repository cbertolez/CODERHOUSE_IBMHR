# Proyecto final
Proyecto final de Data Science Coder House 
Integrantes: Belén Torres, Celeste Bertolez
Profesor: Jorge Kamlofsky
Tutor: Fernando Culell


# IBM Data Science

IBM ha recopilado información sobre la satisfacción de los empleados, los ingresos, la antigüedad y algunos datos demográficos. Incluye los datos de 1470 empleados. El dataset elegido es:
[IBM dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset?utm_source=canva&utm_medium=iframely)




## Tabla de contenido

Los contenidos que se tratan en este proyecto son:

- El problema

- Las preguntas de investigación

- Data Adquisition / Data Wrangling

- Análisis exploratorios EDA

- Modelos candidatos - Modelo elegido

- Conclusiones

- Lineas futuras

- Bibliografía
##  El problema
El  área  de  RRHH  de  una  empresa  tiene  entre  sus  objetivos  principales detectar  las  oportunidades  de   mejora para ajustar el gap entre las competencias de  las personal y los requerimientos de los puestos en  particular.  Para  esto  se  realizan  evaluaciones  de  desempeño periódicas a las personas y a los equipos  de  trabajo  en  cuanto  a  su  rendimiento  real  en  comparación a lo planificado según la planificación de  RRHH.
Una función clave del área, es asegurar de que se viva  en un clima laboral favorable y cómodo para todos los  colaboradores. Entre otros actores a tener en cuenta,  esto ayuda a asegurar altos índices de productividad en  los  procesos  de  producción/servucción,  al  mismo  tiempo  que  ayuda  a  mantener  la  motivación  y  la  fidelidad de los integrantes de la organización en todos  
sus niveles
## Preguntas y objetivos de la investigación
- ¿Cuánto es el tiempo de permanencia  en una empresa antes de aceptar una  
oferta del mercado mejor paga?
- ¿Cuál es  la  tasa  de  rotación  por  estrato de antigüedad del personal?  
- ¿Cuáles son las causas determinantes  que  hacen  que  el  empleado  decida  
renunciar  o  disminuya  su  rendimiento  por insatisfacción laboral?
## Métricas para clasificación
Criterios para decidir un mejor algoritmo:  
- **Accuracy**: La exactitud (accuracy) mide el porcentaje de casos que el modelo ha acertado
- **Precisión**: Con la métrica de precisión podemos medir la **calidad** del modelo de machine learning en tareas de clasificación
- **Recall**: El modelo que tiene mejor recall o sensibilidad, es decir proporción de casos positivos bien identificados 
- **f1-Score**: El valor F1 se utiliza para combinar las medidas de precision y recall en un sólo valor. Esto es práctico porque hace más fácil el poder comparar el rendimiento combinado de la precisión y la exhaustividad entre varias soluciones
## Resultados de los diferentes modelos candidatos

Seleccionando posibles algoritmos candidatos:
![Comparación entre los resultados](https://github.com/cbertolez/CODERHOUSE_IBMHR/blob/main/modelos%20candidatos.PNG)
- **Accuracy**: El modelo ajusta razonablemente bien con más de 75% en accuracy de tanto en train  
como en test en todos los modelos  
- **Precisión**: El modelo que mejor precision tiene es Random Forest fue optimizado buscando los  
mejores hiperparámetros con RandomizedSearchCV  
- **Recall**: El modelo que tiene mejor recall o sensibilidad, es decir proporicion de casos positivos bien  
identificados por el algoritmo es el modelo de Regresión Logística.  
- **f1-Score**: De todos los modelos el que mejor se ajusta en f1 es el modelo de AdaBoostClassifier.
## Modelo elegido
Debido a que el modelo Regresion logistica obtuvo los mejores resultados con respecto a esta metrica, lo usaremos para los próximos pasos ![modelo elegido](https://github.com/cbertolez/CODERHOUSE_IBMHR/blob/main/modelo%20de%20regresion1.PNG)

## Conclusiones
-   Si bien el salario no es competitivo, el mal ambiente de trabajo o la mala relación con el jefe pueden ser razones para que un trabajador renuncie, aunque estas no son razones suficientes para que un empleado renuncie.

-   La renuncia laboral es provocada por **una combinación de múltiples factores que pueden o no ser parte de las características de este conjunto de datos**, sin embargo, se debe tener en cuenta que cada empresa presentará diversos factores y formas de calificar al trabajador, por lo que este conjunto de datos debe tomarse como una visión general.

-   La **regresión logística** demostró ser una la mejor herramienta para clasificar y predecir qué empleados no renunciarán, y eso permite a las empresas seguir tomando medidas y beneficios necesarias para expandir la satisfacción laboral y mejorar la calidad de vida del empleado.

-   Pudimos responder algunas preguntas del problema inicial planteado pero a lo largo de la investigación y el desarrollo surgieron otras nuevas.
## Bibliografía
- [Employee engagement](https://www.comparably.com/companies/ibm/employee-engagement)
- [Satisfacción de empleados](https://www.questionpro.com/blog/es/como-hacer-encuestas-de-satisfaccion-de-empleados/)
- [Métricas de clasificación](https://www.iartificial.net/precision-recall-f1-accuracy-en-clasificacion/)







