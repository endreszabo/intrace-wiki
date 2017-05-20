```
{
	"{Capability ID - e.g. ping}": {
		"name": "{Human readable capability name - e.g. Ping}",
		"highlight": "{Regex used to highlight a line on the web UI}" or {Line number counting from the last line},
		"cmd4": "{Command to execute if the target IP is an IPv4 address - {{TARGET}} is the IP address - e.g. ping -c 4 {{TARGET}} 2>&1}",
		"cmd6": "{Command to execute if the target IP is an IPv6 address - {{TARGET}} is the IP address - e.g. ping -c 4 {{TARGET}} 2>&1}"
	},
	...
}
```