---
# The layout for the page. Default is default.
layout: default
# Supported values: default, central, page, and blog.

date: 2023-05-05 

author:
  name: cmuc doc
lang: en
categories:
  - Admin Guides
templating: true
# Titel der Seite 
title: docker
# Custom Titel für die Navigation
label: docker-setup
icon: terminal
tags:
  - guide
  - config options
  - installation
# route: /custom/path
# redirect: getting-started.md
# order: 100

---

!!!primary
  A **callout** is a short piece of text intended to attract attention.
!!!

!!!secondary
  Today is Friday.
!!!

# Summary
```bash copy
apt install curl -y
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
rm get-docker.sh
sudo curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
sudo usermod -aG docker $(whoami)
su - $(whoami)
groups $(whoami)
```

A **callout** is a short piece of text intended to attract attention. A **callout** is a short piece of text intended to attract attention. A **callout** is a short piece of text intended to attract attention. A **callout** is a short piece of text intended to attract attention.


# docker 

°fa-info° (information text) 
- https://github.com/docker/docker-install#usage
- https://docs.docker.com/compose/install/other/#on-linux

### docker

```bash
apt install curl -y
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```

### docker-compose

```bash
sudo curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```

### docker post-config

```bash
sudo systemctl status docker       

# docker group
sudo usermod -aG docker $(whoami)
su - $(whoami)
groups $(whoami)

# optional login 
docker login
```