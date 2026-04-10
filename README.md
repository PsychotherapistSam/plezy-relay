this is the [plezy](https://github.com/edde746/plezy) relay server built as a docker container for easier use

it is automatically built from the upstream `edde746/plezy` repository and checked for updates hourly

use like this if u want (or don't, I dont care):

```yaml
# docker-compose.yml
services:
    relay:
        image: ghcr.io/psychotherapistsam/plezy-relay:latest
        restart: unless-stopped
        ports:
            - "8080:8080"
        volumes:
            - logs:/data/logs

volumes:
    logs:
```
