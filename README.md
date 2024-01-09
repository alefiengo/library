# library

```
version: '3.8'

services:
  installer:
    image: composer:latest
    volumes:
      - ./:/app
    working_dir: /app
    ports:
      - 8000:8000
```

```
$ curl -sS https://get.symfony.com/cli/installer | bash
$ symfony new library
```