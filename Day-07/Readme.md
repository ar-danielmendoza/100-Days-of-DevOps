# Consigna

Set up a password-less authentication from user thor on jump host to all app servers through their respective sudo users.

Pasos a seguir:
1. Crear keys ed25519 para conectarnos sin usur contraseña.
2. Copiar public key a cada servidor.
3. Verificar conexión.

## 1. Debemos crear las claves ed25519 en nuestro jump host.

```
ssh-keygen -t ed25519
```
## 2. Luego copiamos la public key cada servidor e ingresamos la contraseña.

```
ssh-copy-id tony@stapp01
```

```
ssh-copy-id steve@stapp02
```

```
ssh-copy-id banner@stapp03
```

## 3. verificar conexión a cada servidor.

```
ssh tony@stapp01
```

```
ssh steve@stapp02
```

```
ssh banner@stapp03
```
