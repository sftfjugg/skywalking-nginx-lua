# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

FROM eclipse-temurin:8-jre-alpine

RUN apk add --no-cache curl
RUN wget https://github.com/mikefarah/yq/releases/download/v4.24.5/yq_linux_amd64 -O /usr/bin/yq \
    && chmod +x /usr/bin/yq

COPY execute_and_validate.sh /execute_and_validate.sh

CMD ["sh", "/execute_and_validate.sh"]
