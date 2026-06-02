1. Contexto de la Misión
Un antiguo carguero espacial ha sufrido una avería en un sector inestable, esparciendo valiosos contenedores con recursos por el espacio. El objetivo de este proyecto es incorporar una nueva Nave de Rescate. La misión deberá ser completamente autónoma; es decir, no requiere de interacción de teclado ni mouse. Al iniciar la misión, la nave debe comenzar su recorrido, interactuando con el entorno continuamente para evadir obstáculos y rescatar el cargamento perdido antes de quedarse sin combustible.

2. Requerimientos
A. Autopiloto y Navegación Flexible La nave debe operar sin intervención humana desde el momento en que comienza la misión.
Percepción y Adaptabilidad: La nave debe analizar continuamente su entorno para tomar decisiones de movimiento. Las instrucciones de vuelo no deben ser rígidas; la lógica implementada debe permitir a la nave reaccionar a los obstáculos que tenga enfrente en tiempo real (por ejemplo, girar si detecta un asteroide o el límite del espacio, o atacar determinados objetos).
Prioridad de Rescate: Si los sensores detectan un recurso en las cercanías, la rutina de vuelo debe ser capaz de alterar el rumbo para intentar interceptarlo.

B. Configuración de Escenarios (Mapas) Para demostrar que la navegación es capaz de adaptarse, se requiere:
Diseño de Mapas: Definir al menos dos configuraciones de mundos con disposiciones de obstáculos y recursos diferentes que permitan visualizar distintos escenarios de los puntos detallados en la consigna. Se recomienda modificar la cantidad de casilleros del mapa para probar las misiones en un escenario más grande.
Prueba de Versatilidad: La nave debe ser capaz de cumplir su misión en cualquiera de estos escenarios sin necesidad de modificar su código fuente.

C. Los Recursos Valiosos: Se deben incorporar a la misión contenedores de recursos listos para ser recogidos. Cada contenedor debe estar valorizado con "créditos espaciales" y debe poseer grabado en su exterior un código de manifiesto (una cadena de texto, por ejemplo: "MAT-001", "CHATARRA-99", "CRIS-OMEGA-X"). 
D. Gestión de la Bodega de Carga La nave cuenta con una capacidad física estricta que debe ser administrada mediante software.
Límite de Almacenamiento: La nave posee una bodega con capacidad máxima (por ejemplo, exactamente 10 espacios disponibles). Esta estructura de almacenamiento debe modelarse obligatoriamente utilizando un arreglo.
Lógica de Recolección: Al entrar en contacto con un contenedor, la computadora intentará guardarlo en la bodega. Si la bodega ya alcanzó su capacidad máxima, la nave no podrá retener el objeto y deberá continuar su trayectoria.

E. Bitácora de Sectores: La nave debe registrar su trayectoria en una matriz de sectores. Cada vez que la nave ocupe un sector, debe registrar la visita en la matriz. Si pasa varias veces por un mismo lugar, todas deben ser registradas.

F. Desafío creativo: se deberá agregar al menos un nuevo componente o modificar al menos un componente existente (nave, otro ítem además del contenedor, piloto, obstáculo, otro tipo de ataque, etc). Se sugiere validar la propuesta con el tutor previo a su implementación.

G. Computadora de a bordo: Reporte de Misión La misión finaliza cuando la nave agota su combustible o queda físicamente inmovilizada. En ese instante, la computadora debe procesar la bodega y emitir por consola un Reporte Final detallando:
Balance económico: El valor total acumulado de todos los contenedores rescatados.
Estado de capacidad: La cantidad de espacios de carga que quedaron vacíos al finalizar el recorrido.
El Gran tesoro: El valor del recurso individual más caro que se logró subir a bordo.
Análisis de Manifiesto Crítico: El carguero notificó que perdió un "Cristal de Energía Crítico" altamente inestable. No se conoce su código exacto, pero se sabe que su código de manifiesto contiene la secuencia "OMEGA". El sistema debe rastrear en la bodega e informar si dicho Cristal se encuentra a bordo o si se perdió en el espacio.
Sectores más transitados: al finalizar la misión, la computadora debe imprimir la matriz completa en consola, mostrando qué casilleros fueron los más transitados. 
