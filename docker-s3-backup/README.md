# docker-s3-backup

Dockerfile for setting up [Docker](https://github.com/dotcloud/docker) container with [Jetty](http://www.eclipse.org/jetty/) installed.

## Pulling

    $ docker pull maluuba/s3backup

## Running

    $ chmod +x run-backup.sh
    # SOURCE_DIR = <directory in to backup>
    # S3PATH = the path in s3 starting with bucker name bucket-name/folder/something
    # LIMIT = The number of old backups to keep, includign this one
    $ run-backup.sh AWS_ACCESS_KEY AWS_SECRET_KEY SOURCE_DIR S3PATH LIMIT"

## Building

From sources:

    $ docker build github.com/maluuba/docker-s3-backup
    
## Author

  * Usman Ismail (<usman.ismail@maluuba.com>)

## LICENSE

Copyright 2014 Maluuba

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.    