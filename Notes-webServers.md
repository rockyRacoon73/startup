# The internet
# Web Servers
a computing device that is hosting a web service that knows how to accept incoming internet connections and speak the HTTP application protocol
# web service gateways
* multiple web services on single device
* each service starts on a different port in device
* gateway looks at request and maps it to port number

# Amazon WEb Services - EC2

**opening startup server in browser**
`http://18.232.89.80`

## ssh into server
`➜  ssh -i [key pair file] ubuntu@[ip address]`

restrict permissions
 `chmod  600 [key pair file]`

 # Domain Names
get IP address for any domain - `dig`
domane names may have multiple IP addresses (such as amazon.com)  in cas server listening at IP adress is not responding

domain names 
* a root and 1+ subdomains
 *`[subdomain.]*secondary.top`
 *root domain is represented by secondary level and top level domains
 *TLD representes things like com, edu, or clock
* ex: root domains byu.edu, google.com, cs260.click
* ICAAN controls list of TLDs
* root domain owner can create any number of subdomains

`whois` console utility gets info about domain name from domane name registery

DNS database records for mapping domain names to IP adresses
* `address (A)`
*   straight mapping from a domain  name to IP address
* `canonical name (CNAME)`
*   maps one domain name to another domain name
*   acts like an alias so you can map things like byu.com to byu.edu IP

there are a lot of levels to caching
( browser checks its cache of names for domain, if not contacts DNS and gets IP, if not in DNS, DNS contacts `authoritative name server` as last resort - unkown domain name error
caching can be frustrating when updating domain name
so you can set `time to live` (`TIL`) min to days and caching layers should honor TIL and clear cache

