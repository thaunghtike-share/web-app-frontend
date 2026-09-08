## student-registration-form

Student registration UI

### Local Run

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

### Castone GitOps

For the Helm deployment, CI builds with:

```text
VITE_API_URL=http://web-app-backend.castone.svc.cluster.local:8000
```

After publishing, set the new image tag in
`amm-castone/helm_charts/web-app-frontend/values.yaml`.
The local Docker example above still uses an explicit backend URL.
