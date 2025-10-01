## Задача 1
Создаю контейнер с конфлюенсом на основе образа из Docker Hub и запускаю:

```bash
sudo docker run -v /data/your-confluence-home:/var/atlassian/application-data/confluence --name="confluence" -d -p 8090:8090 -p 8091:8091 atlassian/confluence
```

Проверяю:

```bash
sudo docker ps
```

<img width="1468" height="87" alt="image" src="https://github.com/user-attachments/assets/b0f78e20-81d9-4ffc-88a4-3625acd6d461" />
<img width="1608" height="534" alt="image" src="https://github.com/user-attachments/assets/a942630d-b9db-4295-a2e7-0cacc8040b5a" />

Останавливаю контейнер и провряю

```bash
sudo docker stop f7d54b8b175e
sudo docker ps -a
```

<img width="1464" height="87" alt="image" src="https://github.com/user-attachments/assets/26fe248d-2b10-4e4c-abd5-fa0431807420" />

Удаляю контейнер и проверяю

```bash
sudo docker rm f7d54b8b175e
sudo docker ps -a
```

<img width="1087" height="68" alt="image" src="https://github.com/user-attachments/assets/216a737e-7a8f-49e0-b3c7-ce96021fc304" />

## Задача 2


```bash
sudo docker images
```

<img width="741" height="132" alt="image" src="https://github.com/user-attachments/assets/7fc22291-acd7-45f1-bd8b-e3bc71cf9564" />






