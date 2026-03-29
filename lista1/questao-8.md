# Questão 8

## Sintaxe
- Negação (¬) → ! (C/Java) | not (Python)
- Conjunção (∧) → && (C/Java) | and (Python)
- Disjunção (∨) → || (C/Java) | or (Python)

### Linguagem C:
#### 1º Exemplo:
````c
int idade = 20;
int temCarteira = 1;

if (idade >= 18 && temCarteira) {
    printf("Pode dirigir\n");
}
````
> Usa ∧ (&&). Só executa o comando dentro do if se as duas condições forem verdadeiras.

#### 2º Exemplo:
````c
int chovendo = 0;
int frio = 1;

if (!chovendo || frio) {
    printf("Vou sair\n");
}
````
> Usa ¬ (!) e ∨ (||). Executa se não estiver chovendo ou se estiver frio.

### Java :
#### 1º Exemplo:
````java
int nota = 7;
int frequencia = 80;

if (nota >= 6 && frequencia >= 75) {
    System.out.println("Aprovado");
}
````
> Usa ∧ (&&). É necessário que as duas condições sejam verdadeiras.

#### 2º Exemplo:
````java
boolean loginValido;
boolean usuarioCorreto = true;
boolean senhaCorreta = false;

loginValido = usuarioCorreto && senhaCorreta;
````
> O resultado da expressão é atribuído a uma variável.
### Python :
#### 1º Exemplo:
````py
idade = 16
autorizacao = True

if idade >= 18 or autorizacao:
    print("Pode entrar")
````
> Usa ∨ (or). Basta uma das condições ser verdadeira.
#### 2º Exemplo:
````py
logado = True
admin = False

if not logado and admin:
    print("Acesso especial")
````
> Usa ¬ (not) e ∧ (and). Ambas as condições precisam ser verdadeiras.
