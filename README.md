# Trellis • Redis

The Redis images used by Trellis, replication built in.


## Usage

```
docker run -d --name primary -p 6379:6379 trelllis/redis:primary

docker run -d --name replica-1 -p 6380:6379 --link primary:primary trelllis/redis:replica
```

## Persistence
Primary instances are the only instances that save data using RDB bakground saves,
to **/data** so you might want to mount a directory for backup or re-generating data on failures.

## License
MIT

