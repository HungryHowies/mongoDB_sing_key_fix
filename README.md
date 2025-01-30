Error:
```
The following signatures were invalid: EXPKEYSIG 656408E390CFB1F5 MongoDB 4.4 Release Signing Key
```
Fix:

```
curl -fsSL https://www.mongodb.org/static/pgp/server-4.4.asc | \
   sudo gpg -o /usr/share/keyrings/mongodb-server-4.4.gpg \
   --dearmor
```
