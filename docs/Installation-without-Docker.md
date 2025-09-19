### Prerequisites
- git
- Node.js >= v14.0.0

### Downloading source code
```sh
git clone https://github.com/spiicytuna/flame
cd flame

# installing dependencies (it might take some time)
npm run dev-init
```

### Building client
```sh
cd client
npm run build
```

Then create `data` and `public` directories in the project root directory. Move all content of `client/build` to the `public` directory.

### Running
Edit `.env` file in the root directory
```sh
NODE_ENV=production
PASSWORD=your_password
```

Start Flame with:
```sh
node server.js
```

Wait till server starts. You should get following logs in the terminal:
```sh
[2021-11-14 23:36:40.389 UTC+0] [INFO] Connected to database
[2021-11-14 23:36:40.585 UTC+0] [INFO] Executing pending migrations
[2021-11-14 23:36:41.284 UTC+0] [INFO] Socket: listen
[2021-11-14 23:36:41.288 UTC+0] [INFO] Server is running on port 5005 in production mode
```

Flame is now running. Visit it at `localhost:5005`