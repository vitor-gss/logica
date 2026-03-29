````
Algoritmo ClassificarSentenca

Entrada: sentenca

Passo 1: extrair todas as proposicoes da sentenca
variaveis ← lista de proposicoes (ex: P, Q, R)

Passo 2: gerar todas as combinacoes possíveis de V/F
n ← tamanho(variaveis)
total ← 2^n

temVerdadeiro ← falso
temFalso ← falso

Para i de 0 até total-1 faça:
    
    atribuicao ← gerar combinação de V/F para as variaveis
    
    resultado ← avaliar(sentenca, atribuicao)
    
    Se resultado = verdadeiro então
        temVerdadeiro ← verdadeiro
    Senão
        temFalso ← verdadeiro
    FimSe

FimPara

Passo 3: classificar

Se temVerdadeiro = verdadeiro e temFalso = falso então
    escreva "Tautologia"
Senão se temVerdadeiro = falso e temFalso = verdadeiro então
    escreva "Contradição"
Senão
    escreva "Satisfatível"
FimSe

FimAlgoritmo
````
````
Função avaliar(sentenca, atribuicao)

Substituir cada proposição pelos valores V/F

Resolver:
¬ (negação)
∧ (e)
∨ (ou)
→ (implica)
↔ (bi-implica)

Retornar resultado final (V ou F)

FimFunção
````
