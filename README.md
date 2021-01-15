##Launch

Download Docker to your machine.

Execute:

`docker-compose up -d --build` - building and starting docker containers.

`mkdir ./config/jwt` - creating dir for jwt ssl.

`openssl genpkey -out ./config/jwt/private.pem -aes256 -algorithm rsa -pkeyopt rsa_keygen_bits:4096`

`openssl pkey -in ./config/jwt/private.pem -out config/jwt/public.pem -pubout`

#Backend
`127.0.0.1:88`

`127.0.0.1:81/api/doc` - Api documentation

Your rest application is build. Good luck with developing process.
