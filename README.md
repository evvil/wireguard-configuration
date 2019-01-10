
## Server side

```sh
socat EXEC:./server.sh,pty,rawer TCP-LISTEN:12345,bind=192.168.128.1,fork,reuseaddr
```

## Client side

```sh
export ENDPOINT=<...>
export REMOTE_HOSTNAME=192.168.128.1
export REMOTE_PORT=12345
./client.sh
```
