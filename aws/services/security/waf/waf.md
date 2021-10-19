# Web Application Firewall (WAF)

Protects your web application from common web exploits. 

Specifically operates at Layer 7 of the network packet, the application layer, i.e. HTTP.

Layer 4 = TCP.

WAF can be deployed on
- ALB
- API Gateway
- Cloud Front

Define Web Access Control List (ACL) i.e. rules on the HTTP packet. Protects from:
- SQL injection
- XSS (cross site Scripting)
- size constraints
- geo-match (block countries)
- DDoS (rate based rules)

## AWS Firewall Manager

Manage all firewalls accross all your AWS accounts.

Centralised way to manage all your firewall rules.