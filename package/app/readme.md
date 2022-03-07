# Application Setup Packages

This sections provides packages to setup and build a variety of projects in Kubernetes as follows:

| type | description |
|---|---|
| [quarkus](quarkus) | create a quarkus project and pipeline |
| [spring-boot](spring-boot) | create a spring-boot project and pipeline |


### Configuration variables:

| Variable  | Description  | Example  |
|---|---|---|
|**ARTISAN_REGISTRY_CPU_LIMIT**| It make sure a registry container never goes above a certain value of cpu. The container is only allowed to go up to the limit, and then it is restricted | _2_ |
|**ARTISAN_REGISTRY_CPU_REQUEST**| The amount of CPU that registry needs for standard operation | _1_ |
|**ARTISAN_REGISTRY_MEMORY_LIMIT**| It make sure a registry container never goes above a certain value of memory. The container is only allowed to go up to the limit, and then it is restricted | _2Gi_ |
|**ARTISAN_REGISTRY_MEMORY_REQUEST**| The amount of RAM memory that registry needs for standard operation (normally in Gibibytes) | _1Gi_ |
|**ARTISAN_REGISTRY_TAG**| Tags identify different versions of the same series of registry images. | _v0.0.4-d4fb6f7-031020001129_ |
|**ARTISAN_RUNNER_CPU_LIMIT**| It make sure a artisan runner container never goes above a certain value of cpu. The container is only allowed to go up to the limit, and then it is restricted | _2_ |
|**ARTISAN_RUNNER_CPU_REQUEST**| The amount of CPU that artisan runner needs for standard operation | _1_ |
|**ARTISAN_RUNNER_MEMORY_LIMIT**| It make sure a artisan runner container never goes above a certain value of memory. The container is only allowed to go up to the limit, and then it is restricted | _2Gi_ |
|**ARTISAN_RUNNER_MEMORY_REQUEST**| The amount of RAM memory that artisan runner needs for standard operation (normally in Gibibytes) | _1Gi_ |
|**ARTISAN_RUNNER_TAG**| Tags identify different versions of the same series of runner images | _eg. v0.0.4-d4fb6f7-031020001129_ |
|**CLUSTER_ACCESS_TOKEN**| The authentication token required to access the K8S cluster API In order to obtain an access token for your cluster refer to the K8S cluster implementation documentation | _vsHUC-086iksc4KO72IwrNNmpYulGMagIBVWK9R__oA_ |
|**CLUSTER_DOMAIN_NAME**|  The URI of the Kubernetes cluster inclusing protocol and port number | _https://api.ocp.domain-name.io:6443_ |
|**CLUSTER_USERNAME**| This username should be used in conjunction with CLUSTER_ACCESS_TOKEN | _admin_ |
|**NAMESPACE**| The name of the Kubernetes namespace where nexus is deployed | _amosonline-aws-01-aps-test_ |
|**IMAGE_NAMESPACE**| The name of the Kubernetes namespace where images is deployed | _amosonline-aws-01-aps-images_ |
|**DATABASE_CPU_LIMIT**| It make sure a database container never goes above a certain value of cpu. The container is only allowed to go up to the limit, and then it is restricted. | _2_ |
|**DATABASE_CPU_REQUEST**| The amount of CPU that database needs for standard operation | _1_ |
|**DATABASE_MEMORY_LIMIT**| It make sure a database container never goes above a certain value of memory. The container is only allowed to go up to the limit, and then it is restricted | _2Gi_ |
|**DATABASE_MEMORY_REQUEST**| The amount of RAM memory that database needs for standard operation (normally in Gibibytes) | _1Gi_ |
|**DATABASE_STORAGE_CLASSNAME**| Provides a way for administrators to describe the "class" of storage used by Database Persistent Volumen Claim (PVC). Different classes might map to quality-of-service levels, or to backup policies, or to arbitrary policies determined by the cluster administrators | _gp2 (AWS General Purpose Storage)_ |
|**DATABASE_STORAGE_SIZE**| The size of database storage for onix database | _50_ |
|**DBMAN_SNAPSHOT_TAG**| Tags identify different versions of the same series of dbman images | _v0.0.4-d4fb6f7-031020001129_ |
|**MONGODB_CPU_LIMIT**| It make sure a mongo db container never goes above a certain value of cpu. The container is only allowed to go up to the limit, and then it is restricted | _3_ |
|**MONGODB_CPU_REQUEST**|  The amount of CPU that mongo db needs for standard operation | _1_ |
|**MONGODB_MEMORY_LIMIT**| It make sure a mongo db container never goes above a certain value of memory. The container is only allowed to go up to the limit, and then it is restricted | _5Gi_ |
|**MONGODB_MEMORY_REQUEST**| The amount of RAM memory that mongo db needs for standard operation (normally in Gibibytes) | _3Gi_ |
|**NEXUS_TAG**| Tags identify different versions of the same series of nexus images. | _v0.0.4-d4fb6f7-031020001129_ |
|**NEXUS_CPU_LIMIT**| It make sure a nexus container never goes above a certain value of cpu. The container is only allowed to go up to the limit, and then it is restricted | _2_ |
|**NEXUS_CPU_REQUEST**| The amount of CPU that Nexus needs for standard operation | _1_ |
|**NEXUS_MEMORY_LIMIT**| It make sure a nexus container never goes above a certain value of memory. The container is only allowed to go up to the limit, and then it is restricted | _2Gi_ |
|**NEXUS_MEMORY_REQUEST**|  The amount of RAM memory that Nexus needs for standard operation (normally in Gibibytes) | _1Gi_ |
|**NEXUS_STORAGE**| The amount of storage that will be allocated by the platform to the Nexus persistent volume claim (PVC) | _5Gi (5 Gibibytes) or 800Mi (800 Mebibytes)_ |
|**NEXUS_STORAGE_CLASSNAME**| Provides a way for administrators to describe the "class" of storage used by Nexus Persistent Volumen Claim (PVC).Different classes might map to quality-of-service levels, or to backup policies, or to arbitrary policies determined by the cluster administrators | _gp2 (AWS General Purpose Storage)_ |
|**MONGO_TAG**| Tags identify different versions of the same series of mongo images. | _v0.0.4-d4fb6f7-031020001129_ |
|**NEXUS_OPERATOR_FLAG**| Using this flag we can switch between nexus and nexusoperator | _false_ |
|**ONIX_CPU_LIMIT**| It make sure a Onix container never goes above a certain value of cpu. The container is only allowed to go up to the limit, and then it is restricted. | _2_ |
|**ONIX_CPU_REQUEST**| The amount of CPU that Onix needs for standard operation | _1_ |
|**ONIX_MEMORY_LIMIT**| It make sure a Onix container never goes above a certain value of memory. The container is only allowed to go up to the limit, and then it is restricted | _2Gi_ |
|**ONIX_MEMORY_REQUEST**| The amount of RAM memory that Onix needs for standard operation (normally in Gibibytes) | _1Gi_ |
|**ONIX_SNAPSHOT_TAG**| Tags identify different versions of the same series of onix images | _v0.0.4-d4fb6f7-031020001129_ |
|**ONIXDB_COMMIT_HASH**| It's unique identifier generated by Git with latest changes | _2067daeeabb5e1ceee1fb838a1b46844bd48923c_ |
|**PILOTCTL_CPU_LIMIT**| It make sure a pilotctl container never goes above a certain value of cpu. The container is only allowed to go up to the limit, and then it is restricted. | _2_ |
|**PILOTCTL_CPU_REQUEST**| The amount of CPU that pilotctl needs for standard operation | _1_ |
|**PILOTCTL_MEMORY_LIMIT**| It make sure a pilotctl container never goes above a certain value of memory. The container is only allowed to go up to the limit, and then it is restricted | _2Gi_ |
|**PILOTCTL_MEMORY_REQUEST**| The amount of RAM memory that pilotctl needs for standard operation (normally in Gibibytes) | _1Gi_ |
|**PILOTCTL_TAG**| Tags identify different versions of the same series of pilotctl images | _v0.0.4-d4fb6f7-031020001129_ |
|**PILOTCTLDB_COMMIT_HASH**| It's unique identifier generated by Git with latest changes | _3087daeeabb5e1ceee1fb838a1b46844bd48923c_ |
|**PILOTCTL_MONGO_EVR_CPU_LIMIT**| It make sure a mongo event receiver container never goes above a certain value of cpu. The container is only allowed to go up to the limit, and then it is restricted. | _2_ |
|**PILOTCTL_MONGO_EVR_CPU_REQUEST**| The amount of CPU that mongo event receiver needs for standard operation | _1_ |
|**PILOTCTL_MONGO_EVR_MEMORY_LIMIT**| It make sure a mongo event receiver container never goes above a certain value of memory. The container is only allowed to go up to the limit, and then it is restricted | _2Gi_ |
|**PILOTCTL_MONGO_EVR_MEMORY_REQUEST**| The amount of RAM memory that mongo event receiver needs for standard operation (normally in Gibibytes) | _1Gi_ |
|**PILOTCTL_EVR_MONGODB_TAG**| Tags identify different versions of the same series of mongo event receiver images | _v0.0.4-d4fb6f7-031020001129_ |
|**SERVICE_TYPE**| A service is responsible for exposing an interface to pods, which enables network access from either within the cluster or between external processes and the service | _ClusterIP,NodePort,LoadBalancer_ |
|**PGADMIN_TAG**| Tags identify different versions of the same series of pgadmin images | _latest_ |
|**POSTGRES_TAG**| Tags identify different versions of the same series of postgres images | _latest_ |
|**TESTDATA_FLAG**| If this flag is enabled apply test for all the apps | _false_ |
|**DB_DEFAULT_ADMIN_PWD**| The password for default admin user of the database | _admin_ |
|**DB_DEFAULT_ADMIN_USER**| The default admin user comes with the postgres database | _admin_ |
|**DBMAN_HTTP_PWD**| The password for dbman web api | _admin_ |
|**DBMAN_HTTP_USER**| The username for dbman web api (@ localhost:8085/api/) | _admin_ |
|**MONGO_EVR_HTTP_PWD**| The password required to access mongo event receiver http API | _admin_ |
|**MONGO_EVR_HTTP_USER**| The username required to access mongo event receiver http API | _admin_ |
|**MONGODB_PASSWORD**| The password required to access mongodb | _admin_ |
|**MONGODB_USERNAME**| The username required to access mongodb | _admin_ |
|**ONIX_DB_PWD**| The password for the onix database | _onix_ |
|**ONIX_DB_USER**| The user for the onix database | _onix_ |
|**ONIX_HTTP_READER_PWD**| The Onix WAPI http user password (@ localhost:8080/swagger-ui.html) | _admin_ |
|**ONIX_HTTP_READER_USER**| The Onix WAPI http user (@ localhost:8080/swagger-ui.html) | _admin_ |
|**ONIX_HTTP_WRITER_PWD**| A service is responsible for exposing an interface to pods, which enables network access from either within the cluster or between external processes and the service | _ClusterIP,NodePort,LoadBalancer_ |
|**ONIX_HTTP_WRITER_USER**| The Onix WAPI http user password (@ localhost:8080/swagger-ui.html) | _admin_ |
|**ONIX_WAPI_ADMIN_PWD**| The Onix WAPI http password (@ localhost:8080/swagger-ui.html) | _admin_ |
|**ONIX_WAPI_ADMIN_USER**| The Onix WAPI http user (@ localhost:8080/swagger-ui.html) | _admin_ |
|**OX_HTTP_PWD**| The password required to access runner application | _admin_ |
|**OX_HTTP_UNAME**| The username required to access runner application | _admin_ |
|**OX_WAPI_PWD**| The Onix WAPI http password (@ localhost:8080/swagger-ui.html) | _admin_ |
|**OX_WAPI_UNAME**| The Onix WAPI http user (@ localhost:8080/swagger-ui.html) | _admin_ |
|**OXA_HTTP_PWD**| The password required to access registry application | _admin_ |
|**OXA_HTTP_UNAME**| The username required to access registry application | _admin_ |
|**PILOTCTL_DB_PWD**| The password for the PILOTCTL database | _admin_ |
|**PILOTCTL_DB_USER**| The user for the PILOTCTL database | _admin_ |
|**PILOTCTL_HTTP_PWD**| The pilotctl WAPI password | _admin_ |
|**PILOTCTL_SIGNING_KEY**| the tls key required for signing pilotctl | _LS0y3556 |
|**TLS_KEY**| The base64 value of key to be applied to all the applications | _LS0y3443= |
|**TLS_CRT**| The base64 value of crt to be applied to all the applications | _LS3435=_ |
|**APS_ONIX_OXART_REG_USER**| The username to authenticate with the registry at artisan-registry-amosonline-aws-01-aps-test.apps.amosds.amosonline.io | _admin_ |
|**APS_ONIX_OXART_REG_PWD**| The password to authenticate with the registry at 'artisan-registry-amosonline-aws-01-aps-test.apps.amosds.amosonline.io' | _admin_ |
|**APS_ONIX_OXART_VERIFICATION_KEY**| the path of the key in the artisan registry,public PGP key required to open the package artisan-registry-amosonline-aws-01-aps-test.apps.amosds.amosonline.io | _/_ |

# How to build the packages

Use the below commands to create artisan packages. Please refer build.yaml file for available profiles.

```bash
# build package using art cli
art build -t <PACKAGE_NAME> -p <ART_PROFILE>

# push package into the repository
art push -u=<ART_REG_USER>:<ART_REG_PWD> <PACKAGE_NAME>
```

# How to run the packages

If the package is already available in the repository then use the below commands to use them

```bash
# Pull package from repository
art pull -u=<ART_REG_USER>:<ART_REG_PWD> <PACKAGE_NAME>

# Generate configuration file & populate configuration
art env package <PACKAGE_NAME>

# Update corresponding environment variable values
vi .env

# Execute package
art exec -u=<ART_REG_USER>:<ART_REG_PWD> <PACKAGE_NAME> setup

```

