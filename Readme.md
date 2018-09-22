
# Install

```
docker build -t web-dieteticienne-micronutrition.fr .

docker run -d web-dieteticienne-micronutrition.fr \
    -e VIRTUAL_HOST=www.dieteticienne-micronutrition.fr \
    -e LETSENCRYPT_HOST=www.dieteticienne-micronutrition.fr \
    -e LETSENCRYPT_EMAIL=lucas.cherifi@gmail.com \
    --network=webproxy \
    --name dieteticienne-micronutrition.fr \
    nginx
```