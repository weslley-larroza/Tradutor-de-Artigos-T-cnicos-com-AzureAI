


# Tradução Automática de Artigos Técnicos com AzureAI

Este projeto foi desenvolvido como parte de um desafio no **Bootcamp Microsoft**, com o objetivo de criar uma solução de tradução automática de artigos técnicos, utilizando **Azure OpenAI**. A solução busca garantir precisão terminológica e contexto específico, facilitando o acesso a conteúdos especializados em diferentes idiomas.

## 🛠 Funcionalidades

- **Extração de texto**: Utiliza a biblioteca `BeautifulSoup` para extrair o conteúdo textual de páginas da web.
- **Tradução automática**: Integra a API do Azure OpenAI para realizar traduções com alta precisão.
- **Foco técnico**: O modelo é configurado para respeitar o contexto técnico do artigo traduzido.

## 🚀 Tecnologias Utilizadas

- **Python**: Linguagem principal para desenvolvimento.
- **Azure OpenAI**: API usada para tradução.
- **BeautifulSoup**: Para extração de texto de páginas HTML.
- **LangChain**: Gerenciamento da integração com o Azure.

## 📂 Estrutura do Código

- **`extract_text_from_url`**: Função para extrair o texto de uma URL fornecida.
- **`translate_article`**: Função que utiliza o Azure OpenAI para traduzir o conteúdo extraído.
- **Fluxo do projeto**:
  1. Extração do texto do artigo técnico.
  2. Tradução do conteúdo para o idioma escolhido.
  3. Exibição do texto traduzido no console.

## 🧑‍🏫 Sobre o Instrutor

Este projeto foi desenvolvido seguindo a aula do professor **Henrique Eduardo Souza**, **Microsoft MVP**, que forneceu orientações detalhadas sobre o uso do Azure OpenAI em soluções práticas.

## 📜 Pré-requisitos

1. **Conta no Azure**: Configure um endpoint para o Azure OpenAI.
2. **Chave de API**: Obtenha a chave da API no portal do Azure.
3. Instale as bibliotecas necessárias:
   ```bash
   pip install beautifulsoup4 requests langchain-openai
   ```

## 📝 Como Executar

1. Clone este repositório:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   cd <NOME_DO_DIRETORIO>
   ```
2. Configure suas credenciais do Azure OpenAI no código:
   ```python
   client = AzureChatOpenAI(
       api_key="SUA_CHAVE_DE_API",
       endpoint="SEU_ENDPOINT_AZURE",
       deployment_name="NOME_DO_DEPLOYMENT"
   )
   ```
3. Execute o script:
   ```bash
   python nome_do_arquivo.py
   ```
4. Informe a URL do artigo técnico e o idioma desejado.

## 📚 Exemplos de Uso

Entrada:
```python
url = 'https://exemplo.com/artigo-tecnico'
idioma = 'portuguese'
```

Saída:
```markdown
# Artigo Traduzido
Lorem ipsum dolor sit amet...
```

## 🌟 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
