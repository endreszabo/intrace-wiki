```
[array of objects, each object represents a single probe/node
	{
		"country": "{country - e.g. United States}",
		"city": "{city - e.g. Los Angeles}",
		"unlocode": "{UN/LOCODE - e.g. uslax - see http://www.unece.org/cefact/locode/service/location for valid UN/LOCODE values}",
		"provider": "{provider name - e.g. Hurricane Electric}",
		"asnumber": {as number - e.g. 6939},
		"host": "{ssh username and hostname - e.g. root@uslax.yourserver.tld}",
		"group": "{group name - e.g. North america}",
		"residential": {boolean, true if this probe is a residential connection (end user, DSL connection, etc.), false if not},
		"caps": {
			"{Capability ID - e.g. ping}": {boolean or number, true=probe supports dual stack for this capability, 4=probe supports IPv4 only, 6=probe supports IPv6 only, false=probe does not support this capability},
			...
		}
	},
	...
]
```