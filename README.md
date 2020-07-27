# SFG Brewery Cloud Config Service
Spring Boot Microservice project

## Initial run
Used the example config repo (and used clone on start):
```
spring.cloud.config.server.git.uri=https://github.com/springframeworkguru/mssc-example-config-repo
spring.cloud.config.server.git.clone-on-start=true
```

To verify the available properties use Postman with http://localhost:8888/application/profile:

```
{
    "name": "application",
    "profiles": [
        "profile"
    ],
    "label": null,
    "version": "6d7a3d2cd2cb87c18b2e116ecdad72756c21e8a2",
    "state": null,
    "propertySources": [
        {
            "name": "https://github.com/springframeworkguru/mssc-example-config-repo/application.yml",
            "source": {
                "foo": "bar"
            }
        }
    ]
}
```
