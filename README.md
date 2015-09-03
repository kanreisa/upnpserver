# Chinachu UPnP Server
![chinachu icon](icon/icon_128.png)

UPnP Server for Chinachu Air.

forked from [oeuillot/upnpserver](https://github.com/oeuillot/upnpserver).

##Configuration
Server constructor accepts an optional configuration object. At the moment, the following is supported:

- `log` _Boolean_ Enable/disable logging. Default: false.
- `logLevel` _String_ Specifies log level to print. Possible values: `TRACE`, `DEBUG`, `INFO`, `WARN`, `ERROR`, `FATAL`. Defaults to `ERROR`.
- `name` _String_ Name of server. Default 'Node Server'
- `uuid` _String_ UUID of server. (If not specified, a UUID v4 will be generated)
- `hostname` _String_ Hostname to bind the server. Default: 0.0.0.0
- `httpPort` _Number_ Http port. Default: 10293
- `dlnaSupport` _Boolean_ Enable/disable dlna support. Default: true
- `strict` _Boolean_ Use only official UPnP attributes. Default: false
- `lang` _String_ Specify the language (en, fr) for virtual folder names. Default: en
- `ssdpLog` _Boolean_ Enable log of ssdp layer. Default: false
- `ssdpLogLevel` _String_ Log level of ssdp layer.

## Testing
For testing purposes used *mocha* framework. To run tests, you should do this:
```bash
make test
```
