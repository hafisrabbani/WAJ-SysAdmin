# Getting our App into PWD
1. Download Getting Started with PWD
2. Download file menggunakan wget:
```wget http://ip172-18-0-53-cp4cola91nsg00ebdma0-80.direct.labs.play-with-docker.com/assets/app.zip```
![download](./img/1.png)
3. Unzip the file:
```unzip app.zip```
![unzip](./img/2.png)
4. Edit Dockerfile: 
    ```vim Dockerfile```

    ![vim](./img/3.png)
5. Isi Dockerfile:
    ```
    FROM node:18-alpine
    WORKDIR /app
    COPY . .
    RUN yarn install --production
    CMD ["node", "src/index.js"]
    ```
    ![vim](./img/4.png)
6. Build Docker image:
```docker build -t getting-started .```
![build](./img/5.png)
7. Run Docker image:
```docker run -d -p 3000:3000 getting-started```
8. Buka port 3000 dari instance PWD:
```http://ip172-18-0-53-cp4cola91nsg00ebdma0-3000.direct.labs.play-with-docker.com/```
![run](./img/6.png)

