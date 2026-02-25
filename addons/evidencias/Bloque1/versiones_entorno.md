# Versiones por entorno (DEV / QA / PROD)
## Comandos utilizados

### Odoo

- `sudo docker exec -it odoo-dev odoo --version`
- `sudo docker exec -it odoo-qa odoo --version`
- `sudo docker exec -it odoo-prod odoo --version`

### PostgresSQL

-`sudo docker exec -it postgres-dev postgres --version`
-`sudo docker exec -it postgres-prod postgres --version`
-`sudo docker exec -it postgres-qa postgres --version`

### Apache Hop

-Imagen detectada por `Docker ps -a`: `apache/hop:2.17.0`
- `sudo docker exec hop-dev /opt/hop/hop-conf.sh -v`
- `sudo docker exec hop-qa /opt/hop/hop-conf.sh -v`
- `sudo docker exec hop-prod /opt/hop/hop.sh -v`

## Tabla de versiones
| Entorno | Odoo | `pstgres| Hop PostresSQL 16.11 | Hop | 
|---|---|---|---|
|DEV | Odoo Server 18.0-20251121 | postgres (PostgresSQL) 16.11 | apache/hop:2.17.0 |
|QA  | Odoo Server 18.0-20251121 | postgres (PostgresSQL) 16.11 | apache/hop:2.17.0 |
|PROD | Odoo Server 18.0-20251121 | postgres (PostgresSQL) 16.11 | apache/hop:2.17.0 |

## Observaciones

- Odoo y PostgreSQL están alineados en los tres entornos (misma versión).
- Hop también está alineado por el tag de la imagen (`2.17.0`).