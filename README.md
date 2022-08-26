# cache.do
Cache any HTTP Request on the Edge

```
https://cache.do/:ttl/:url
```

<https://cache.do/86400/uuid.do>

You can also specify the TTL in shorthand format like `5m`, `2h`, `7d`, or `2w`

<https://cache.do/1w/uuid.do>

By default, the cache is stored in a single edge location and is not globally replicated.  If global replication is desired, there are two additional variations:

- KV <https://kv.cache.do/1w/uuid.do>
- R2 <https://r2.cache.do/1w/uuid.do>

Additional variations:

- [swr.do](https://swr.do): Stale While Refresh Caching
