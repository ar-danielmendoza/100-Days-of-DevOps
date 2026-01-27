# Consigna

Set up a password-less authentication from user thor on jump host to all app servers through their respective sudo users.


##Debemos crear las claves ed25519 en nuestro jump host.

```
ssh-keygen -t ed25519
```
## Luego copiamos la public key cada servidore e ingresamos la contraseña.

```
ssh-copy-id tony@stapp01
```

```
ssh-copy-id steve@stapp02
```

```
ssh-copy-id banner@stapp03
```
