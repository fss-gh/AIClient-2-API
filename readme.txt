podman build -t docker_aiclient-api:latest --format docker -f Dockerfile .

podman-compose -f 'docker-compose.build.yml' up -d --remove-orphans

podman-compose -f 'docker-compose.yml' up -d