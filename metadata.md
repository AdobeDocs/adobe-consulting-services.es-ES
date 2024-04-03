---
product: adobe experience manager
solution: Experience Manager
description: Documentación del Experience Manager consultor
type: Documentation
git-repo: https://github.com/AdobeDocs/adobe-consulting-services.es-ES
index: y
source-git-commit: e2dac4b36fb94d72b72ef6f73a77e3f566539444
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 54%

---


# Metadatos para uso interno

Los metadatos del sistema de creación de GitHub son jerárquicos y se definen con los siguientes niveles crecientes de precedentes.

1. metadata.md
1. TDC
1. Artículo

Los metadatos definidos en el archivo metadata.md se aplican a todo el repositorio, pero se pueden sobrescribir en los niveles de TDC y de artículo. Cualquier anulación de los metadatos debe realizarse en el nivel más bajo posible.

metadata.md

* `product`
* `git-repo`
* `index: y`

TDC

* `sub-product`
* `user-guide-title`

Artículo

* `title`
* `description`

Encontrará información adicional sobre los metadatos en la [guía de creación interna](https://experienceleague.adobe.com/docs/authoring-guide-exl/using/authoring/metadata.html).
