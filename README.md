# NEXT AUTO EXPORTS LLC — Desktop Cotizador

## Descripción

Herramienta HTML independiente para preparar facturas de gastos de logística, taller y preparación de vehículos en Miami. Permite editar los datos del cliente y del vehículo, detallar los gastos, calcular los totales automáticamente e imprimir o guardar la factura como PDF.

Esta herramienta es independiente de la plataforma principal de cotizaciones y proformas. No modifica el HTML de esa plataforma.

## Requisitos

- Navegador moderno como Chrome, Brave, Edge o Safari.
- Conexión a internet para cargar el lector PDF cuando sea necesario.
- Cotización o factura proforma en PDF. La extracción funciona mejor cuando el PDF contiene texto seleccionable; los PDF escaneados como imágenes pueden requerir OCR, que no está incorporado en esta versión.

## Cómo abrir la herramienta

1. Descarga `NEXT_AUTO_EXPORTS_LLC_COTIZADOR.html`.
2. Abre el archivo con tu navegador.
3. Completa los datos manualmente o importa una cotización/proforma en PDF.
4. Revisa todos los datos detectados y corrige lo que sea necesario.
5. Confirma el número de factura cuando esté listo.
6. Pulsa **Imprimir / Guardar PDF** y selecciona **Guardar como PDF** en el diálogo del navegador.

## Importar una cotización o proforma PDF

1. Pulsa **Importar cotización PDF**.
2. Selecciona el PDF exportado desde la otra plataforma.
3. La herramienta intentará leer el texto del documento y detectar campos que puedan incluir:
   - Nombre del cliente.
   - Teléfono y dirección.
   - Vehículo, año, color y VIN/chasis.
   - Fecha y concepto de la operación.
   - Partidas de gastos e importes reconocibles.
4. Comprueba el resultado antes de generar la factura.

La extracción automática no garantiza reconocer todos los diseños de PDF. Los nombres de campos, el orden del texto, las tablas y los formatos numéricos pueden afectar el resultado. Verifica especialmente las partidas y los importes. No des por correctos los datos únicamente porque se hayan importado.

La importación puede reemplazar las partidas existentes para evitar mezclar gastos de la operación anterior con los de la nueva.

## Crear una factura nueva

Usa **Nueva factura / Limpiar todo** para empezar otra operación. La función debe limpiar los campos editables del cliente y del vehículo, el concepto y las partidas de gastos, restablecer la confirmación del número y dejar la herramienta lista para otra factura.

Después puedes introducir los datos manualmente o cargar un PDF nuevo. Revisa siempre que no queden datos de la operación anterior.

## Número de factura y nombre del PDF

- El número se calcula a partir de los últimos seis dígitos numéricos del VIN cuando hay suficientes dígitos disponibles.
- Si no se pueden obtener seis dígitos, se utiliza un número automático de seis dígitos.
- El botón de confirmación bloquea el número para la factura actual.
- El nombre sugerido para guardar el documento utiliza el número de factura, por ejemplo: `Factura_209759.pdf`.

La comprobación de números usados depende del almacenamiento local del navegador y no equivale a un registro central compartido entre dispositivos o navegadores. Para evitar duplicados entre usuarios, lleva un registro externo de las facturas emitidas.

## Editar gastos y calcular totales

- Añade partidas con **Añadir línea**.
- Edita la cantidad, descripción y precio unitario de cada gasto.
- Elimina partidas que no correspondan a la operación.
- La vista previa y los totales se actualizan mientras editas los datos.

Revisa cantidades, moneda e importes antes de confirmar la factura.

## Modo oscuro y claro

Utiliza el botón de modo oscuro/claro en el encabezado para cambiar la apariencia de la interfaz.

## Guardar o imprimir el PDF

1. Pulsa **Imprimir / Guardar PDF**.
2. En el diálogo del navegador, elige **Guardar como PDF**.
3. Comprueba el nombre del archivo antes de guardar.

El navegador puede solicitar que confirmes la carpeta de destino. El nombre del archivo se prepara automáticamente cuando el navegador lo permite; la herramienta no puede garantizar un guardado silencioso.

## Limitaciones conocidas

- La lectura de PDF requiere que el texto sea accesible. Un PDF escaneado puede no producir texto que la herramienta pueda extraer.
- El lector PDF puede necesitar conexión a internet para cargarse.
- La extracción automática es una ayuda inicial, no una validación contable. Siempre compara los campos importados con el documento original.
- Los números usados se recuerdan localmente en el navegador y no se sincronizan entre equipos.
- Guarda copias de las facturas emitidas en una ubicación segura.

## Archivo principal

`NEXT_AUTO_EXPORTS_LLC_COTIZADOR.html`

Este README describe el uso previsto de la herramienta. Las funciones de importación deben comprobarse con cotizaciones y proformas reales de la plataforma de origen antes de depender de ellas en el trabajo diario.
