# Incompatibilidades

## Mostrar contenido de '__manifest__.py'

`sed -n '1,200p' addons/dev/custom_sale_codes/__manifest__.py`
`sed: can't read addons/dev/custom_sale_codes/__manifest__.py: No such file or directory`

### Carga del modulo en DEV

{
    "name": "Custom Sale Codes (Report)",
    "version": "1.0.0",
    "category": "Sales",
    "summary": "Añade referencia interna y código de barras al reporte de pedido",
    "depends": ["sales"],
    "data": [
        "views/sale_report_views.xml",
    ],
    "installable": True,
    "application": False,
    "license": "LGPL-3",
}