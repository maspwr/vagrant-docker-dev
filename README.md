# Description

This README should appear in the Docker container. Any updates to it
should also appear in the container.

# Testing

Make sure you have Vagrant and Ansible installed. Then:

```
vagrant up --provider=docker
```

Then make a change to this README.md file and then:

```
vagrant rsync
```

