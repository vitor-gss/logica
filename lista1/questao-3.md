````
Algoritmo VerificarEquivalencia

Entrada: sentenca1, sentenca2

Passo 1: extrair proposições das duas sentenças
variaveis ← união das variáveis de sentenca1 e sentenca2

n ← tamanho(variaveis)
total ← 2^n

equivalente ← verdadeiro

Para i de 0 até total-1 faça:

    atribuicao ← gerar combinação de V/F
    
    resultado1 ← avaliar(sentenca1, atribuicao)
    resultado2 ← avaliar(sentenca2, atribuicao)
    
    Se resultado1 ≠ resultado2 então
        equivalente ← falso
    FimSe

FimPara

Passo 3: resultado final

Se equivalente = verdadeiro então
    escreva "As sentenças são logicamente equivalentes"
Senão
    escreva "As sentenças NÃO são equivalentes"
FimSe

FimAlgoritmo
````

````
Função avaliar(sentenca, atribuicao)

Substituir variáveis por V/F

Resolver operadores:
¬, ∧, ∨, →, ↔

Retornar V ou F

FimFunção
````
### Exemplo 1: 
- ¬(P ∧ Q)
- ¬P ∨ ¬Q

| P   | Q   | ¬(P∧Q)| ¬P∨¬Q |
| --- | --- | ----- | ----- |
| V | V | F | F |
| V | F | V | V |
| F | V | V | V |
| F | F | V | V |
> Equivalentes

### Exemplo 2: 
- P ∨ Q
- P ∧ Q

| P   | Q   | P ∨ Q | P ∧ Q |
| --- | --- | ----- | ----- |
| V | V | V | V |
| V | F | V | F |
| F | V | V | F |
| F | F | F | F |
> Não Equivalentes

### Exemplo 3: 
- P → Q
- ¬P ∨ Q

| P   | Q   | P → Q | ¬P ∨ Q |
| --- | --- | ----- | ----- |
| V | V | V | V |
| V | F | F | F |
| F | V | V | V |
| F | F | V | V |
> Equivalentes
