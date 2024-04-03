```
SELECT
	U.USUARIO,
	dbo.decrypt(U.SENHA) as SENHA,
	u.NOME,
	u.PADRAO
FROM
	HD_USUARIO U
WHERE
	U.USUARIO = 'zeus';
```
