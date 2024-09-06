# Plantilla de Email en HTML Optimizada para Outlook

Esta es una plantilla de email en HTML diseñada para garantizar una visualización correcta en Microsoft Outlook, incluyendo versiones más antiguas como Outlook 2010 y 2013. Dado que Outlook utiliza el motor de renderizado de Microsoft Word, es crucial tener en cuenta ciertas limitaciones y peculiaridades al crear correos electrónicos que se verán bien en este cliente de correo.

## Características

- **Compatibilidad con Outlook:** La plantilla ha sido probada en varias versiones de Outlook, incluyendo 2010, 2013, 2016, 2019 y Outlook 365.
- **Soporte para diseños de columna:** Uso de tablas para estructurar el contenido, garantizando un diseño de columnas responsivo en Outlook.
- **Fuentes estándar:** Uso de fuentes estándar y seguras para web, garantizando una buena visualización en todos los clientes de correo.
- **Imágenes internas:** Implementación correcta de imágenes internas que se renderizan adecuadamente en Outlook.
- **Botones y enlaces estilizados:** Los botones y enlaces están diseñados usando `VML` para asegurar que se muestren correctamente en Outlook.

## Estructura del Proyecto

\`\`\`
/plantilla-email/
│
├── index.html               # Archivo principal de la plantilla de email
│
├── images/
│   ├── logo.png             # Ejemplo de imagen incluida en el email
│   └── banner.jpg           # Imagen de banner de ejemplo
│
└── README.md                # Instrucciones y documentación
\`\`\`

## Instrucciones de Uso

1. **Editar Contenido:** Abre el archivo `index.html` y edita el contenido con tu propio texto e imágenes. Asegúrate de mantener la estructura básica de tablas y estilos en línea para preservar la compatibilidad con Outlook.

2. **Incorporar Estilos en Línea:** Si agregas nuevos estilos, recuerda usar una herramienta de "inline CSS" para convertirlos en estilos en línea, ya que muchos clientes de correo, incluyendo Outlook, no soportan \`<style>\` en el \`<head>\`.

3. **Pruebas de Compatibilidad:** Antes de enviar el email a tus suscriptores, prueba la plantilla en diferentes clientes de correo (incluyendo diferentes versiones de Outlook) usando herramientas como [Litmus](https://litmus.com/) o [Email on Acid](https://www.emailonacid.com/).

4. **Ajustes para Outlook:** Si encuentras algún problema específico en Outlook, consulta la documentación oficial o foros especializados para encontrar soluciones específicas. Por ejemplo, el uso de \`<div>\` con \`display:inline-block\` puede no funcionar bien en Outlook, por lo que se recomienda usar tablas para lograr diseños de columnas.

## Consideraciones Especiales

- **Tablas:** La plantilla está construida utilizando un diseño basado en tablas, ya que Outlook maneja mejor las tablas que los \`div\` o \`flexbox\`.
- **Estilos en Línea:** Todos los estilos deben estar en línea. Outlook no procesa bien los estilos en el \`<head>\`.
- **Imágenes:** Usa el atributo \`width\` y \`height\` en las imágenes para asegurar que se dimensionen correctamente. Considera también el uso de \`mso-hide:all;\` para imágenes de fondo y otros elementos decorativos que Outlook podría manejar de manera diferente.
- **Botones:** Los botones están hechos utilizando \`VML\` para asegurar que se vean correctamente en versiones de Outlook que no manejan bien los estilos de fondo y bordes.

## Recursos Adicionales

- [Guía de desarrollo para correos electrónicos en Outlook](https://www.campaignmonitor.com/css/)
- [Plantillas gratuitas optimizadas para Outlook](https://litmus.com/community/templates)

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo \`LICENSE\` para obtener más detalles.' > README.md