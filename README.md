# ansible-lab
Playbook de ansible para instanciar un POD en AWS para el curso "Advanced Network Programmability" de CONATEL S.A.

## Requerimientos

Para poder correr los `playbooks` es necesario precargar las siguientes variables de entorno:

- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY

## Levantar el Lab

```bash
ansible-playbook pod_up.yml
```

## Archivos generados

Tras ejecutar el `playbook` se generarán dos archivos en la carpeta `secret_vars`:

- `pod_X.yml`: contiene información de los recursos generados para el POD.
- `key_pair_X`: corresponde a la llave privada a utilizar para conectarse con los servidores.

_OBS: La `X` corresponde al número de POD utilizado._

## Eliminar el lab

```bash
ansible-playbook pod_down.yml
```

## Licencia 

[MIT](./LICENCE)

## Autores

- Ismael Almandos
- Guzmán Monné

## Copyright

CONATEL S.A. 2018
