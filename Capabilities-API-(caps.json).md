* URL: `/caps.json`
* Method: `GET`
* Input (Parameters):
  * none
* Output (Response):
  * Format: `json`
  * Syntax: (Object)
    * "{Capability ID - e.g. ping}": (Object)
      * "name": (String) "{Human readable capability name - e.g. Ping}"
      * "highlight": (String|Number) "{Regex used to highlight a line on the web UI}" or {Line number counting from the last line}
      * "cmd4": (String) "{Command to execute if the target IP is an IPv4 address - {{TARGET}} is the IP address}"
      * "cmd6": (String) "{Command to execute if the target IP is an IPv6 address - {{TARGET}} is the IP address}"