# Blog do Agi - Testes Automatizados

Este repositório contém uma suíte de testes automatizados desenvolvidos em Java usando Selenium WebDriver e JUnit para validar a funcionalidade de pesquisa no site Blog do Agi. O projeto inclui testes de funcionalidade e segurança, como SQL Injection.

## Requisitos

- Java 11 ou superior
- Maven 3.6 ou superior
- Google Chrome
- [WebDriverManager](https://github.com/bonigarcia/webdrivermanager)

## Configuração do Ambiente

1. **Clone o repositório:**

```bash
  git clone https://github.com/RBoker/agi-test.git
```
2. **Instale as dependências:**

Maven será usado para gerenciar as dependências do projeto. As dependências são listadas no arquivo pom.xml.
  
```bash
   mvn clean install
``` 
3. **Execute os testes:**

Para executar todos os testes, utilize o seguinte comando:
```bash
   mvn test
```
## Estrutura do Projeto
- src/test/java/br/com/rboker/blogdoagi/search/: Contém as classes de teste.
- SearchTests.java: Testes que seguem as boas práticas de programação.
- SqlInjectionTests.java: Teste que simula um ataque de SQL Injection para verificar vulnerabilidades.

## Detalhes dos Testes
1. `SearchTests.java`

Esta classe de testes contém cenários que verificam a funcionalidade de pesquisa no Blog do Agi:

- Pesquisar um termo existente: Verifica se a pesquisa por um termo válido retorna resultados relevantes.
- Pesquisar um termo inexistente: Verifica se a pesquisa por um termo inválido ou inexistente retorna a mensagem apropriada de "nenhum resultado encontrado".

2. `SqlInjectionTests.java`

   Este teste verifica se o campo de pesquisa do Blog do Agi é vulnerável a ataques de SQL Injection.

   **Atenção:** Este teste deve ser executado apenas em ambientes de teste controlados.


3. Um relatório simplificado da execução pode ser visto em:
````bash
target/site/surefire-report.html
````

## Contribuição
Contribuições são bem-vindas! Se você quiser contribuir com este projeto, siga estas etapas:

1. Faça um fork do repositório.

2. Crie uma nova branch com uma descrição significativa:

````bash
git checkout -b minha-feature
````
3. Faça as alterações necessárias e adicione testes para elas.

4. Envie suas alterações:

````bash
git push origin minha-feature
````
5. Abra um Pull Request.

## Licença
Este projeto é licenciado sob a licença MIT. Consulte o arquivo LICENSE para obter mais detalhes.

---

**Atenção:** Os testes de segurança, como o de SQL Injection, devem ser usados com responsabilidade. Nunca execute testes de vulnerabilidade em sistemas para os quais você não tem permissão explícita.

## Contato
Para dúvidas ou sugestões, entre em contato:

Nome: Roberto Boker

Email: rboker@gmail.com

LinkedIn: https://www.linkedin.com/in/roberto-boker-1b5b6530/


### Explicação do README

- **Introdução**: O README começa com uma introdução clara sobre o propósito do repositório, indicando que é uma suíte de testes para o site Blog do Agi.

- **Requisitos**: Especifica as dependências necessárias para rodar o projeto.

- **Configuração do Ambiente**: Passos detalhados sobre como clonar o repositório, instalar as dependências e rodar os testes.

- **Estrutura do Projeto**: Uma descrição básica da estrutura do código, ajudando novos desenvolvedores a entender onde encontrar os testes.

- **Detalhes dos Testes**: Explicação dos principais testes, com foco nas funcionalidades verificadas e na importância do teste de SQL Injection.

- **Contribuição**: Instruções claras para quem quiser contribuir com o projeto, incluindo como criar uma branch, fazer alterações e enviar um pull request.

- **Licença**: Informações sobre a licença do projeto.

- **Contato**: Informações para que os usuários possam entrar em contato com o autor do projeto.

Este README serve como um guia completo para entender, configurar e contribuir com o projeto.

