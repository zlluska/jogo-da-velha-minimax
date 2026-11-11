# 🧠 Algoritmos de Busca e Decisão em Python: Minimax & Backtracking

![Python](https://img.shields.io/badge/Python_3-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Algorithms](https://img.shields.io/badge/Algoritmos-IA_&_Grafos-FF6F00?style=for-the-badge)

Implementações práticas em Python de algoritmos clássicos de **Inteligência Artificial (Teoria dos Jogos)** e **Busca em Espaço de Estados (Backtracking)** para encontrar decisões ótimas e caminhos mínimos.

---

## 📂 Estrutura do Repositório

| Arquivo | Algoritmo | Descrição |
| :--- | :--- | :--- |
| [`mini.py`](./mini.py) | **Minimax (Com Profundidade)** | Agente invencível de **Jogo da Velha (Tic-Tac-Toe)** que avalia recursivamente toda a árvore de possibilidades para maximizar sua chance de vitória no menor número de jogadas. |
| [`teste.py`](./teste.py) | **Backtracking (Menor Caminho)** | Algoritmo de busca exaustiva com retrocesso (*backtracking*) em matriz 2D para encontrar o **caminho mais curto** entre a origem `(0,0)` e o destino `(3,3)` desviando de obstáculos (`X`). |

---

## 🎮 1. Jogo da Velha Invencível (`mini.py`)

O algoritmo **Minimax** simula todas as jogadas futuras possíveis assumindo que o oponente humano (`X`) também jogará da melhor forma possível:

- **Vitória da IA (`O`):** Pontuação `+10 - profundidade` (prefere vencer o mais rápido possível).
- **Vitória do Jogador (`X`):** Pontuação `-10 + profundidade` (posterga derrotas caso estivesse em posição perdida).
- **Empate:** Pontuação `0`.

### Como jogar:
```bash
python mini.py
```
Escolha uma posição de `0` a `8` conforme o mapa do tabuleiro:
```text
0 | 1 | 2
--+---+--
3 | 4 | 5
--+---+--
6 | 7 | 8
```

---

## 🧩 2. Menor Caminho em Labirinto com Backtracking (`teste.py`)

Percorre o grid em 4 direções (baixo, cima, direita, esquerda), marcando células visitadas e desfazendo a escolha (*backtrack*) ao atingir um beco sem saída ou após registrar um caminho válido menor que o melhor encontrado até então.

### Como executar:
```bash
python teste.py
```

### Exemplo de Saída:
```text
Melhor Caminho Encontrado:
| |*|X| |
|X|*|X| |
| |*|*|*|
| |X|X| |
```

---

## 👤 Autor

**Lucas Fraga** — [GitHub (@zlluska)](https://github.com/zlluska)
