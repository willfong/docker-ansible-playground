# Docker Ansible Playground

Stupid project to use Docker containers instead of VMs to learn about Ansible.

## Getting Started

Build the images:

```
docker compose build
```

Start the containers:

```
docker compose up -d
```

Shell into the container:

```
docker exec -it controller bash
```

Test connectivity:

```
ansible all -m ping
```

Wipe out containers (to start over):

```
docker compose down
```
