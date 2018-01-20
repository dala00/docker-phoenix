# docker-phoenix

This repository contains a script for create [phoenix](http://www.phoenixframework.org/) server image.

You can use these tags as a version of elixir.

- `1.5.3-slim`

### docker-compose

```
app:
    image: dala00/phoenix:1.5.3-slim
    env_file: .docker-env
    volumes:
      - .:/var/opt/app
    ports:
      - "4000:4000"
    tty: true
    stdin_open: true
```