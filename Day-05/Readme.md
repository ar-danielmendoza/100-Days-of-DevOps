# Consigna
Install the required SELinux packages. 

Permanently disable SELinux for the time being; it will be re-enabled after necessary configuration changes.

No need to reboot the server, as a scheduled maintenance reboot is already planned for tonight.

Disregard the current status of SELinux via the command line; the final status after the reboot should be disabled.

Pasos a seguir:
1. Conectar por ssh.
2. Instalar selinux.
3. deshabilitar.
4. Verificar cambios realizados.

## 1. Conectar por ssh al servidor.
```
ssh chiquito@appserver
```

## 2. Instalar selinux.
```
yum install -y selinux-policy selinux-policy-targeted policycoreutils
```
## 3. Realizamos los cambios en /etc/selinux/config, modificando la linea.

```
SELINUX=disabled
```

## NOTA: El ejemplo pide no reiniciar, así que podemos validar hasta que se reinicie el servidor o servicio.
