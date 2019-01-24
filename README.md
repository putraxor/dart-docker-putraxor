# dart-docker-putraxor
Dart docker runtime. It can automatically bundle a Dart application and its dependencies with
a single line Dockerfile.

Build and push image:
```
docker build --rm -f "DockerFile" -t putraxor/dart_putraxor:latest .
docker tag putraxor/dart_putraxor:latest putraxor/dart_putraxor
docker push putraxor/dart_putraxor:latest
```

## Usage

Create a `Dockerfile` in your Dart application directory with the following
content:
```
FROM putraxor/dart_putraxor:latest
ADD . /
RUN pub get
```