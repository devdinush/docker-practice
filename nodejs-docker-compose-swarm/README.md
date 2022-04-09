## NodeJs Multistage Docker

### Build it for development

```
docker build --target development -t nodejs-multistage:development .
```

### Build it for test

```
docker build --target test -t nodejs-multistage:test .
```

### Build it for production
```
docker build --target production -t nodejs-multistage:production .
```
