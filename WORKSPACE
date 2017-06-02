# Copyright 2017 The Bazel Authors. All rights reserved.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#    http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
workspace(name = "io_bazel_rules_docker")

load("//docker:docker.bzl", "docker_repositories", "docker_pull")

# Consumers shouldn't need to do this themselves once WORKSPACE is
# instantiated recursively.
docker_repositories()

docker_pull(
    name = "official_busybox",
    registry = "index.docker.io",
    repository = "library/busybox",
    tag = "1.26",
)

docker_pull(
    name = "official_python",
    registry = "index.docker.io",
    repository = "library/python",
    tag = "2.7",
)
