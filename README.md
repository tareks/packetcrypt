# packetcrypt
Build a Docker Image for latest PKT mining

In many cases, the develop branch may have the latest code with improvements for mining (multipool, performance boosts, etc).

## Build

Clone this repo into a new empty directory, then:
```
docker build --progress=plain -f Dockerfile.distroless  -t packetcrypt:develop .
```

## Run

```
docker run --rm packetcrypt:develop ann -p <PKT wallet address> <pool #1> <pool #2> <pool #3>
```
