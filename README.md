## Usage

Use `docker-compose` to bring up the container.

```
# docker-compose up
```

And your local forwarder should be ready on `*:53`. Try `dig whoami.akamai.net @127.0.0.1` to see if it works.

## Configuration

This repository configures Cloudflare's 1.1.1.1 via DoT by default. Modify `Corefile` to use other providers.

See https://coredns.io/plugins/forward/ for how to configure it.
