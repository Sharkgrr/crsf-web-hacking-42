## Explaining CSRF

CSRF (Cross-Site Request Forgery) is a web application attack in which the attacker impersonates a legitimate user and attempts to perform actions or induce practices without consent or authorization.

In this case of the attack, an external request was successfully made without authentication.

# Scenario 1 

## How to execute

1. Run the server ./start.sh
2. Open the prompt terminal
3. Execute the code:

```
curl -X POST http://localhost:8080/transfer \
-H "Content-Type: application/x-www-form-urlencoded" \
-d "amount=1000"
```

4. Reload the main project 'index.html'
5. Click submit

Output: Current Balance: 0$

# Scenario 2

## How to execute

1. Run the server ./start.sh
2. Open the main source code 'index.html'
3. Open the fake code 'index_fake.html'
4. Go to 'index_fake.html', submit an transfer with '1000' value.
5. Go to 'index.html'
4. Reload the main project 'index.html'
5. Click submit with '1' value

Output: Current Balance: 0$

6. If reload, the current balance will continue to be $0.