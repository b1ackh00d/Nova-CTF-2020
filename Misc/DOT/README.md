#### Question
 * Try to find the flag

   65794a68624763694f694a49557a49314e694973496e567a5a584a755957316c496a6f695957527461573469665165794a6d6247466e4d534936496b3576646d4637496977695a6d78685a7a49694f694a774e486c736232466b5832673063794973496d5a735957637a496a6f69596a4d7a626c3969636a42724d32347a5a483069665148653945616a765145613341667a72383874687072335537654b692d7243703577332d7a4934726a4b6b41

#### Hint
    Split the string at 92 and 264 :)

#### Solution

```
#!/usr/bin/python

def fun():
     fin = "65794a68624763694f694a49557a49314e694973496e567a5a584a755957316c496a6f695957527461573469665165794a6d6247466e4d534936496b3576646d4637496977695a6d78685a7a49694f694a774e486c736232466b5832673063794973496d5a735957637a496a6f69596a4d7a626c3969636a42724d32347a5a483069665148653945616a765145613341667a72383874687072335537654b692d7243703577332d7a4934726a4b6b41"
     aa = fin[:92]
     bb = fin[92:264]
     cc = fin[264:]
     return aa,bb,cc

l = fun()

print(l[0].decode("hex") + "." + l[1].decode("hex") + "." + l[2].decode("hex"))

#Output:
eyJhbGciOiJIUzI1NiIsInVzZXJuYW1lIjoiYWRtaW4ifQ.eyJmbGFnMSI6Ik5vdmF7IiwiZmxhZzIiOiJwNHlsb2FkX2g0cyIsImZsYWczIjoiYjMzbl9icjBrM24zZH0ifQ.He9EajvQEa3Afzr88thpr3U7eKi-rCp5w3-zI4rjKkA
```

#### Flag
    The output is nothing but DOTs separated base64URL encoded values generally known as JWT token.

    By visiting [jwt.io](https://jwt.io/#debugger-io?token=eyJhbGciOiJIUzI1NiIsInVzZXJuYW1lIjoiYWRtaW4ifQ.eyJmbGFnMSI6Ik5vdmF7IiwiZmxhZzIiOiJwNHlsb2FkX2g0cyIsImZsYWczIjoiYjMzbl9icjBrM24zZH0ifQ.He9EajvQEa3Afzr88thpr3U7eKi-rCp5w3-zI4rjKkA) we can easily see the decoded value(or payload) of this token.

    Flag : Nova{p4yload_h4sb33n_br0k3n3d}
