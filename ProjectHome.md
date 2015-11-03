pynexpose provides Python bindings for interacting with a NeXpose server through v1.1 of its API. It is heavily inspired by the [pynessus](http://code.google.com/p/pynessus) module.

This module is currently in an early alpha stage and as does little more than provide functions for all the v1.1 API calls and returns their respective XML responses.

Basic usage example: listing reports on a NeXpose server.

```
import pynexpose

serveraddr = 'server'
port = 443
username = 'nexpose'
password = 'password'

n = pynexpose.NeXposeServer(serveraddr, port, username, password)
response = n.report_listing()

print response
```

This module is maintained by Patrik Nordlén (patriki at gmail dot com). Suggestions and bug reports are appreciated.