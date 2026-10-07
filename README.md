# Conciertos Chile (datos)

Próximos conciertos en Santiago, actualizados automáticamente 2 veces al día. Pensado para pantallas y
proyectos personales (por ejemplo, una ESP32).

| Archivo | Contenido |
|---|---|
| `proximos.json` | Solo los próximos 20 eventos (pequeño, para dispositivos). |
| `conciertos.json` | Lista completa de eventos futuros que cumplen el filtro. |

URL de descarga directa:
`https://raw.githubusercontent.com/<usuario>/conciertos-datos/main/proximos.json`

## Formato
```json
{"updated":"2026-10-07T02:30Z","events":[
  {"title":"BTS - World Tour ARIRANG","date":"2026-10-14","dates":["2026-10-14","2026-10-16","2026-10-17"],"venue":"Estadio Nacional","sources":["Ticketmaster"]}
]}
```
- `date`: primer día del evento (`YYYY-MM-DD`). `dates`: **todas** las fechas exactas del evento, en orden
  (pueden no ser consecutivas: en el ejemplo no hay función el 15).
- `sources`: ticketera donde se publica el evento.

## Criterio de selección
Solo conciertos en Santiago, sin festivales con varios artistas, y de artistas con una audiencia
considerable (la popularidad se consulta en Last.fm; los números no se publican).

## Aviso
Datos recopilados de listados públicos de ticketeras, sin carácter oficial. Pueden estar incompletos
o desactualizados: la ticketera de origen es la fuente de verdad en fechas, precios y disponibilidad.
