# Identificación de cuellos de botella

## Cuellos detectados

| Tipo | Problema | Impacto | Gravedad |
|----|---------|--------|---------|
| Hardware | Memoria RAM insuficiente | Alto | Alta |
| Software | Errores recurrentes de aplicaciones (ID 1000) | Alto | Alta |
| Configuración | Servicios innecesarios al arranque | Medio | Media |
| Configuración | Errores DistributedCOM (ID 10010) | Bajo | Media |
| Uso | Uso intensivo de aplicaciones simultáneas | Medio | Media |

## Justificación técnica

- **RAM insuficiente:** alto consumo observado y quejas de usuarios por lentitud.
- **Errores de aplicaciones:** cierres inesperados registrados en el visor de eventos.
- **Servicios al arranque:** retraso en el inicio del sistema.
- **DistributedCOM:** errores de permisos sin impacto crítico.
- **Uso intensivo:** múltiples aplicaciones abiertas simultáneamente.
## Justificación técnica

### 1️⃣ RAM insuficiente
- Detectado alto consumo en pruebas de rendimiento
- Usuarios reportan lentitud al trabajar con varias aplicaciones
- Provoca cierres inesperados de aplicaciones

### 2️⃣ Errores recurrentes de aplicaciones
- Eventos ID 1000 repetidos en el visor de eventos
- Relación directa con cierres inesperados
- Impacto directo en la experiencia de usuario

### 3️⃣ Servicios innecesarios en el arranque
- Retraso en el inicio del sistema
- Mayor consumo de recursos
- Detectado en entrevistas y observación del sistema

### 4️⃣ Errores DistributedCOM
- Problema de permisos o configuración
- No crítico pero recurrente
- Puede generar ruido en logs

### 5️⃣ Malas prácticas de uso
- Usuarios mantienen múltiples aplicaciones abiertas
- Incremento del consumo de RAM y CPU
## Conclusión

Los principales cuellos de botella están relacionados con la gestión de recursos y errores de aplicaciones. 
La falta de optimización del software y la configuración del sistema impactan directamente en el rendimiento percibido por los usuarios.