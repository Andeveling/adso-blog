---
author: Andres Parra
pubDatetime: 2024-03-18T12:17:41.816Z
title: "Diseño de Base de Datos: Modelo Entidad-Relación para un Sistema de Control de Vuelos"
slug: "diseno-de-base-de-datos-modelo-entidad-relacion-sistema-control-vuelos"
featured: true
draft: false
tags:
  - Base de Datos
  - Modelo Entidad-Relación
  - Diseño de Base de Datos
description: "En este artículo, exploraremos el diseño de una base de datos para un sistema de control de vuelos, adaptado a las reglas de gestión establecidas. Desde la identificación de entidades y atributos hasta la definición de relaciones, aprenderemos a crear un modelo entidad-relación que satisfaga los requisitos del sistema."
ogImage: "https://res.cloudinary.com/dg84upfsp/image/upload/v1710785999/adso-blog/tak4pmyoa3adkvmgedvm.jpg"
---

Según el "Anexo – Estudio de caso" gestión de sistemas de control de vuelos, el diseño de la base de datos desempeña un papel fundamental para garantizar la eficiencia y la integridad de los datos. En este artículo, vamos a explorar el proceso de diseño de una base de datos para un sistema de control de vuelos, adaptado a las reglas de gestión establecidas en el Anexo suministrado.

## Introducción

El diseño de una base de datos comienza con la identificación de las entidades, atributos y relaciones clave que representan el dominio del problema. En el caso de nuestro sistema de control de vuelos, las reglas de gestión proporcionan información crucial sobre las entidades involucradas y cómo están interrelacionadas.

## Entidades y Atributos

1. Para comenzar, identificamos las siguientes entidades principales:

- Aeropuerto
- Modelo de Avión
- Programa de Vuelo
- Vuelo
- Escala Técnica

2. Cada una de estas entidades tiene atributos específicos que las caracterizan, se ha añadido un ID por cada uno para que tengan un identificador único. Por ejemplo:

- **Aeropuerto**: ID, Código, Nombre, Ciudad, País
- **Modelo de Avión**: ID, Modelo, Capacidad
- **Programa de Vuelo**: ID, Número de vuelo, Línea aérea, Días de la semana
- **Vuelo**: ID, Fecha, Plazas vacías
- **Escala Técnica**: ID, Aeropuerto de Escala
  

## Relaciones

3. Una vez identificadas las entidades y sus atributos, establecemos las relaciones entre ellas. Las reglas de gestión nos indican cómo se relacionan las entidades en el contexto del sistema de control de vuelos. Algunas de las relaciones clave incluyen:

- Entre Aeropuerto y Modelo de Avión: Relación de que en cada aeropuerto pueden tomar tierra diversos modelos de aviones.
- Entre Aeropuerto y Programa de Vuelo: Relación de que en cada aeropuerto existe una colección de programas de vuelo.
- Entre Programa de Vuelo y Aeropuerto: Relación de que cada programa de vuelo despega de un aeropuerto y aterriza en otro.
- Entre Programa de Vuelo y Vuelo: Relación de que cada vuelo realizado pertenece a un cierto programa de vuelo.
- Entre Vuelo y Modelo de Avión: Relación de que para cada vuelo se quiere conocer el modelo de avión utilizado.
- Entre Vuelo y Escala Técnica: Relación de que algunos vuelos pueden hacer o no escalas técnicas.
- Entre Escala Técnica y Aeropuerto: Relación de que la escala se hace en un Aeropuerto. 

## Conclusión

El diseño de una base de datos utilizando el modelo entidad-relación es un proceso fundamental en el desarrollo de sistemas de información. Al comprender las reglas de gestión y las necesidades del sistema, podemos crear una estructura de datos que refleje con precisión el dominio del problema y permita una gestión eficiente de la información en el sistema de control de vuelos.

Para la elaboración del modelo use la app web https://app.diagrams.net/

![Modelo entidad Relación](https://res.cloudinary.com/dg84upfsp/image/upload/v1710785999/adso-blog/tak4pmyoa3adkvmgedvm.jpg "Modelo entidad Relación")