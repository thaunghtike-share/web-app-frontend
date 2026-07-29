# student-registration-form

Student registration frontend for the backend API.

## Environment

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

## Docker Build For Backend

```bash
docker build \
  --build-arg VITE_API_URL=http://web-app-backend.ecs.local:8000 \
  -t student-registration-form .
```

## Container Port

```text
80
```

## Notes

The app uses:

```js
import.meta.env.VITE_API_URL
```
