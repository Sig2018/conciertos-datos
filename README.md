# Conciertos Chile (datos)

`conciertos.json`: próximos conciertos en Santiago, actualizado automáticamente 2 veces al día.
Pensado para pantallas y proyectos personales (por ejemplo, una ESP32).

URL de descarga directa:
`https://raw.githubusercontent.com/<usuario>/conciertos-datos/main/conciertos.json`

## Formato
```json
{"updated":"2026-10-07T02:30Z","events":[
  {"title":"Deep Purple","date":"2026-12-08","date_end":null,"venue":"Santander Arena - Santiago Centro","sources":["PuntoTicket"]}
]}
```
- `date`: primer día del evento (`YYYY-MM-DD`). `date_end`: último día si dura varios, o `null`.
- `sources`: ticketera donde se publica el evento.

## Aviso
Datos recopilados de listados públicos de ticketeras, sin carácter oficial. Pueden estar incompletos
o desactualizados: la ticketera de origen es la fuente de verdad en fechas, precios y disponibilidad.
