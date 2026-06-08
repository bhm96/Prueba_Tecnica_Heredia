# Arquitectura Cloud-Native en AWS

## Descripción

Este repositorio contiene el diseño de una arquitectura cloud-native basada en Amazon Web Services (AWS), junto con la documentación técnica que justifica la selección de los servicios utilizados y las decisiones de diseño adoptadas.

La solución propuesta considera aspectos de escalabilidad, alta disponibilidad, seguridad y observabilidad mediante servicios administrados de AWS.

---

## Objetivos

- Diseñar una arquitectura cloud-native moderna.
- Utilizar servicios administrados de AWS.
- Garantizar alta disponibilidad y escalabilidad.
- Implementar mecanismos de seguridad y monitoreo.
- Documentar la solución y sus componentes.

---

## Servicios AWS Utilizados

### Frontend
- Amazon S3
- Amazon CloudFront

### Backend
- Amazon API Gateway
- Amazon ECS Fargate

### Base de Datos
- Amazon RDS PostgreSQL (Multi-AZ)

### Almacenamiento
- Amazon S3

### Seguridad
- AWS WAF
- AWS IAM
- AWS Secrets Manager

### Observabilidad
- Amazon CloudWatch
- Amazon SNS

---

## Flujo General

1. El usuario accede a la aplicación a través de Internet.
2. AWS WAF protege la aplicación contra amenazas web.
3. CloudFront distribuye el contenido estático alojado en S3.
4. API Gateway recibe las solicitudes del frontend.
5. ECS Fargate ejecuta la lógica de negocio.
6. RDS PostgreSQL almacena la información persistente.
7. S3 almacena imágenes y documentos.
8. CloudWatch monitorea los servicios y SNS envía alertas.

---

## Estructura del Repositorio

```text
.
├── README.md
├── Prueba_Heredia.drawio
└── Reto_Técnico_Heredia.pdf
```

---

## Archivos Incluidos

### Prueba_Heredia.drawio
Diagrama de arquitectura elaborado en Draw.io que representa la solución cloud-native propuesta.

### Reto_Técnico_Heredia.pdf
Documento técnico que describe la arquitectura, los componentes utilizados, el flujo de funcionamiento y la justificación de las decisiones de diseño.

---

## Características de la Arquitectura

- Arquitectura Cloud-Native.
- Alta disponibilidad mediante Multi-AZ.
- Escalabilidad horizontal con ECS Fargate.
- Seguridad mediante WAF, IAM y Secrets Manager.
- Monitoreo y observabilidad con CloudWatch.
- Almacenamiento seguro y duradero con Amazon S3.

---

## Autor

Brayan Heredia

---

## Licencia

Proyecto desarrollado con fines académicos y educativos.
