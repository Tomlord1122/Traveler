# Web Programming #HW4

## Run the project

**_Modified from Notion Clone_**

1. Install dependencies
   ```bash
   yarn
   ```
2. Get Pusher credentials and Setup Google credentials

   Please refer to the [Google Setup](https://developers.google.com/identity/protocols/oauth2/web-server?hl=zh-tw)

   Please refer to the [Pusher Setup](https://github.com/ntuee-web-programming/112-1-unit2-notion-clone#pusher-setup) section in Notion Clone README for more details.

3. Create `.env.local` file in the project root and add the following content:

````
POSTGRES_URL=postgres://postgres:postgres@localhost:5432/traveler

PUSHER_ID=
NEXT_PUBLIC_PUSHER_KEY=
PUSHER_SECRET=
NEXT_PUBLIC_PUSHER_CLUSTER=

AUTH_SECRET=
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=

NEXT_PUBLIC_BASE_URL=http://localhost:3000
```



4. Start the database
```bash
docker compose up -d
```

5. Run migrations
   ```bash
   yarn migrate
   ```
6. Start the development server
   ```bash
   yarn dev
   ```
7. Open http://localhost:3000 in your browser

## Features

###登入畫面
<img width="1116" alt="image" src="https://github.com/Tomlord1122/Traveler/assets/79390871/ad591a60-e1d3-4508-aaa9-ca33d7772524">
###系統畫面
<img width="1174" alt="image" src="https://github.com/Tomlord1122/Traveler/assets/79390871/3fb1a457-e6f4-421b-b404-7cc56caa3b09">



1. 可以新增Plan
2. 在這裡可以選擇要編輯的Plan
3. 之後還是可以修改Plan的name以及description
4. 可以新增行程
5. 在這邊可以查看行程並且可以重新編輯
6. 可以分享給你的好友並且可以同步即時編輯
7. 最後可以輸出到你的Google Calender
````
