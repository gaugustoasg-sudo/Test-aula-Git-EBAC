# Instruções do que se encontra no projeto. *** Importante ***

## Calculadora executável Linux Ubunto- 

Objetivo: executar o arquivo nome_do_executavel, uma calculadora básica que exibe informações sobre o diretório em que está e, em seguida, abre a calculadora do sistema operacional.

Passo a passo:

1 - Abra o terminal. 
2 - Use o atalho Ctrl + Alt + T ou procure por "Terminal" no menu de aplicativos.
3 - Acesse a pasta onde o arquivo está salvo. 
4 - Use o comando cd seguido do caminho da pasta. 

Por exemplo:
cd ~/Downloads

Confira se o arquivo está na pasta. Liste o conteúdo do diretório com:

ls

Dê permissão de execução ao arquivo. Por padrão, o Linux não permite executar arquivos baixados. Use:

chmod +x calculadora.sh

Execute o programa. Digite:

./calculadora.sh

O que deve acontecer:

* O programa exibe no terminal as informações do diretório em que está sendo executado (por exemplo, o caminho atual e os arquivos presentes nele).
* Em seguida, a calculadora padrão do Ubuntu é aberta automaticamente, e você pode usá-la normalmente.

Observação: se aparecer a mensagem "Permissão negada", repita o passo 4. Se aparecer "Arquivo ou diretório inexistente", confira se você está na pasta correta (passos 2 e 3).


## Calculadora de simulação de rebaixamento brasileirão. 

⚽ Análise de Risco de Rebaixamento

Programa em Python que avalia a possibilidade de rebaixamento de um time do Campeonato Brasileiro, com base no desempenho recente.

## 📋 Cenário

- O time tem **35 pontos**.
- Restam **5 partidas** para o fim do campeonato (38ª rodada).
- Pontuação de segurança adotada: **45 pontos** (referência aproximada).

> Este é um programa simples, que não consulta a internet e não se baseia na realidade atual.

## ▶️ Como executar

1. Tenha o Python 3 instalado.
2. Salve o código em um arquivo, por exemplo `rebaixamento.py`.
3. No terminal, execute:

## 🧠 Como o código funciona

### 1. Constantes do cenário
Define os valores fixos: pontos atuais (35), jogos restantes (5) e pontuação de segurança (45).

### 2. Entrada de dados (`input`)
O programa pergunta:
- O nome do time;
- Quantas partidas recentes serão analisadas;
- Quantos pontos o time fez nessas partidas;
- Quantas vitórias o time teve nessas partidas.

Os valores numéricos são convertidos para inteiros com `int()`, pois o `input` sempre retorna texto.

### 3. Operações matemáticas
- **Divisão:** média de pontos por partida (`pontos_recentes / partidas`).
- **Multiplicação:** projeção de pontos nos jogos restantes.
- **Soma:** total projetado ao fim do campeonato.
- **Subtração:** pontos que faltam para chegar aos 45.

O **aproveitamento necessário** é calculado dividindo os pontos que faltam pelos pontos em disputa (5 jogos × 3 = 15). No cenário fixo, o time precisa de 10 dos 15 pontos, ou seja, cerca de **66,7%**.

### 4. Laço de repetição (`while`)
Enquanto o usuário responder `s`, o programa repete a análise, permitindo testar diferentes situações sem reiniciar.

### 5. Condicional (`if/else`)
- Se o total projetado for **maior ou igual a 45**, o time deve escapar do rebaixamento.
- Caso contrário, o time continua na **zona de risco**.

### 6. Saída (`print`)
O programa exibe:
- Média de pontos nas últimas partidas;
- Número de vitórias nas últimas partidas;
- % de aproveitamento necessário nos jogos restantes;
- Pontuação projetada e avaliação de risco.

## 📌 Exemplo de saída

```text
--- Análise do Flamengo ---
Média de pontos nas últimas 5 partidas: 1.60
Número de vitórias nas últimas 5 partidas: 2
Aproveitamento necessário nos 5 jogos restantes: 66.7%
Pontuação projetada ao fim do campeonato: 43.0
Situação: atenção! Nesse ritmo, o time continua na zona de risco.
python3 rebaixamento.py
