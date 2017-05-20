```
{
	"probe_id_hash": "{Random string to use as hashing initialization vector - e.g. 7QnL4dld5nzmHpsk}",
	"ssh_defaults": [{Array of arguments in strings to use when connecting via SSH to remote hosts}
		"-q",
		"-F/dev/null",
		"-oPasswordAuthentication=no",
		"-oKbdInteractiveAuthentication=no",
		"-oChallengeResponseAuthentication=no",
		"-oUseRoaming=no",
		"-oStrictHostKeyChecking=no",
		"-oConnectTimeout=60",
		"-oServerAliveCountMax=120",
		"-oServerAliveInterval=1",
		"-oControlPath=/tmp/%r@%h:%p",
		"-oControlMaster=auto",
		"-oControlPersist=3600"
	],
	"queue": {
		"probe": {number of tests one probe can run simultaneously before starting to queue up query requests},
		"websocket": {number of tests one websocket client can run simultaneously before starting to queue up query requests},
		"global": {number of tests the entire system can run simultaneously before starting to queue up query requests}
	},
	"logs": {
		"status": {boolean - true if query requests should be printed on stdout, false if not},
		"requests": {
			"http": {boolean - true if http query requests should be printed on stdout, false if not},
			"websocket": {boolean - true if websocket query requests should be printed on stdout, false if not}
		},
		"use_x_forwarded_for": {boolean - true if the X-Forwarded-For header should be used to print logs instead of using the remote address, false if not},
		"debug": {boolean - true if we should print all kinds of debug messages, false if not}
	},
	"http": {
		"port": {number of HTTP port to listen on, ports below 1024 require this script to be executed as root}
	}
}
```