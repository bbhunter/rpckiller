
# rpckiller
This script checks for any possible SSRF dns/http interactions in xmlrpc.php pingback feature and with that you can  further try to escalate it to -

1. Internal Port scans 
2. DOS [HTTP Reflection attack]
3. brute force attacks


## Installation


```bash
pip3 install urllib3 requests
```

## Usage

```python
python3 rpckiller.py http(s)://target/xmlrpc.php collab.net/localhost:port '/endpoint/'
```

## Note

This script does Out of Band detection using the burp collaborator or you can use any other service , also you can check for port scans by adding a list of ports and automate it and look at the response on the screen. If the int value is greater than 0 then port is Open as we assume .

"This script does the basic check so make sure to have a good list of endpoints gathered from the target you testing in order to get proper interaction"

## Developer
[@D0rkerDevil] (https://twitter.com/D0rkerDevil)

## License
[MIT](https://choosealicense.com/licenses/mit/)
