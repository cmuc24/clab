
### yt-dlp

```bash
# Same command to install & update via python pip
python -m pip install -U yt-dlp
```

### node, npm & yarn via nvm

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
nvm ls available
nvm install 18
npm install --global yarn
```

Version aktuell?
* Linux: https://github.com/nvm-sh/nvm#installing-and-updating
* Windows: https://github.com/coreybutler/nvm-windows#nvm-for-windows

### node, npm & yarn via nodesource & apt

* https://github.com/nodesource/distributions/blob/master/README.md#table-of-contents

### yarn 
* https://classic.yarnpkg.com/lang/en/docs/install/#windows-stable
* https://yarnpkg.com/getting-started/install

### pnpm
* https://pnpm.io/installation


### another npm version manager: n
* https://www.npmjs.com/package/n#installation


### windows apps
* TextCrawler (digitalvolcano.co.uk)](https://www.digitalvolcano.co.uk/tcdownloads.html)
* Duplicate Cleaner (digitalvolcano.co.uk)](https://www.digitalvolcano.co.uk/dcdownload_versions.html)

## apache2, mysql, postgresql, php, phpmyadmin, composer

https://webmin.com/download/

```bash copy
curl -o setup-repos.sh https://raw.githubusercontent.com/webmin/webmin/master/setup-repos.sh
sh setup-repos.sh
```

# urls

- https://github.com/mikeroyal/Self-Hosting-Guide/blob/main/README.md
- https://github.com/hlissner/dotfiles (NixOS)
- https://marketplace.visualstudio.com/items?itemName=vscode-nested-tags.vscode-nested-tags


# regex

Datum
```js copy
(?<!\d)(\d|0\d|1\d|2\d|3\d)[\.,]\s{0,3}(\d|0\d|1[012]|Januar|Februar|März|April|Mai|Juni|Juli|August|September|Oktober|November|Dezember)[\.,]?\s{0,3}(19\d{2}|20\d{2}|\d{2}(?!\d))
```
