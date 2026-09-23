# VB6-Formatos

Catálogo de formatos de impresión para los programas de gestión Doscar / Prosicar.

Cada carpeta corresponde a un programa y contiene los formatos disponibles para él.
Los formatos **no se comparten entre programas**.

```
<programa>/
  indice.json        lista de formatos disponibles
  <formato>.json     el formato (medidas y campos)
```

## `indice.json`

```json
{
  "programa": "gestion",
  "actualizado": "2026-09-23",
  "formatos": [
    {
      "id": "factura-a4",
      "fichero": "Facturas de Venta",
      "nombre": "Factura A4",
      "descripcion": "Factura a página completa con desglose por tipo de IVA.",
      "fecha": "2026-09-23"
    }
  ]
}
```

- `fichero` es el tipo de documento al que se aplica el formato.
- `id` es el nombre del fichero `.json` del formato.

## Uso

Desde el programa, en el mantenimiento de formatos de impresión, hay un botón para
ver los formatos disponibles e importar los que se quieran. Cada importación crea
un formato nuevo en la empresa activa: **nunca modifica ni borra los existentes**.
