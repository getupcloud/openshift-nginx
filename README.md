# OpenShift Nginx Cartridge
This cartridge serves static content using nginx web server.

Place your files inside www/ dir, commit and push.

## Usage

```bash
$ rhc app create nginx https://reflector-getupcloud.getup.io/reflect?github=getupcloud/openshift-nginx
$ cd nginx
$ echo 'Hello World' >> www/hello.html
$ git add .
$ git commit -m 'Testing'
$ git push
```

## User-defined configuration

Place your .conf files inside config/nginx.d/. It will be include()ed from "server" scope.
