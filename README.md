# Docker Ansible Playground

Stupid project to use Docker containers instead of VMs to learn about Ansible.

Why?

- Didn't want to set up virtual machines
- Docker uses a lot less memory
- Volume mapping (for playbooks) so I can use an editor instead of copying files into a VM

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
ansible-playbook ping-test.yml
```

Wipe out containers (to start over):

```
docker compose down
```
