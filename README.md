Driver Score – Modelo Predictivo Basado en Telemetría Vehicular
🧩 Descripción del Proyecto

Este repositorio contiene el desarrollo completo de un modelo de Driver Score diseñado para evaluar el comportamiento de conducción de un vehículo a partir de datos de telemetría en tiempo real.

El ecosistema captura señales como velocidad, frenadas bruscas, aceleraciones fuertes, giros agresivos, patrones de conducción y eventos emitidos por dispositivos GPS/IoT.
Estas señales se procesan y transforman en un puntaje que resume el nivel de riesgo o seguridad asociado a cada conductor.

El modelo está pensado para funcionar en tiempo real mediante Kafka y AWS, y además permite reentrenamiento periódico usando Piperlines de SageMaker.

* ¿Qué hace el modelo?

El modelo analiza eventos de telemetría (GPS y sensores) y genera un score que representa:

Nivel de conducción segura

Agresividad al volante

Tendencias de riesgo (frenadas bruscas, aceleración excesiva, exceso de velocidad)

Estabilidad del conductor por zonas, horas y patrones de uso

Cambios significativos frente a su comportamiento histórico

En producción, el modelo puede recibir eventos en tiempo real y responder con un Driver Score instantáneo por viaje, por conductor o por evento.

* Aplicaciones del Driver Score

El puntaje puede ser utilizado en múltiples contextos:

1. Seguridad Vial

Identificar patrones de conducción riesgosa y generar alertas.

2. Operación de flotas

Detectar conductores que requieren entrenamiento o intervención.

3. Seguros basados en uso (UBI – Usage Based Insurance)

Calcular primas variables y monitorear comportamiento.
🛠️ Tecnologías Utilizadas

Python 3.x

Pandas, NumPy

Scikit-learn

Kafka / MSK

AWS Lambda

Amazon Redshift

Amazon SageMaker Feature Store


