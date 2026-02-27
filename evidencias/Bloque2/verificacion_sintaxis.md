# 2.2 Verificación sintáctica

Módulo: Personalización de formato de ventas  
Archivo de manifiesto detectado: manifest  
Nombre esperado por Odoo: __manifest__.py  

---

## 1) Sintaxis Python

### 1.1 Comprobación del nombre del archivo (requisito Odoo)

__Objetivo:__ verificar que el manifiesto tiene el nombre requerido por Odoo para que el módulo sea reconocido.

__Comando ejecutado:__
```bash
ls -la

drwxrwxr-x 3 user user 4096 Feb 25 13:41 .
drwxrwxr-x 3 user user 4096 Feb 25 10:28 ..
-rw-rw-r-- 1 user user    0 Feb 25 10:42 __init__.py
-rw-rw-r-- 1 user user  338 Feb 25 13:41 __manifest__.py
drwxrwxr-x 2 user user 4096 Feb 25 13:49 views



```bash

{
    "name": "Custom Sale Codes (Report)",
    "version": "1.0.0",
    "category": "Sales",
    "summary": "Añade referencia interna y código de barras al reporte de pedido",
    "depends": ["sale"],
    "data": [
        "views/sale_report.xml",
    ],
    "installable": True,
    "application": False,
    "license": "LGPL-3",
}    

```

### 1) Validación del XML

__Objetivo__ comprobar que el xml referenciado en el manifest está bien formado.

__Archivo referanciado:__

- views/sale_report.xml

### 1.1 Verificar la existencia del archivo

__Comando ejecutado:__

```bash


```
__Salida obtenida:__
```bash


```

### 1.2 Validación archivo XML (bien formado)
```bash
xmllint --noout views/sale_report.xml
echo $?
```
__Salida obtenida:__
```bash


```
__Reslutado:__
- Código de retorno
- Interpretación
    - 0 -> XML bien formado
    - Error -> indicar mensaje exacto