# Classificador-N-vel-de-Her-i
Desafio para o curso de lógica em programação frontend DIO
# Desafio Classificador de Nível de Herói 🦸‍♀️⚔️

## O que rolou aqui?

Fiz um código simples e direto pra classificar o nível de um herói baseado na XP dele.  
Não inventei muito, segui a lógica dos intervalos usando **if/else** porque, sinceramente, achei que o switch case não era a melhor escolha pra esse caso (e tava certa).

## Como funciona?

- Criei uma variável fixa pra guardar o nome do herói (`nomeHeroi`), porque o exercício não pediu input.  
- A XP também foi fixada numa variável (`xp`) pra testar os níveis.  
- Usei uma sequência de `if` e `else if` pra verificar em qual faixa a XP se encaixa e definir o nível correspondente.  
- Por fim, o código imprime no console uma mensagem bonitinha dizendo o nome do herói e o nível dele.

## O que aprendi?

- Que `if/else` é pra comparar intervalos, e switch case é mais pra casos de valores fixos.  
- Que Node não tem `prompt()`, então pra input no terminal tem que usar outro esquema (mas isso deixei de lado aqui pois quis deixar o projeto mais simples).  
- Que const é melhor pra valores fixos, let pra variáveis que vão mudar durante a execução.  
- Que a lógica simples, quando bem feita, já resolve.

## Próximos Passos
- Pretendo utilizar esse projeto para exercitar também minhas habilidades com HTML, CSS  e Javascript, fazendo um seletor de classe para personagens de RPG. Com interface, personagens e interacoes dinamicas.

## Código que usei

```js
const nomeHeroi = "Rama";
let xp = 6000;
let nivel = "";

if (xp <= 1000) {
  nivel = "Ferro";
} else if (xp <= 2000) {
  nivel = "Bronze";
} else if (xp <= 5000) {
  nivel = "Prata";
} else if (xp <= 7000) {
  nivel = "Ouro";
} else if (xp <= 8000) {
  nivel = "Platina";
} else if (xp <= 9000) {
  nivel = "Ascendente";
} else if (xp <= 10000) {
  nivel = "Imortal";
} else {
  nivel = "Radiante";
}

console.log(`O Herói de nome ${nomeHeroi} está no nível de ${nivel}`);