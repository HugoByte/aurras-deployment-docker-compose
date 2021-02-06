<!--
#
# Licensed to the Apache Software Foundation (ASF) under one or more
# contributor license agreements.  See the NOTICE file distributed with
# this work for additional information regarding copyright ownership.
# The ASF licenses this file to You under the Apache License, Version 2.0
# (the "License"); you may not use this file except in compliance with
# the License.  You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
-->
# Aurras Docker Compose Deployment Configuration
[![License](https://img.shields.io/badge/license-Apache--2.0-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)

> docker-compose deployment is used for local development and testing and should not be used for production.  

### Prerequisites

1. [Docker](https://docs.docker.com/engine/install/)
2. [Docker Compose](https://docs.docker.com/compose/)

### Deployment Guide

Clone [aurras-deployment-docker-compose](https://github.com/HugoByte/aurras-deployment-docker-compose)

```text
git clone https://github.com/HugoByte/aurras-deployment-docker-compose
```

#### Openwhisk

1. Navigate to openwhisk setup directory

```text
cd aurras-deployment-docker-compose/openwhisk
```

2. Run docker-compose command to start the services

```text
docker-compose --project-name openwhisk up -d
```

#### Event Feed - Substrate

1. Navigate to aurras-event-feed-substrate setup directory

```text
cd aurras-deployment-docker-compose/aurras-event-feed-substrate
```

2. Make configuration changes if needed to local.env  

3. Run docker-compose command to start the services

```text
docker-compose --project-name aurras up -d
```

### License
Licensed under [Apache-2.0](./LICENSE)