## how to install

[binary from command line](https://docs.nats.io/running-a-nats-service/introduction/installation#getting-the-binary-from-the-command-line)

```sh
curl -sf https://binaries.nats.dev/nats-io/nats-server/v2@v2.10.20 | sh
```

## and run
```sh
~$ ./nats-server
[726963] 2024/11/20 06:34:27.901263 [INF] Starting nats-server
[726963] 2024/11/20 06:34:27.901380 [INF]   Version:  2.10.20
[726963] 2024/11/20 06:34:27.901384 [INF]   Git:      [7140387]
[726963] 2024/11/20 06:34:27.901389 [INF]   Name:     NCSEQ7AH4OZKQN37XIQT4B7RY7KOE5XWGDVVRHIM7TMHC4N2XD3XUEGP
[726963] 2024/11/20 06:34:27.901392 [INF]   ID:       NCSEQ7AH4OZKQN37XIQT4B7RY7KOE5XWGDVVRHIM7TMHC4N2XD3XUEGP
[726963] 2024/11/20 06:34:27.902161 [INF] Listening for client connections on 0.0.0.0:4222
[726963] 2024/11/20 06:34:27.902937 [INF] Server is ready
```

### system.d
https://github.com/nats-io/nats-server/blob/main/util/nats-server.service


## develop

- [faststream as connector](https://faststream.airt.ai/latest/nats/)

https://docs.nats.io/using-nats/developer/develop_jetstream

- kv: [nats.io](https://docs.nats.io/using-nats/developer/develop_jetstream/kv#creating-and-deleting-kv-buckets)
