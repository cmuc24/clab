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
title: apt..
# Custom Titel für die Navigation
label: Setup
icon: terminal
tags:
  - guide
  - config options
  - installation
# route: /custom/path
# redirect: getting-started.md
# order: 100

---



apt install ca-certificates apt-transport-https lsb-release gnupg curl nano unzip -y

apt install software-properties-common -y




## php, python

apt install software-properties-common

add-apt-repository ppa:ondrej/php
add-apt-repository ppa:deadsnakes/ppa



apt install php8.2 php8.2-cli php8.2-common php8.2-curl php8.2-gd php8.2-intl php8.2-mbstring php8.2-mysql php8.2-opcache php8.2-readline php8.2-xml php8.2-xsl php8.2-zip php8.2-bz2 libapache2-mod-php8.2 -y

apt install php8.0 php8.0-cli php8.0-common php8.0-curl php8.0-gd php8.0-intl php8.0-mbstring php8.0-mysql php8.0-opcache php8.0-readline php8.0-xml php8.0-xsl php8.0-zip php8.0-bz2 libapache2-mod-php8.0 -y