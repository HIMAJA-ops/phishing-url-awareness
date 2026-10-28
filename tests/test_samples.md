# Test Results
Python version used: 3.14.6 | Operating system: Windows | Date: 28/10/26
| # | Input | Expected result | Actual result | Pass/Fail |
|---|-------|-----------------|---------------|-----------|
| 1 | https://www.example.com/login | No listed warning signs |No listed warniing signs found. | Pass|
| 2 | http://192.0.2.10/account | IP address + HTTP | IP address + HTTP|Pass |
| 3 | http://example.com@sample.invalid/login | @ symbol + HTTP |Contains an @ symbol; Uses HTTP. |Pass |
| 4 | https://a.b.c.d.e.example.invalid/path | Many hostname segments |Contains many hostname segments/domains. |Pass |
| 5 | https://xn--example.invalid/ | Punycode-style hostname |Contains a punycode-style hostname. |Pass |
## Notes
I learned that a URL Checker program doesn't actually visit websites or scan for malware but instead analyzes the text for warming indicators.I was surprised to realize that a url can return "No listing warnings found" and still be completely dangerous, meaning lack of clues does not guarantee online safety.