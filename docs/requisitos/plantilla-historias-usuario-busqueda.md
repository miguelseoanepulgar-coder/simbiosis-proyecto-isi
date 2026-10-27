# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Fecha | [dd/mm/aaaa] |
| Versión | [Versión de trabajo] |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como usuario registrado, quiero poder filtrar por palabras, inclusión y exclusión de ingredientes la búsqueda de recetas, para poder encontrar recetas que se adecúen a mis necesidades.

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

Para poder realizar búsquedas simultaneas o mas cómodas para usuarios que requieran de una funcionalidad compleja o usuarios que se expresen de maneras diferentes.

## US-01

**Título:** Búsqueda de recetas por palabra clave

Como usuario registrado, quiero poder filtrar la búsqueda de recetas por palabras, para para poder encontrar recetas que se adecúen a mis necesidades.

**Fuentes:** UR-08; UC-21; FR-085; acta, apartado 2.

### Criterios de aceptación

- **CA-01.** Dado un usuario registrado usando la función de búsqueda de recetas de la aplicación, cuando escribe la frase "pastel" que esta contenida en el título o descripción de algunas recetas, entonces mostrar por pantalla las recetas con esa frase.
- **CA-02.** Dado un usuario registrado usando la función de búsqueda de recetas de la aplicación, cuando escribe la frase "njbhkl" que no esta contenida en el título o descripción de ninguna receta, entonces se muestra que no hay resultados por pantalla y se guarda la frase.
- **CA-03.** Dado un usuario registrado usando la función de búsqueda de recetas de la aplicación, cuando escribe la frase "pastel de caramelo" que esta contenida en el título o descripción de algunas recetas, entonces mostrar por pantalla las recetas con solo esa frase, ignorando las palabras por separado.

## US-02

**Título:** Búsqueda de recetas por inclusión de ingredientes

Como usuario registrado, quiero poder filtrar la búsqueda de recetas por inclusión de ingredientes, para  para para poder encontrar recetas que se adecúen a mis necesidades.

**Fuentes:** UR-08; UC-21; FR-086; acta, apartado 2.

### Criterios de aceptación

- **CA-01.** Dado un usuario registrado usando la función de búsqueda de recetas de la aplicación, cuando seleccionan los ingredientes "lechuga tomate y cebolla" que forman algunas recetas, entonces mostrar por pantalla la lista de recetas que están formadas por algunos de los ingredientes seleccionados.
- **CA-02.** Dado un usuario registrado usando la función de búsqueda de recetas de la aplicación, cuando selecciona los ingredientes "sal y azucar" que no forman ninguna receta en si, entonces se muestra que no hay resultados por pantalla y se guardan los ingredientes.
- **CA-03.** Dado un usuario registrado usando la función de búsqueda de recetas de la aplicación,  cuando el usuario realiza una búsqueda que el sistema no puede completar, entonces informa del problema y guarda los ingredientes.

## US-03

**Título:** Búsqueda de recetas por exclusión de ingredientes

Como usuario registrado, quiero poder filtrar la búsqueda de recetas por exclusión de ingredientes, para  para para poder encontrar recetas que se adecúen a mis necesidades.

**Fuentes:** UR-08; UC-21; FR-087; acta, apartado 2.

### Criterios de aceptación

- **CA-01.** Dado un usuario registrado usando la función de búsqueda de recetas de la aplicación, cuando selecciona excluir los ingredientes "vinagre y aceite", entonces mostrar por pantalla todas las recetas que no contengan ningún ingrediente seleccionado.
- **CA-02.** Dado un usuario registrado usando la función de búsqueda de recetas de la aplicación, cuando selecciona excluir todos los ingredientes, entonces se muestra que no hay resultados por pantalla y se guardan los ingredientes excluidos.
- **CA-03.** Dado un usuario registrado usando la función de búsqueda de recetas de la aplicación,  cuando el usuario realiza una búsqueda que el sistema no puede completar, entonces informa del problema y guarda los ingredientes excluidos.

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | Sí | Sí | - |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | Sí | Sí | - |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | Sí | Sí | - |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | Sí | Sí | - |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | Sí | Sí | - |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | Sí | Sí | - |

## Dudas pendientes

[Cuestiones pendientes de aclaración. Si no quedan cuestiones, indicar «Ninguna».]
