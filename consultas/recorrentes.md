# 📑 Consultas Recorrentes

Validar o padrão do usuario:
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
Caso tenha executado o SetupBD ou o retorno do select acima tenha retornado o PADRAO = GERAL, execute o comando abaixo:
```
UPDATE HD_USUARIO SET PADRAO = NULL WHERE USUARIO = 'zeus';
```
Senha do Aluno:
```
select a.nome_compl, a.aluno, dbo.decrypt(p.senha_tac) senha, a.sit_aluno, a.curso, a.turno, a.curriculo, a.serie, a.turma_pref, a.PESSOA, p.SENHA_TAC
from ly_aluno a
inner join ly_pessoa p on (a.pessoa = p.pessoa)
where a.ALUNO = '1410001'
```
Alterar senha do aluno:
```
DECLARE @senhaNova VARCHAR(200);
SET @senhaNova = dbo.Crypt('aluno');
UPDATE LY_PESSOA SET SENHA_TAC = @senhaNova WHERE PESSOA = 274627;
```
Obter responsável (pai/mãe) e senha para logar no AOR que possua filho matriculado:
```
SELECT PESSOA_PAPEL, PR.CPF, PR.e_MAIL, DBO.DECRYPT(SENHA_TAC) FROM LY_RELACIONAMENTO_PESSOA R JOIN LY_PESSOA PR ON R.PESSOA_pAPEL=PR.PESSOA  
WHERE EXISTS (SELECT 1 FROM LY_PESSOA P JOIN LY_ALUNO A ON P.PESSOA=A.PESSOA AND R.PESSOA=P.PESSOA 
WHERE EXISTS (SELECT 1 FROM LY_MATRICULA M WHERE M.ALUNO=A.ALUNO)) 
AND R.ON_LINE='S'
```
