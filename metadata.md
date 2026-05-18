---
product: adobe experience manager
solution: Experience Manager
product_v2:
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
description: Consultar la documentación de Experience Manager
type: Documentation
git-repo: https://github.com/AdobeDocs/adobe-consulting-services.en
index: true
source-git-commit: 78d98fcb8f43f48cab7de480af1eac087526cec5
workflow-type: tm+mt
source-wordcount: 94
ht-degree: 2%

---


# Metadatos para uso interno

Los metadatos del sistema de creación de GitHub son jerárquicos y se definen con los siguientes niveles crecientes de precedentes.

1. metadata.md
1. ToC
1. Artículo

Los metadatos definidos en el archivo metadata.md se aplican a todo el repositorio, pero se pueden sobrescribir en los niveles de TDC y de artículo. Cualquier anulación de los metadatos debe realizarse en el nivel más bajo posible.

metadata.md

* `product`
* `git-repo`
* `index: y`

ToCs

* `sub-product`
* `user-guide-title`

Artículo

* `title`
* `description`

Encontrará información adicional sobre los metadatos en la [guía de creación interna](https://experienceleague.adobe.com/docs/authoring-guide-exl/using/authoring/metadata.html).
