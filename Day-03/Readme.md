Your task is to disable direct SSH root login on all app servers within the Datacenter.

Luego de loguearme y elevar privilegios en cada servidor debo:

## cambiar configuraciones en el archivo

```
sudo vi /etc/ssh/sshd_config

```

Buscar PermitRootLogin y cambiar `yes` por `no`
```
PermitRootLogin no
``` 

Reiniciar servicios ssh
```
sudo systemctl restart sshd
```
