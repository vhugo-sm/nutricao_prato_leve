# Prato Leve

Site de nutrição para quem quer comer melhor sem seguir uma dieta rígida. O conteúdo é dividido em três níveis (iniciante, intermediário e avançado), com visual simples e navegação fácil, inclusive no celular.

> Conteúdo informativo. Não substitui o acompanhamento de nutricionista ou médico.

## O que tem no site

- **Três níveis de dieta**
  - **Iniciante:** sem contar nada, com foco em montar o prato e criar rotina.
  - **Intermediário:** porções medidas pela mão, proteína em toda refeição e planejamento da semana.
  - **Avançado:** calorias e macros, carboidrato conforme o treino e ajustes pela média de peso.
- **Prato do dia:** gráfico em formato de prato com a divisão de vegetais, proteína, carboidrato e gorduras boas. No nível avançado dá para alternar entre dia de treino e dia de descanso.
- **Regras e cardápio de exemplo** para cada nível.
- **Checklist de hábitos da semana** com barra de progresso. O progresso fica salvo no navegador (`localStorage`).
- **Trocas que ajudam:** substituições simples de alimentos.
- **Calculadora de metas diárias:** estima calorias, proteína, carboidrato, gordura e água a partir de sexo, idade, peso, altura, atividade, objetivo e nível. Usa a equação de Mifflin-St Jeor.
- **Dúvidas comuns** em formato de lista expansível.
- **Responsivo** e com **modo claro e escuro** automático, seguindo o tema do aparelho.
- **Acessível:** abas com navegação pelo teclado (setas), foco visível e respeito à preferência de movimento reduzido.

## Tecnologias

- HTML, CSS e JavaScript puros, em um único arquivo, sem build e sem dependências.
- Fontes [Bricolage Grotesque](https://fonts.google.com/specimen/Bricolage+Grotesque) e [Inter](https://fonts.google.com/specimen/Inter), carregadas pelo Google Fonts.

## Como rodar localmente

1. Baixe ou clone o repositório.
2. Abra o arquivo `index.html` no navegador.

Não é preciso instalar nada.

## Como publicar no GitHub Pages

1. Envie os arquivos para um repositório no GitHub, com o `index.html` na raiz.
2. No repositório, abra **Settings > Pages**.
3. Em **Build and deployment**, escolha **Deploy from a branch**, selecione a branch `main` e a pasta `/ (root)`.
4. Salve. Em alguns minutos o site fica disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

## Estrutura do projeto

```
.
├── index.html   # site completo (HTML, CSS e JavaScript)
└── README.md
```

## Como personalizar

Tudo fica no `index.html`:

- **Cores e fontes:** variáveis no bloco `:root`, no começo do `<style>`. Há uma versão para o modo escuro logo abaixo.
- **Conteúdo dos níveis** (regras, cardápio, hábitos, trocas e proporções do prato): objeto `LEVELS`, no `<script>`.
- **Proteína por nível e fórmulas da calculadora:** objeto `PROT` e função `calc()`.

## Aviso sobre a calculadora

Os resultados são estimativas gerais para adultos saudáveis. Pessoas com condição de saúde, gestantes, lactantes, quem usa medicação contínua ou tem histórico de transtorno alimentar devem conversar com um profissional antes de mudar a alimentação.

## Licença

Defina a licença do projeto antes de publicar, por exemplo [MIT](https://choosealicense.com/licenses/mit/).
