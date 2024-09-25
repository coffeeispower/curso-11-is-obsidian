---
tags: [sibd, slides]
modulo: 1
---

## Evolução dos Sistemas

[[Bancos de dados]]
![[Banco de dados]]

---

## Dec. 50
### Como se guardavam dados antigamente?

---

## Papel
![[Pasted image 20240923091658.png]]

---

Que guardavam em pastas

![[Pasted Image 20240923092104_325.png|360]]

---

E depois guardavam essas pastas em arquivos:

![[Pasted image 20240923091351.png]]

---

## Qual seria a evolução de arquivos físicos?

---

### Computadores da altura
Eram grandes e usavam **fitas magnéticas** e **cartões perfurados** que eram **sequenciais**.
![[Pasted image 20240923105833.png|550]]

---

### Bancos de dados sequenciais

![[Pasted image 20240923105516.png|230]]

---
#### Computador ↓
![](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExaWYyamFmZWdqMHM4YjhoeXV1cWh6ZDY4YXVtNXZ4OTJpeGk4cnZveiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/WoWm8YzFQJg5i/giphy.webp)

---

# Década de 1960

---

- Os **HDs** apareceram
- HDs permitem acessar **qualquer informação** em **qualquer lugar** do disco **sem precisar de rebobinar** uma fita
- Começamos a precisar de armazenar informação de maneira **mais organizada** e em um **volume maior**

---

![[Pasted image 20240925091427.png]]

---

# SQL
## Structured Query Language
Uma linguagem padronizada para comandar bancos de dados relacionais.

---

#### Bancos de dados relacionais trabalham com tabelas interligadas

![[Drawing 2024-09-25 09.19.06.excalidraw|1000]]

---

## Relação com o que era feito antigamente

- **Papéis** se transformaram em **registros** ou **linhas** nas tabelas
- As **pastas** se transformaram nas **tabelas**
- E os **arquivos** se transformaram em **bancos de dados**

---

# Comandos básicos

---

Criar tabelas

```sql
CREATE TABLE produtos(
	-- NOT NULL: precisa de sempre estar preenchido
	id INT NOT NULL,
	nome TEXT NOT NULL,
	valor DOUBLE NOT NULL,
	-- ENUM("USD", "EUR"): apenas pode conter "USD ou "EUR"
	moeda ENUM("USD", "EUR") NOT NULL,
	-- A tabela não pode ter IDs repetidos
	PRIMARY KEY (id)
);
```

---

Comentários
```sql
-- Comentários começam com -- em cada linha
```

---

Procurar registros nas tabelas

```sql
SELECT 
	-- Buscar as colunas nome, valor e moeda
	nome, valor, moeda
FROM produtos -- dos registros da tabela de faturas
WHERE id = 1; -- em que o id é igual a 1
```
![[Drawing 2024-09-25 09.19.06.excalidraw 1|700]]

---
Adicionar registros:
```sql
-- Inserir nos produtos uma linha
INSERT INTO produto(
	-- com as colunas id, nome, valor e moeda
	id, nome, valor, moeda
)
-- com os valores 4, "Adaptador HDMI para VGA", 3,00 e "USD" respectivamente
VALUES (3, "Adaptador HDMI para VGA", 3.00, "USD");
```

![[Drawing 2024-09-25 10.41.40.excalidraw]]

---
# Software de Gestão de Banco de Dados (SGBD)
- **MySQL**: O mais popular
- **PostgreSQL**: Mais novo e com mais funcionalidades
- **Microsoft SQL Server**: Melhor maneira de gastar dinheiro atoa

---
# Fontes
- [Curso MySQL #01 - O que é um Banco de Dados? - Youtube](https://www.youtube.com/watch?v=Ofktsne-utM)