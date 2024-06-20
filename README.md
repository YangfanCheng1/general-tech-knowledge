# general-tech-knowledge

CNF -> CSR + key -> CRT (End certificate body) + Chain (Intermediate + Root)

Command:
```
openssl req -new -out {domain.csr} -newKey rsa:2048 -nodes -sha256 -keyout {domain.key} -config {domain.cnf}
```
