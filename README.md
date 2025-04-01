# *DOCKER COMPOSE*

![image](https://github.com/user-attachments/assets/79a188a0-855b-49bf-b98c-d1fe53a97937)

- Установка `гостевых дополнений` Linux

![image](https://github.com/user-attachments/assets/aec98eea-ba1b-4a29-b988-cb77ec7828d3)

- `sudo yum install wget ` производим установку пакета wget.
  
- `sudo yum install curl ` производим установку пакета curl.

![image](https://github.com/user-attachments/assets/f7651679-b7f0-4e2b-bd68-906f896a14ca)

- `sudo wget -P /etc/yum.repos.d/` установка docker.

![image](https://github.com/user-attachments/assets/ac92c472-5f0d-41d8-966c-6330051da7b3)

- `sudo yum install docker-ce docker-ce-cli containerd.io` установка docker.

![image](https://github.com/user-attachments/assets/5c5f0ee0-d259-4f30-ba19-047cc209a6db)

![image](https://github.com/user-attachments/assets/9678f515-698f-4451-98e3-b8a586e76da9)

- `sudo systemctl enable docker --now` запуск docker и разрешение на его автозапуск.

![image](https://github.com/user-attachments/assets/751da184-f766-4472-91c0-800803fea6cb)

- `COMVER=$(curl -s https://api.github.com/repos/docker/compose/releases/latest | grep 'tag_name' | cut -d\" -f4)` получение последней актуальной версии docker.

![image](https://github.com/user-attachments/assets/5b6faee9-d8be-4e24-9c10-be7a09d47566)

- `sudo curl -L "https://github.com/docker/compose/releases/download/$COMVER/docker-compose-$(uname -s)-$(uname -m)" -o /usr/bin/docker-compose` загрузка и установка последней версии docker.

![image](https://github.com/user-attachments/assets/24f7723a-ad82-4324-99ba-0d45354dc408)

- `sudo chmod +x /usr/bin/docker-compose` docker становится исполняемым.

![image](https://github.com/user-attachments/assets/ad126c81-d088-433e-898d-f06ac2ee6450)

- `git clone https://github.com/skl256/grafana_stack_for_docker.git` клонирование репозитория

![image](https://github.com/user-attachments/assets/90a10806-e9fd-4e5a-b336-f0f994129f85)

- `cd grafana_stack_for_docker` смена директории.

![image](https://github.com/user-attachments/assets/ca35f718-187b-446d-a866-9a8c656e1324)

- `sudo docker compose up -d` создание и запуск контейнеров.

![image](https://github.com/user-attachments/assets/4efb8b54-c984-4df6-886e-790545145541)

![image](https://github.com/user-attachments/assets/cbffa0e8-9a03-4d88-bad6-add9728c8e44)

- `sudo docker compose stop` остановка контейнеров (не удаляет).

![image](https://github.com/user-attachments/assets/bcb8fcf5-c13c-4dc5-bef0-13a0a725d33e)

- `sudo docker compose down` остановка и удаление всех контейнеров.

![image](https://github.com/user-attachments/assets/01e65ef3-ae19-40a0-b7f7-78dd130e6156)

- `sudo vi docker-compose.yaml` открытие файла docker-compose.yaml в текстовом редакторе

![image](https://github.com/user-attachments/assets/817c7770-47e3-45a7-8816-4e353f64166f)

- `cd /mnt/common_volume/swarm/grafana/config` создание папки с указанным путем

![image](https://github.com/user-attachments/assets/727689de-2164-4482-9d14-bf4c34650498)

- меняем на `exporter:9100`

![image](https://github.com/user-attachments/assets/81e018b7-9517-4173-9be9-7a747cb3eb38)


# *GRAFANA*

- вход в графану `localhost:3000`

![image](https://github.com/user-attachments/assets/6a16a55f-d7d3-4ae3-b3a8-6cfed6fe516c)

- начальный экран графаны

![image](https://github.com/user-attachments/assets/98f20339-ede7-4875-89cb-c23600b1a0e4)

- создание нового дашборда с `prometheus`

![image](https://github.com/user-attachments/assets/9b014b92-fe75-4e25-aa3e-1352999aa714)

![image](https://github.com/user-attachments/assets/fb52dff2-7a9d-42a6-a3dc-ab357d3d7c01)

- подключение `prometheus:9090`

![image](https://github.com/user-attachments/assets/ddb1b200-f8cf-4f30-8f91-7ca607aa153a)

![image](https://github.com/user-attachments/assets/6c70426f-a42e-4295-b573-2ac1e1b43834)

- импорт дашборда `1860`.

![image](https://github.com/user-attachments/assets/3f380773-5873-4213-9c20-4dd50ec4f465)

![image](https://github.com/user-attachments/assets/3d140a50-9375-4094-80e6-ff709cb33cd1)

- `CPU` мониторинг процессов.

![image](https://github.com/user-attachments/assets/08cab9fe-8393-4a55-82fe-15491dd79019)


