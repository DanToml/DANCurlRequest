DANCurlRequest [![Build Status](https://travis-ci.org/endocrimes/DANCurlRequest.svg?branch=master)](https://travis-ci.org/endocrimes/DANCurlRequest)
==============

Quickly output NSURLRequests as cURL strings.

Usage:
```objc
NSMutableURLRequest *request = [[NSMutableURLRequest alloc] initWithURL:[NSURL URLWithString:@"https://api.github.com/zen"]];
[request addValue:@"application/json" forHTTPHeaderField:@"Accept"];
[request setHTTPMethod:@"GET"];

NSString *curl = [request dan_curlRequest];
```
