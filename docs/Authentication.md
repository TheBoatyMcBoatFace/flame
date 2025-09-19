### Set custom password
To set your own password, simply pass `PASSWORD=your_password` environment variable to your `docker run` command or your `docker-compose` file.

> If custom password is not provided, default password `flame_password` will be used.

- Command example
```bash
docker run -p 5005:5005 -v /path/to/data:/app/data -e PASSWORD=my_password flame
```

- File example
```yaml
version: '2.1'
services:
  flame:
    image: spiicytuna/flame:latest
    container_name: flame
    volumes:
      - <host_dir>:/app/data
    ports:
      - 5005:5005
    environment:
       - PASSWORD=my_password
    restart: unless-stopped
```

### Login
To login, go to `Settings > App`. Authentication section contains form with two inputs:
- **password**: your password
- **session duration**: how long auth token should be valid for

### Access
Authenticated user has access to:
- all apps
- all categories
- all bookmarks
- all editors
- all settings

Guest user has access to:
- all apps set to public (homescreen - only pinned, apps - all public apps)
- all categories set to public (homescreen - only pinned, bookmarks - all public categories)
- all bookmarks set to public (homescreen/bookmarks - only if parent category is set to public)
- Theme and App sections of settings

> If category is set to `hidden`, all bookmarks associated with it will also be hidden. Setting `visible` on specific bookmark **will not be respected**.