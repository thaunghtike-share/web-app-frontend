# student-registration-form

Student registration UI

## Local Run

```bash
docker build \
  --build-arg VITE_API_URL=http://localhost \
  -t student-registration-form .

docker run -d -p 3000:80 student-registration-form
```

Open:

```text
http://localhost:3000
```

## Kubernetes Build Arg

Use the backend service name on port 80 in cluster:

```bash
docker build \
  --build-arg VITE_API_URL=http://web-app-backend \
  -t student-registration-form .
```
