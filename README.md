Start keycloak via podman in dev mode
podman run -p 8080:8080 -e KC_BOOTSTRAP_ADMIN_USERNAME=admin -e KC_BOOTSTRAP_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:26.1.0 start-dev

login
http://localhost:8080/

with
admin
admin

Create a
new Realm
new Clients -> set Client ID
new User -> set example User

Create CHAINLIT_AUTH_SECRET for chainlit
chainlit create-secret

and add the secret to your .env

