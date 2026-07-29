# student-registration-form

Student registration UI

## Local Run

```bash
docker build \
  --build-arg VITE_API_URL=http://localhost:8000 \
  -t student-registration-form .

docker run -d -p 3000:80 student-registration-form
```

Open:

```text
http://localhost:3000
```
