# spring-keycl

docker run -p 127.0.0.1:8080:8080 \
-e KC_BOOTSTRAP_ADMIN_USERNAME=admin \
-e KC_BOOTSTRAP_ADMIN_PASSWORD=admin \
-v ./data:/opt/keycloak/data \
quay.io/keycloak/keycloak:26.5.2 \
start-dev --import-realm


export JAVA_HOME=/media/pmercado/hd2/programas/openjdk-25.0.2_linux-x64_bin/jdk-25.0.2
export M2_HOME=/media/pmercado/hd2/programas/apache-maven-3.9.9


REALMS
local-realm

USER
4833200-user
external-user

REALM ROLES
local-entidad-realmrol
local-publico-realmrol

CLIENTS
local-sicoes-pac-client
local-sicoes-us-client
