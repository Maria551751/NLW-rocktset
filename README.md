
# 🎮 Assistente de Meta para Jogos com IA (Gemini)

Este é um projeto marcante na minha jornada de desenvolvimento web, representando meu **primeiro projeto completo e funcional que envolve a criação de um backend e a integração com uma Inteligência Artificial externa**. Desenvolvido com **JavaScript, HTML e CSS**, esta aplicação serve como uma assistente de meta interativa para diversos jogos, oferecendo estratégias, builds e dicas atualizadas. Todo o conhecimento e a base para a construção deste projeto vieram das excelentes aulas e mentorias fornecidas pela **Rocketseat**.

## 🚀 O Desafio e o Aprendizado

O principal objetivo deste projeto era solidificar meus conhecimentos em desenvolvimento web e, crucialmente, dar os primeiros passos no mundo da Inteligência Artificial. A integração com a API do Google Gemini representou um desafio excitante e uma grande oportunidade de aprendizado sobre como as IAs modernas podem ser incorporadas em aplicações web.

### Pontos Chave do Desenvolvimento:

-   **Frontend Responsivo:** Construção da interface do usuário (UI) utilizando HTML e CSS para garantir uma experiência amigável e adaptável em diferentes dispositivos.
-   **Interatividade com JavaScript:** Implementação da lógica do aplicativo no navegador, gerenciando eventos de formulário, exibição de respostas e validações iniciais.
-   **Consumo de API:** Aprendizado sobre como fazer requisições assíncronas (usando `fetch`) para interagir com serviços externos.
-   **Integração com IA (Google Gemini API):** O coração do projeto, onde a magia acontece. Configurei a comunicação com a API do Gemini para enviar as perguntas dos usuários e processar as respostas da IA.
-   **Criação de um Backend (Node.js com Express):**
    -   Esta foi uma etapa crucial para a **segurança** e a **escalabilidade**. Em vez de expor a chave da API Gemini diretamente no frontend (o que seria uma vulnerabilidade de segurança), desenvolvi um servidor backend simples.
    -   O frontend se comunica com este backend, que então, de forma segura, utiliza a chave da API para interagir com o Gemini e retorna a resposta para o frontend.
    -   Utilizei **`express.js`** para criar as rotas da API e **`dotenv`** para gerenciar variáveis de ambiente (onde a API Key é armazenada de forma segura).
    -   O módulo **`cors`** foi essencial para permitir a comunicação entre o frontend (rodando em uma porta) e o backend (rodando em outra).
    -   O **`node-fetch`** foi usado no backend para fazer as requisições HTTP para a API do Gemini.
-   **Personalização de Prompts por Jogo:** Implementei uma lógica no backend para que a IA receba instruções (prompts) personalizadas, dependendo do jogo selecionado pelo usuário. Isso melhora drasticamente a relevância e a qualidade das respostas da IA para cada título específico (ex: Valorant, League of Legends, CS:GO, Fortnite, Apex Legends, Overwatch 2, etc.).
-   **Renderização de Markdown:** Utilize a biblioteca **`Showdown.js`** no frontend para converter as respostas formatadas em Markdown da IA para HTML, garantindo uma apresentação visualmente agradável e estruturada.

## 🛠️ Tecnologias Utilizadas

-   **Frontend:**
    -   `HTML5`
    -   `CSS3`
    -   `JavaScript` (ES6+)
    -   `Showdown.js` (para renderização de Markdown)
-   **Backend:**
    -   `Node.js`
    -   `Express.js` (framework web)
    -   `dotenv` (para gerenciamento de variáveis de ambiente)
    -   `cors` (para Cross-Origin Resource Sharing)
    -   `node-fetch` (para requisições HTTP)
-   **Inteligência Artificial:**
    -   `Google Gemini API` (`gemini-2.5-flash` model)

## 🙏 Agradecimentos

Gostaria de expressar minha gratidão à **Rocketseat** pelas aulas de alta qualidade e pelo suporte, que foram fundamentais para a concepção e execução deste projeto. A experiência de aplicar o conhecimento adquirido em um projeto prático e funcional foi incrivelmente valiosa.

---
