<div style="text-align: center;"><h1 style="color:blue"> BACKEND </h1><hr> 

### Creating BackEnd use docker-compose

#### kotlin-gradle use Ktor

#### koltin: 1.7.10 | ktor: 2.2.2 | SDK - 17.0.7

<hr>
</div>

#### Swagger Localhost

- http://localhost:8080/swagger

#### Local RUN

- Generate an SSL certificate

```bash
  keytool -genkey -alias selfsigned -keyalg RSA -keypass 123456  -storepass 123456 -keystore ssl/dev/keystore.jks
``` 

- Change in [.env.dev](.docker%2F.env.dev) the GPT_KEY variable for your gpt key


- Build and Run

```bash
./gradlew clean build
```

```bash
sudo docker-compose --env-file=.docker/.env.dev up --build
```