## Building

Just do it `make build` in terminal

mkdir ./config/jwt
openssl genpkey -out ./backend/config/jwt/private.pem -aes256 -algorithm rsa -pkeyopt rsa_keygen_bits:4096
openssl pkey -in ./backend/config/jwt/private.pem -out config/jwt/public.pem -pubout

#Backend

`127.0.0.1:88`
`127.0.0.1:81/api/doc`: Api documentation
`127.0.0.1:81/api/login`: login
`127.0.0.1:81/api/v1/somePath`: routing to api
