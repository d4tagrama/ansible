
Lista de archivos:

* [CentOS-PHP](ansible/centos-php.yml)


### Uso rapido

Agregar la IP en el archivo `/etc/ansible/hosts` y ejecutar el comando:
```bash
    ansible-playbook -u usradm <playbook.yml>  --extra-var "major_version=<major_version>"
```

Parametros:
* `<playbook.yml>`: Archivo playbook para aplicar
* `<major_version>`: Variable general para indicar la versión mayor de PHP ejemplo: 7



Examples:

1. Instalar php 7.2

	`ansible-playbook -u usradm centos-php.yml  --extra-vars '{"major_version":7,"enablerepo":remi-php72}'`


