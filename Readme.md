
# Install

```
docker build -t web-dieteticienne-micronutrition.fr .

docker run -d \
-e LETSENCRYPT_HOST=www.dieteticienne-micronutrition.fr \
-e LETSENCRYPT_EMAIL=lucas.cherifi@gmail.com \
-e VIRTUAL_HOST=www.dieteticienne-micronutrition.fr \
--network=webproxy \
--name www.dieteticienne-micronutrition.fr \
web-dieteticienne-micronutrition.fr:latest
```
