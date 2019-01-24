# dart-docker-putraxor
Dart docker runtime

Build and push image:
```
docker build --rm -f "DockerFile" -t putraxor/dart_putraxor:latest .
docker tag putraxor/dart_putraxor:latest putraxor/dart_putraxor
docker push putraxor/dart_putraxor:latest
```