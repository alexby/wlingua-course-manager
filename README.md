This repository includes docker images used on [Wlingua.com](http://www.wlingua.com) for dev.

## Usage example

`docker-compose.yml`

```yaml
version: "3"
services:
  web:
    image: alexby/wlingua-course-manager-web
    ports:
      - "80:80"
    volumes:
      - ./:/var/www/html/
```