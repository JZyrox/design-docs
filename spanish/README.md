# dannihehbot
Link: [[Link a este design doc](https://github.com/pakoite/design-docs/edit/main/spanish/README.md)](#)

Author(s): Daniela Guadalupe Hernández Guzmán

Status: [Draft, Ready for review, In Review, Reviewed]

Ultima actualización: 2015-03-15

## Contenido
- Goals
- Non-Goals
- Background
- Overview
- Detailed Design
  - Solucion 1
    - Frontend
    - Backend
  - Solucion 2
    - Frontend
    - Backend
- Consideraciones
- Métricas

## Links
- [Un link](#)
- [Otro link](#)

## Objetivo
_Estamos desarrollando un bot para Telegram que funcionará como un buscador de definiciones. El propósito de este proyecto es proporcionar una herramienta rápida y eficiente que permita a los usuarios obtener definiciones de palabras o conceptos directamente en Telegram, sin necesidad de salir de la aplicación.

Este bot está orientado a facilitar el acceso a definiciones de manera sencilla y accesible, mejorando la experiencia de aprendizaje y consulta dentro de la plataforma._

## Goals
_Permitir a los usuarios buscar definiciones de palabras o conceptos a través de comandos en Telegram._

_Responder de manera rápida y precisa con la definición solicitada._

_Soportar múltiples idiomas (opcional en fases futuras)._
## Non-Goals
_No se buscará proporcionar definiciones de términos altamente técnicos o especializados en esta primera versión._

_No se incluirá integración con bases de datos complejas o de pago en la fase inicial._

_No se desarrollarán interfaces gráficas avanzadas, ya que el enfoque será texto plano dentro de Telegram._

## Background
_Telegram ofrece la posibilidad de crear bots mediante su API. Este bot se construirá para satisfacer la necesidad de obtener definiciones rápidas, principalmente utilizando APIs abiertas de diccionarios en línea._

Recursos considerados:

_Documentación oficial de la API de Telegram._

_APIs de definiciones como la de DictionaryAPI._

## Overview
_El bot funcionará a través de comandos específicos en Telegram. Los usuarios podrán enviar mensajes con palabras o frases y el bot devolverá las definiciones correspondientes. El bot procesará la entrada del usuario, consultará la API de definiciones y mostrará el resultado en un formato claro y legible._

## Detailed Design
Nuevas funciones:

_Función de procesamiento de mensajes._

_Función de consulta a la API de definiciones._

_Función de formateo y envío de la respuesta._

Componentes necesarios:

_Componente de interacción con la API de Telegram._

_Componente de integración con la API de definiciones._

Código reusable:

_Módulos para validación de entrada y procesamiento de texto._

_Manejadores de errores reutilizables para mejorar la estabilidad del bot._

## Solution 1
### Frontend
_No aplica, ya que la interacción será a través de la interfaz de Telegram._
### Backend
_Python con la librería python-telegram-bot._

_Consultas a APIs de definiciones._

_Estructura modular para facilitar la escalabilidad._

## Solution 2
### Frontend
_No aplica en esta versión inicial._
### Backend
_Node.js con node-telegram-bot-api como alternativa._

_Uso de axios para realizar peticiones HTTP a las APIs de definiciones._

## Consideraciones
_Dependencia de APIs externas para obtener las definiciones, lo cual puede implicar restricciones en la cantidad de solicitudes._

_Manejo adecuado de errores y respuestas no encontradas._

_Posible necesidad de caché para optimizar las respuestas._

## Métricas
_Tiempo de respuesta del bot._

_Porcentaje de definiciones correctamente devueltas._

_Cantidad de solicitudes procesadas por día._

_Nivel de satisfacción del usuario (opcional mediante feedback)._
