Introducción


Este análisis busca entender por qué algunos clientes se van (churn/evasion) y cómo podemos retenerlos.


Datos


Se trabajó con un archivo JSON (como si viniera de una API) convertido a tabla. Variables clave: customerID, Churn, género, edad, contrato, método de pago, mensualidad y gasto total.


Limpieza


Columnas renombradas para mayor claridad.

Conversión de texto a números en cargos.

Se unificaron categorías como "No internet service" en "No".

Se eliminaron duplicados.

Se imputaron valores de TotalCharges cuando faltaban.

Se creó la columna Cuentas_Diarias = MonthlyCharges/30.


Exploración


Tasa de evasión total: ~26.5% (1 de cada 4 clientes).

Contratos mes a mes tienen mucho más evasión (42%) vs contratos de 1 año (11%) o 2 años (3%).

Método de pago: cheque electrónico con 45% de evasión, vs automático con ~17%.

Internet: fibra óptica 42% de churn, DSL 19%, sin internet 7%.


Conclusion


La evasión está fuertemente asociado a contratos cortos, método de pago y tipo de internet. Los clientes nuevos y con mensualidades más altas tienden a irse más.

Recomendaciones

♥ Retener a clientes nuevos en los primeros 3–6 meses con promociones.

♥ Incentivar contratos largos con descuentos.

♥ Promover pagos automáticos para reducir la evasión.

♥ Ofrecer bundles con valor agregado para clientes de cargos altos.

♥ Activar alertas tempranas para clientes en riesgo (ej. por baja de servicios).

