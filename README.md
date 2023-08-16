# Ansible Role: EMQX

![GitHub](https://img.shields.io/github/license/xylodev/ansible-role-emqx)

Installs EMQX MQTT broker in Docker container on Debian/Ubuntu machines

## Role variables

    emqx_version: latest
    
EMQX version to install. See https://hub.docker.com/r/emqx/emqx/tags for available Docker image versions.

    emqx_container_name: emqx

Name for the EMQX container.

    emqx_app_dir: /opt/emqx

A directory on the Docker host to store volumes for EMQX container

## Example Playbook

    - hosts: all
      roles:
        - role: xylodev.emqx
          vars:
            emqx_version: "5.1"
