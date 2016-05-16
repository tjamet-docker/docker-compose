# docker-compose
A simple dockerfile to provide smallest docker-compose image

Simply run `cat docker-compose.yml | docker run --rm -i -v /var/run/docker.sock:/var/run/docker.sock tjamet/docker-compose -f - config`

or

`docker run --rm -v $PWD/docker-compose.yml:/docker-compose.yml:ro -v /var/run/docker.sock:/var/run/docker.sock tjamet/docker-compose config`
