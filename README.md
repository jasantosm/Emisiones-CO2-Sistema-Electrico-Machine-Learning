# **Proyecto: Modelo Machine Learning de las Emisiones de Gases Contaminantes (CO2Eq) Sistema Eléctrico Colombiano**

Realizado por: **Julián Andrés Santos Méndez**

email: ingjuliansantos@gmail.com

# **1. Entendimiento del Negocio**
## **1.1. Objetivos de negocio y situación actual**
Colombia es un país que se enorgullese de que el 69.25% de su energía eléctrica es generada con recursos renovables, los cuales constituyen una matriz energetica no fósil muy variada con diferentes fuentes, tales como la energía hidráulica, la biomasa, la energía eólica y la energía solar, sin embargo, el 98.5% de esa energía es generada con recursos hidráulicos a gran escala. 

Como consecuencia de esa depedencia a los grandes embalses, se tiene un sistema eléctrico que es muy sensible a fenomenos climáticos como el fenomeno del niño.

*Tabla 1. Capacidad efectiva neta del Sistema Interconectado Nacional (SIN) por tipo de recurso natural, Fuente: Informe 2019 XM S.A. E.S.P. [1]*

| Fuente de energía               | 2018 MW   | 2019 MW   | Participación (%) | Variación 2019 vs. 2018 |
|---------------------------------|-----------|-----------|-------------------|-------------------------|
| **Fuentes de energía No Renovable**
| Combustible fósil               | 5,308.14  | 5,369.74  | 30.75%            | 1.16%                   |
| Total No Renovable              | 5,308.14  | 5,369.74  | 30.75%            | 1.16%                   |
| **Fuentes de energía Renovable**    
| Biomasa                         | 139.60    | 139.60    | 0.80%             | 0.00%                   |
| Eólica                          | 18.42     | 18.42     | 0.11%             | 0.00%                   |
| Hidráulica                      | 11,836.57 | 11,916.61 | 68.24%            | 0.68%                   |
| Solar                           | 9.80      | 17.98     | 0.10%             | 83.43%                  |
| **Total Renovable**                 | **12,004.39** | **12,092.60** | **69.25%**           | **0.73%**                   |
| **Total general**                  | **17,312.53** | **17,462.34** | **100.00%**           | **0.87%**                   |

Para contrarrestar esa dependecia a la energía hidráulica, el país inició el proceso de incoporación de mas activos de generacion térmica con combustibles fósiles[2].

Es por esta razón que **el objetivo** principal de este proyecto es hacer un seguimiento de las emisiones de gases contaminantes que ha hecho el sistema eléctrico Colombiano y determinar su relacion con otras variables del sistema, para así tener una base con la cual analizar en el futuro las emisiones de los nuevos activos térmicos.

## **1.2. Metas del proyecto de Machine Learning**
Este proyecto es la continuacion del proyecto de EDA <https://github.com/jasantosm/Emisiones-CO2-Sistema-Electrico>, por lo tanto las metas de este proyecto son:
1. Seleccionar un modelo de aprendizaje automático para predecir la emisiones de $CO_2$ equivalente del sistema eléctrico colombiano, como serie de tiempo.