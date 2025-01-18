docker run -d --name keycloak -p 8080:8080 \
  -v /path/to/realm-export.json:/opt/keycloak/realm-export.json \
  -e KEYCLOAK_IMPORT=/opt/keycloak/realm-export.json \
  quay.io/keycloak/keycloak:latest start-dev
