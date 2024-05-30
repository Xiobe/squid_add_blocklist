# squid_add_blocklist
List of regular expressions to block adds using a squid proxy. Copy the blocklist over to ad_block.txt.

## Config squid.conf
```text
# advertisement blocking
acl ads dstdom_regex "/etc/squid/ad_block.txt"
http_access deny ads
```
