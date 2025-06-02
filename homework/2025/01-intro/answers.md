# Answers

1. dbcbbbd0bc4924cfeb28929dc05d82d662c527b7
2. index
3. 44.50
4. "How do I copy files from a different folder into docker container’s working directory?"
5. 1446
6. 320

# Solution

1. ```{bash}

docker run -it \
    --rm \
    --name elasticsearch \
    -m 4GB \
    -p 9200:9200 \
    -p 9300:9300 \
    -e "discovery.type=single-node" \
    -e "xpack.security.enabled=false" \
    docker.elastic.co/elasticsearch/elasticsearch:8.17.6

curl localhost:9200

```
