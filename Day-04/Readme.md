# Consigna
Your task is to grant executable permissions to the /tmp/xfusioncorp.sh script on App Server. Additionally, ensure that all users have the capability to execute it.
Pasos a seguir:
1. Conectar por ssh.
2. agregar permisos de lectura y ejecución.
3. verificar permisos asignados.

## 1. Conectar por ssh al servidor.
```
ssh chiquito@appserver
```

## 2. Luego deberemos agregar permisos de lectura y ejecución.
```
chmod a+rx /tmp/xfusioncorp.sh
```
## 3. Verificamos que se asignaron correctamente los permisos.
```
ls -lah /tmp/xfusioncorp.sh
```

## NOTA: debemos asignar permisos de lectura, para que pueda validarse que este el script sin necesidad de ejecutarlo.
