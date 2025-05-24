# 🔍 Proceso técnico del proyecto

## 1. Recepción del archivo original

- 3 hojas separadas: Semis, Tractores y Tanques
- Filas duplicadas, campos inconsistentes
- Sin validación de datos, sin estructura

## 2. Limpieza y transformación en Google Sheets

- Unificación en una hoja única (`Disponibilidad unificada`)
- Agregado de columna `Tipo` para distinguir remolques
- Fórmula condicional en columna `Estado` según fechas y confirmación
- Validación de datos en `Estado` y `Confirmación`
- Formato condicional con color por estado (disponible, no disponible, en viaje, etc.)

## 3. Conexión con Looker Studio

- KPI de unidades disponibles hoy (`Estado = "Disponible"`)
- KPI de próximas unidades disponibles (`MIN(Disponible desde)` con filtros)
- Filtros por período, tipo y estado
- Gráficos de torta, barras y tabla interactiva

## 4. Documentación y publicación

- Subida a GitHub como caso real de transformación de datos para logística
- Video corto tipo reel mostrando antes y después del sistema
