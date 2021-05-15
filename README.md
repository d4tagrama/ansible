### Uso rapido

Agregar la IP en el archivo `/etc/ansible/hosts` y ejecutar el comando:
```bash
    ansible-playbook -u usradm <playbook.yml>  --extra-var "major_version=<major_version>"
```

Donde:
* `<playbook.yml>`: Archivo playbook para aplicar
* `major_version`: Variable general para indicar la versión mayor de PHP ejemplo: 7

**Nota**: Este playbook es solo para instalar php 7.2
Ver playbook [Descargar](ansible/centos-php.yml)