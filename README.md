# spring-security-keycloak-react-angular

http://localhost:8080/auth/realms/Demo-Realm/protocol/openid-connect/auth

http://localhost:8080/auth/realms/Demo-Realm/protocol/openid-connect/token

https://stackoverflow.com/questions/46073485/keycloak-spring-security-client-credential-grant/46400975

https://stackoverflow.com/questions/53118828/keycloak-public-client-and-authorization

https://sandor-nemeth.github.io/java/spring/2017/06/15/spring-boot-with-keycloak.html

https://scalac.io/user-authentication-keycloak-1/

{ "error": "invalid_grant", "error_description": "Account is not fully set up" }
https://stackoverflow.com/questions/42524153/keycloak-not-returning-access-token-if-update-password-action-selected
https://www.janua.fr/understanding-token-usage-in-keycloak/

https://stackoverflow.com/questions/62082685/how-to-get-user-details-from-keycloak-not-logged-in-user-but-any-user-by-his-id/62083431#62083431

POST http://localhost:8080/auth/realms/<my_realm>/protocol/openid-connect/logout
access type = public
if access type = Credential/beareronly then client_secret required
Content-Type: application/x-www-form-urlencoded
curl -L -X POST  --insecure 'http://localhost:8080/auth/realms/Demo-Realm/protocol/openid-connect/token' \
-H 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'client_id=tutorial-backend' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'client_secret=2bd8c133-91f1-49d3-8636-d9ef3f0131b1' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username=a' \
--data-urlencode 'password=123456'

--data-urlencode 'grant_type=refresh_token' \

https://geeks18.com/?p=1347
