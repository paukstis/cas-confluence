A quick make recipe to build and install CAS integration with Atlassian Confluence

## Requirements
- Installed [Atlassian Confluence](https://www.atlassian.com/software/confluence)
- Installed [Apereo CAS](https://github.com/apereo/cas)
- Linux and GNU make (to run this recipe)
- Git, JDK and Apache Maven (to build CAS Java client)
- openssl (optional, to install LDAPS trust certificate in Confluence java keystore)

## Getting started
Checkout `cas` branch
```shell
git checkout cas
```

Copy `makefile.inc.sample` to `makefile.inc` and edit it to match your site
configuration. Run
```shell
make build
```
This will build all files required for CAS integration in `target` folder.


```shell
sudo make install
```
