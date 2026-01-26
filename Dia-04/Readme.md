Your task is to grant executable permissions to the /tmp/xfusioncorp.sh script on App Server. Additionally, ensure that all users have the capability to execute it.

Conectar por ssh al servidor por ssh.

Luego deberemos agregar permisos de lectura y ejecución.
```
chmod a+rx /tmp/xfusioncorp.sh
```

Verificamos que se asignaron correctamente los permisos, necesariamente debemos asignar permisos de lectura, para que pueda validarse que este el script sin necesidad de ejecutarlo.
```
ls -lah /tmp/xfusioncorp.sh
```
