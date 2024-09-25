# Sistema Inteligente para Vendas, Análise de Sentimentos e Detecção de Fraudes 🤖

Este projeto utiliza Python e a API da OpenAI para criar chatbots inteligentes.

## Índice 📇

1. [Sobre o Projeto](#sobre-o-projeto)
2. [Tecnologias Utilizadas](#tecnologias-utilizadas)
3. [Instalação](#instalação)
4. [Como Usar](#como-usar)
   - [Analisador de Sentimentos](#analisador-de-sentimentos)
   - [Detecção de Fraudes](#detecção-de-fraudes)
   - [Categorizador de Produtos](#categorizador-de-produtos)
5. [Contribuição](#contribuição)
6. [Contato](#contato)

---

## Sobre o Projeto 🗂️

Este sistema foi desenvolvido para ajudar empresas de vendas a melhorarem sua análise de feedbacks e detecção de fraudes. Ele oferece três funcionalidades principais:
- **Analisador de Sentimentos**: Avalia as avaliações dos clientes sobre produtos, identificando o sentimento geral, pontos fortes e fracos.
- **Detecção de Fraudes**: Analisa transações financeiras para identificar possíveis fraudes com base em padrões suspeitos.
- **Categorizador de Produtos**: Categorização de produtos com base no feedback dos clientes e na demanda de vendas.

## Tecnologias Utilizadas 💻

Este projeto faz uso das seguintes tecnologias:
- **Python**: Linguagem principal utilizada.
- **API da OpenAI**: Para análise de texto e criação de chatbots inteligentes.
- **dotenv**: Para gerenciamento seguro de variáveis de ambiente.
- **JSON**: Formato de dados para transações e comunicações entre serviços.

## Instalação ⚙️

Siga os passos abaixo para configurar o projeto localmente:

1. Clone este repositório:
   ```bash
   git clone https://github.com/rodrigoalmeida2/Chat_Bot_Openai.git

2. Acesse o diretório do projeto:
   ```bash
   cd nome-do-repositorio
3. Crie um ambiente virtual:
   ```bash
   python -m venv venv
     - Para acessar a venv:
       source venv/bin/activate  # No Windows: venv\Scripts\activate
4. Instale as dependências:
   ```bash
   pip install -r requirements.txt
5. Configure as variáveis de ambiente no arquivo .env, incluindo a chave da API da OpenAI:
   ```bash
   OPENAI_API_KEY=your-openai-api-key


## Como Usar 🤳🏾

**Analisador de Sentimentos**  
- Este módulo analisa avaliações de clientes sobre produtos e gera um relatório com sentimento geral, pontos fortes e fracos do produto:  
  1. Adicione as avaliações de um produto em um arquivo ```.txt``` no diretório ```./dados/``` com o nome ```avaliacoes-[nome_do_produto].txt```.
  2. Execute o analisador de sentimentos:
     ```bash
     python analisador_de_sentimentos.py
  3. O resultado será salvo no diretório ```./dados/``` como ```analise-[nome_do_produto].txt```.

**Detecção de Fraudes**  
- Este módulo analisa transações financeiras e determina se há possíveis fraudes:  
  1. Adicione um arquivo ```.csv``` com as transações no diretório ```./dados/```.
  2. Execute o analisador de transações:
     ```bash
     python analisador_transacoes.py
  3. O resultado será um arquivo JSON com a análise, incluindo o status da transação ("Aprovado" ou "Possível Fraude").  

**Categorizador de Produtos**  
- Baseado nas avaliações e nos feedbacks, este módulo categoriza os produtos conforme suas demandas e características:  
    1. O sistema utilizará as avaliações analisadas para sugerir categorias.  
    2. A execução é automática após a análise de sentimentos, gerando sugestões com base nas informações coletadas.

## Contribuição  🙏🏼
Contribuições são bem-vindas! Siga os passos abaixo:  

  - Faça um fork do repositório.
  - Crie uma branch com a sua feature
    ```bash
    git checkout -b feature/nova-feature
  - Commit suas mudanças
    ```bash
    git commit -m "Adiciona nova feature"
  - Envie para o repositório original
    ```bash
    git push origin feature/nova-feature
  - Abra um Pull Request.

## Contato  
<p align="left">
  <a href="mailto:rodrigoalmeida350.ra@gmail.com" title="Gmail">
  <img src="https://img.shields.io/badge/-Gmail-FF0000?style=flat-square&labelColor=FF0000&logo=gmail&logoColor=white&link=LINK-DO-SEU-GMAIL" alt="Gmail"/></a>
  <a href="https://www.linkedin.com/in/rodrigo101/" title="LinkedIn">
  <img src="https://img.shields.io/badge/-Linkedin-0e76a8?style=flat-square&logo=Linkedin&logoColor=white&link=LINK-DO-SEU-LINKEDIN" alt="LinkedIn"/></a>
  <a href="https://www.instagram.com/rodrigoalmeida2k/" title="Instagram">
  <img src="https://img.shields.io/badge/-Instagram-DF0174?style=flat-square&labelColor=DF0174&logo=instagram&logoColor=white&link=LINK-DO-SEU-INSTAGRAM" alt="Instagram"/></a>
</p>
