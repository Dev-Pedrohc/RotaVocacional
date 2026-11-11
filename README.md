# RotaVocacional

Projeto em grupo da faculdade: um sistema de **orientação vocacional**.

A ideia é ajudar a pessoa a explorar os próprios interesses e conhecer áreas profissionais, **sem dizer "essa é a sua carreira"**. O sistema não dá um veredito. Ele mostra caminhos possíveis, e quem decide é o usuário.

---

## O que o projeto faz

Muita gente chega no fim do ensino médio ou no meio da faculdade sem saber o que quer seguir. Os testes vocacionais que existem costumam entregar uma resposta fechada, tipo "você nasceu para ser X". A gente quis fazer diferente.

No RotaVocacional o usuário:

1. Se identifica (nome e dados básicos).
2. Responde perguntas sobre o que gosta de fazer, o que tem facilidade e como prefere trabalhar.
3. O sistema soma os pontos por área (tecnologia, saúde, comunicação, exatas, humanas, artes etc.).
4. Recebe um **ranking de áreas com maior afinidade**, com uma explicação do que cada área envolve e exemplos de profissões.
5. Pode refazer o teste e explorar outras áreas, mesmo as que não ficaram no topo.

## Nosso diferencial

Além de verificar qual área combina mais com a pessoa, a gente também quer **ajudar a escolher dentro da própria área**.

Exemplo: se o resultado for computação, o sistema não para aí. Ele mostra os caminhos dentro dela (desenvolvimento, redes, segurança, dados, jogos etc.) para a pessoa entender pra onde pode ir.

Também vamos discutir no grupo mais ideias para adicionar no site ao longo do projeto.

---

## Tecnologias

- **C**: o sistema em si (perguntas, cálculo de pontuação, manipulação de dados).
- **HTML e CSS**: a interface virtual do projeto, que é a parte que o usuário vê e usa.

---

## Estrutura do projeto

O sistema foi dividido em **funções/módulos**, e cada módulo fica com uma pessoa do grupo.

```
RotaVocacional/
├── src/
│   ├── usuario/         # cadastro e dados do usuário
│   ├── questionario/    # perguntas e coleta das respostas
│   ├── pontuacao/       # cálculo da afinidade por área
│   ├── areas/           # base de áreas e profissões
│   ├── resultado/       # montagem e exibição do resultado
│   └── interface/       # interface virtual (HTML e CSS)
├── include/             # arquivos de cabeçalho (.h)
├── data/                # arquivos com perguntas e áreas
├── main.c               # ponto de entrada do programa
└── README.md
```

> A estrutura pode mudar conforme o projeto avançar.

---

## Módulos e responsabilidades

| Módulo | O que faz | Responsável | Branch |
|---|---|---|---|
| Usuário | Cadastro e dados da pessoa | | `feature/usuario` |
| Questionário | Perguntas e respostas | | `feature/questionario` |
| Pontuação | Pontos por área e ranking | Pedro Candido | `feature/pontuacao` |
| Áreas e profissões | Descrição das áreas e carreiras | Carlos Eduardo | `feature/areas` |
| Resultado | Mostra o resultado final | Ronne | `feature/resultado` |
| Interface virtual | Parte visual que liga tudo | Emily e Taislayne | `feature/interface` |

---

## Interface virtual

Além do sistema funcionando, o projeto precisa de uma **interface virtual**, feita em **HTML e CSS**, para o usuário usar o programa de forma visual e organizada. O usuário navega pelas telas (início, perguntas, resultado) e a interface se conecta ao sistema em C por trás.

---

## Trabalho por branches

O projeto é feito por **branches**. A `main` só recebe código que já está funcionando, e cada integrante trabalha na sua própria branch, mexendo só no seu módulo. Quando termina, junta com a `main`. Assim ela não fica bagunçada.

### Como clonar o repositório

Você precisa ter o [Git](https://git-scm.com/) instalado.

```bash
git clone <link-do-repositorio>
cd RotaVocacional
```

---

## Como compilar e executar

```bash
gcc main.c src/**/*.c -o rotavocacional
./rotavocacional
```

---

## Integrantes

- Carlos
- Emily
- Enzo
- Iarley
- Pedro Candido
- Ronne
- Taislayne

---

## Observação

O RotaVocacional serve como ponto de partida para a pessoa se conhecer melhor. O resultado não é uma decisão de carreira, é só uma orientação para explorar.
