## Top Level
## invidious

|    | invidious | [mediacms.io](http://mediacms.io) |    |    |
|----|----|----|----|----|
| Git | <https://github.com/iv-org/invidious> | <https://github.com/mediacms-io/mediacms> |    |    |
| Docu | [https://docs.invidious.io](https://docs.invidious.io/) | \* [Users documentation](https://github.com/mediacms-io/mediacms/blob/main/docs/user_docs.md) \n \* [Administrators documentation](https://github.com/mediacms-io/mediacms/blob/main/docs/admins_docs.md) \n \* [Developers documentation](https://github.com/mediacms-io/mediacms/blob/main/docs/developers_docs.md) |    |    |
|    |    |    |    |    |
| clab | [http://192.168.178.124:3210](http://192.168.178.124:3210/) | [http://192.168.178.124:105](http://192.168.178.124:105/) |    |    |
| Public? | nope | nope |    |    |
| admin | cmuc:pw | cmuc:pw |    |    |
| Database | PG Admin local 5432 | PG Admin local 5433 | h |    |
|    | [\\docker\\data\\invidious\\docker-compose.yml](\\\\192.168.178.124\\docker\\data\\invidious\\docker-compose.yml) | [\\docker\\data\\mediacms\\docker-compose.yaml](\\\\192.168.178.124\\docker\\data\\mediacms\\docker-compose.yaml) |    |    |
|    |    |    |    |    |
|    |    |    |    |    |

* 12321
* 232
* 213

#### Updating a Docker install

<https://docs.invidious.io/installation/#updating-a-docker-install>

```bash
docker-compose pull
```

```bash
docker-compose up -d
```

```bash
docker image prune -f
```

## [mediacms.io](http://mediacms.io)

#### local env

cmuc:password

#### Github

#### Updating a Docker install

<https://github.com/mediacms-io/mediacms/blob/main/docs/admins_docs.md#update-1>

```bash
cd /path/to/mediacms/installation
docker pull mediacms/mediacms
docker-compose down
docker-compose up
```