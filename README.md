# general-tech-knowledge

CNF -> CSR + key -> CRT (End certificate body) + Chain (Intermediate + Root)

Command:
```
openssl req -new -out {domain.csr} -newKey rsa:2048 -nodes -sha256 -keyout {domain.key} -config {domain.cnf}
```

AWS IAM

```
Account A & Account B
B creates a role arn:aws:iam::B:role/Some-Role with a permission for A, 
A creates a policy 
{
      "Version": "2012-10-17",
      "Statement": {
             "Effect": "Allow",
             "Action": "sts:AssumeRole",
             "Resource": "arn:aws:iam::B:role/Some-Role"
         }
}
```
