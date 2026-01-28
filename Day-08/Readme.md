# Consigna
Install ansible version 4.8.0 on Jump host using pip3 only. Make sure Ansible binary is available globally on this system, i.e all users on this system are able to run Ansible commands.

Pasos a seguir:
1. Verificar que este disponible ansible 4.8.0.
2. Instalar ansible 4.8.0.
3. Verificar cambios realizados.

## 1. Verificamos con pip3 las versiones disponibles de Ansible.
```
pip3 index versions ansible

```

## 2. Instalar ansible usando pip3.
```
pip3 install ansible==4.8.0
```
## 3. Verificamos la version de ansible instalada.

```
ansible --version
```

## NOTA: El ejemplo pide no reiniciar, así que podemos validar hasta que se reinicie el servidor o servicio.
