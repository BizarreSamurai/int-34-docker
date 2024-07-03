# int-34-docker
## Как запустить?

Сборка Docker образа: __docker build -t python-server .__

Запуск Docker контейнера: __docker run -p 8000:8000 my-python-server__

## Как проверить?

При запросе __curl -i localhost:8000/healthz__ получаем:
'''bash
HTTP/1.0 200 OK
'''
В иных случаях:
'''bash
HTTP/1.0 404 Not Found
'''
