# AND, OR and NOT Operators

**AND** : specifies that both conditions must be met simultaneously 

example

```
SELECT *
FROM machines
WHERE operating_system='OS 1'
AND email_client='Email client 1';
```

---

**OR** : specifies that either condition can be met

example

```
SELECT *
FROM machines
WHERE operating_system='OS 1'
OR operating_system='OS 2';
```

---

**NOT** : negates a condition

example

```
SELECT *
FROM machines
WHERE NOT operating_system='OS 3'
```




































































