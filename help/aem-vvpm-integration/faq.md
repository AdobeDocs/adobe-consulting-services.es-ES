---
title: Preguntas frecuentes sobre la integración con Veeva Vault
description: Preguntas frecuentes sobre la integración con Veeva Vault
exl-id: c308ebb3-7881-4094-9f35-c67a96fb5ab1
product_v2:
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
    internal-label: Experience Manager
source-git-commit: 02aa1622ee171cd56ec9cdeb6bdef04b5d5464b5
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 1%
---
# Preguntas frecuentes

**¿Qué metadatos se deben sincronizar con Veeva?**

Es importante comprender los metadatos basados en el tipo de contenido (p. ej., promociones) en el portal de Veeva. Después de revisar el portal de Veeva, construya el esquema de metadatos de contenido en AEM para contener todos los metadatos relevantes para cada recurso/página y configure la integración para asignar los metadatos entre los dos sistemas.

**¿La integración es compatible con los documentos vinculados de Veeva? Si no es así, ¿qué tipos de relación se admiten?**

No. Ver [documento de Veeva](https://vaulthelp2.vod309.com/wordpress/admin-user-help/documents-admin-user-help/about-document-relationships/). El documento vinculado (tipo de relación de referencia) es uno de los tipos de relación estándar que no se puede crear o eliminar mediante API debido a que tiene un comportamiento especial de Vault. El componente, los documentos de soporte y cualquier otro no incluido en esta lista deben poder configurarse mediante la configuración en la nube de AEM Veeva.

**¿Admite la integración el contenido modular de AEM?**

Sí, la integración es compatible con fragmentos de contenido y de experiencias de AEM.

**¿Admite la integración el contenido modular de Veeva?**

No, en este momento no.

**¿Sincroniza la integración las anotaciones visuales de Veeva con AEM?**

No, en este momento no. Solo se puede acceder a las anotaciones visuales mediante API as a PDF.

**¿Cómo establecemos permisos en documentos VPM sincronizados por la integración?**

La integración utiliza un usuario de servicio para cargar documentos a través de la API.  Las reglas de anulación y asignación por defecto de documentos (funciones por defecto en documentos) solo son compatibles con la interfaz de usuario de VPM y no se aplican al utilizar la API. Se recomienda utilizar DAC (control de acceso dinámico) para las asignaciones de funciones. La DAC se aplica a través de todos los puntos de contacto, incluida la API. [Consulte la documentación aquí.](http://vaulthelp2.vod309.com/wordpress/admin-user-help/ah-user-permissions-access-control/about-dynamic-access-control-for-documents/)

**¿Admite la integración varias instancias de VPM?**

La integración utiliza un enfoque de configuración en la nube que permite configurar varios extremos de Veeva desde una instancia de AEM.

**¿Admite la integración la publicación de AEM?**

No, esta integración solo funciona con el autor de AEM. Está pensado para facilitar los ciclos de revisión de MLR antes de que se publique el contenido.
