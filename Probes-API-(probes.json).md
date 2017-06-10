* URL: `/probes.json`
* Method: `GET`
* Input (Parameters):
  * none
* Output (Response):
  * Format: `json`
  * Syntax: (Object)
    * "{Probe ID (32 char 0-9a-f string)}": (Object)
      * "country": (String) "{Country Name}"
      * "city": (String) "{City Name}"
      * "unlocode": (String) "{UNECE UN/LOCODE}"
      * "provider": (String) "{ISP}"
      * "asnumber": (Number) {BGP AS Number}
      * "group": (String) "{Group name displayed on the probe selection - e.g. continent}"
      * "caps": (Object)
        * "{Capability name - e.g. ping}": (Boolean|Number) {false=no IPv4/6 support, true=IPv4/6 support, 4=IPv4 only, 6=IPv6 only}
      * "status": (Boolean) {true=online, false=offline}