The Nautilus system admins team has prepared scripts to automate several day-to-day tasks. They want them to be deployed on all app servers in Stratos DC on a set schedule. Before that they need to test similar functionality with a sample cron job. Therefore, perform the steps below:



a. Install cronie package on all Nautilus app servers and start crond service.


b. Add a cron */5 * * * * echo hello > /tmp/cron_text for root user.


Para realizar la consigna deberemos:

1. conectarnos a cada App server.
2. Instalar el paquete cronie.
3. Habilitar e iniciar el servicio.
4. configurar la tarea (cron).
5. verificar que funciona la tarea.


## 1
```
ssh usuario@servidor
```

## 2
```
sudo yum install -y cronie
```

## 3
```
sudo systemctl enable crond
sudo systemctl start crond
systemctl status crond
```

## 4 
```
sudo crontab -e
```
Agregar en la primer linea.
```
*/5 * * * * echo hello > /tmp/cron_text
```

## 5
```
sudo crontab -l
```

```
cat /tmp/cron_text
```
