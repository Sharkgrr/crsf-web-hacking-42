# The Importance of Authentication

## Two-Factor Authentication

Two-factor authentication is currently the best way to protect against external requests. It requires the attacker to not only have the username and password but also access to the security code. In this case, it would not be possible to carry out the attack.

## Bearer token

It is important to clarify that with this type of token, renewal is required every 5 minutes. This means that if the attacker has the client ID and client secret, they will have 5 minutes to execute the attack before access is denied. Another important point is that this token is traceable via APIs and will only be permitted if the API accepts that type of client.

## References

https://www.techtudo.com.br/noticias/2021/08/autenticacao-de-dois-fatores-o-que-e-e-para-que-serve-o-recurso.ghtml

https://jwt.io/introduction