Run 2 command to create 2 container
```
docker run -dit --env BG_COLOR="blue" -p 5050:3000 gcr.io/tetratelabs/color-app:1.0.0
docker run -dit --env BG_COLOR="green" -p 5000:3000 gcr.io/tetratelabs/color-app:1.0.0
```

Install envoy server
```
curl -L https://func-e.io/install.sh | bash -s -- -b .
```

Run server
```
./func-e run -c envoy.yaml
```