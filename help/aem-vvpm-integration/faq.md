---
title: Preguntas frecuentes sobre la integración con Veeva Vault
description: Preguntas frecuentes sobre la integración con Veeva Vault
exl-id: c308ebb3-7881-4094-9f35-c67a96fb5ab1
source-git-commit: e4a5e55ac9b79a8de7dfa8ddd3d0ad99560917b8
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Preguntas frecuentes

**¿Qué metadatos se deben sincronizar con Veeva?**

Es importante comprender los metadatos basados en el tipo de contenido (p. ej., promociones) en el portal de Veeva. AEM Después de revisar el Portal de Veeva, construya el esquema de metadatos de contenido en el que se almacenen todos los metadatos relevantes para cada recurso o página y configure la integración para asignar los metadatos entre los dos sistemas.

**¿La integración es compatible con los documentos vinculados de Veeva? Si no es así, ¿qué tipos de relación se admiten?**

No. Ver [documento de Veeva](https://vaulthelp2.vod309.com/wordpress/admin-user-help/documents-admin-user-help/about-document-relationships/). El documento vinculado (tipo de relación de referencia) es uno de los tipos de relación estándar que no se puede crear o eliminar mediante API debido a que tiene un comportamiento especial de Vault. AEM El componente, los documentos de soporte y cualquier otro no incluido en esta lista deben poder configurarse mediante la configuración en la nube de Veva a través de la configuración de la nube de Veva.

AEM **¿Admite la integración el contenido modular de la?**

AEM Sí, la integración admite fragmentos de contenido y fragmentos de experiencias de la.

**¿Admite la integración el contenido modular de Veeva?**

No, en este momento no.

AEM **¿La integración sincroniza las anotaciones visuales de Veeva con el elemento de datos de la vista de la vista de la vista de la página de datos de?**

No, en este momento no. Solo se puede acceder a las anotaciones visuales mediante API como PDF.

**¿Cómo establecemos permisos en documentos VPM sincronizados por la integración?**

La integración utiliza un usuario de servicio para cargar documentos a través de la API.  Las reglas de anulación y asignación por defecto de documentos (funciones por defecto en documentos) solo son compatibles con la interfaz de usuario de VPM y no se aplican al utilizar la API. Se recomienda utilizar DAC (control de acceso dinámico) para las asignaciones de funciones. La DAC se aplica a través de todos los puntos de contacto, incluida la API. [Consulte la documentación aquí.](http://vaulthelp2.vod309.com/wordpress/admin-user-help/ah-user-permissions-access-control/about-dynamic-access-control-for-documents/)

**¿Admite la integración varias instancias de VPM?**

AEM La integración utiliza un enfoque de configuración en la nube que permite configurar varios puntos de conexión de Veeva desde una sola instancia de.

AEM **¿Admite la integración la publicación de los datos de manera predeterminada?**

AEM No, esta integración solo funciona con el autor de la. Está pensado para facilitar los ciclos de revisión de MLR antes de que se publique el contenido.
