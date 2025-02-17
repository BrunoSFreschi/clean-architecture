# Clean Architecture Example
Este projeto é um exemplo simples de como implementar Clean Architecture em uma aplicação web usando ASP.NET Core. A Clean Architecture é um padrão de design que promove a separação de preocupações, tornando o código mais modular, testável e fácil de manter.

## Estrutura do Projeto
O projeto consiste em um único arquivo Program.cs que configura e inicia uma aplicação web minimalista. Apesar de simples, este exemplo demonstra os princípios fundamentais da Clean Architecture.

``` csharp

var builder = WebApplication.CreateBuilder(args);
var app = builder.Build();

app.MapGet("/", () => "Clean Architecture!");

app.Run();
```

## Por que este projeto é um exemplo de Clean Architecture?
### 1. Separação de Responsabilidades
- Clean Architecture promove a separação de responsabilidades em camadas. Embora este exemplo seja minimalista, ele segue o princípio de manter a lógica de negócios separada da infraestrutura e da apresentação.

- No exemplo, a rota "/" é responsável apenas por retornar uma mensagem, sem misturar lógica de negócios ou acesso a dados.

### 2. Independência de Frameworks
- A Clean Architecture enfatiza a independência de frameworks e bibliotecas externas. Neste exemplo, o uso do ASP.NET Core é mínimo e poderia ser facilmente substituído por outro framework sem afetar a lógica de negócios (se houvesse uma).

### 3. Testabilidade
- A simplicidade do código facilita a escrita de testes unitários e de integração. Como a lógica de negócios está separada da infraestrutura, os testes podem ser escritos de forma isolada.

### 4. Facilidade de Manutenção
- A clareza e a simplicidade do código tornam mais fácil a manutenção e a evolução do projeto. Novas funcionalidades podem ser adicionadas sem afetar o código existente.

### 5. Escalabilidade
- Embora este exemplo seja simples, a estrutura proposta pela Clean Architecture permite que o projeto cresça de forma organizada. Novas camadas (como domínio, aplicação e infraestrutura) podem ser adicionadas conforme necessário.

## Como Executar o Projeto
### 1. Pré-requisitos:

- .NET SDK instalado (versão 6 ou superior).

### 2. Executando o Projeto:

- Navegue até o diretório do projeto.

- Execute o comando:

``` dotnet run ```
- Abra o navegador e acesse http://localhost:5000 para ver a mensagem "Clean Architecture!".

## Conclusão
Este projeto, embora simples, é um exemplo de como os princípios da Clean Architecture podem ser aplicados mesmo em aplicações mínimas. A separação de responsabilidades, a independência de frameworks e a facilidade de manutenção são características que tornam a Clean Architecture uma escolha poderosa para projetos de qualquer tamanho.

### Nota: 
Você chegou aqui? Parabéns! Agora, se tiver dúvidas, você já sabe quem chamar. . .
