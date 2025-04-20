## Anotações

### Exeções checadas (checked) e não checadas (unchecked)

 - Exceções checadas são exceções onde é facultativo seu tratamento, normalmente uma RunTimeException.
 Um exemplo disso é a função valueOf da classe Double, onde, na sua hierarquia de exceções, lança uma NumberFormatException, herdada da classe IllegalArgumentException, que por sua vez é herdada da classe RunTimeException.

 - Já exceções não checadas são exceções que precisam ser tratadas imediatamente quando ocorrem, como por exemplo, a exceção ParseException, que herda da classe Exception. Uma das ocasiões em que esta exceção pode ocorrer é no uso da função parse() da classe NumberFormat, onde ao informar um parâmetro impossível de ser convertido para o tipo Number, lançará esta exceção. Normalmente, quando ocorre uma exceção não checada, a própria IDE que você utiliza, antes mesmo de você rodar o projeto, já identifica um possível erro e sugere alguma correção, como encapsular o trecho de código em um bloco try/catch.

## Getting Started

Welcome to the VS Code Java world. Here is a guideline to help you get started to write Java code in Visual Studio Code.

## Folder Structure

The workspace contains two folders by default, where:

- `src`: the folder to maintain sources
- `lib`: the folder to maintain dependencies

Meanwhile, the compiled output files will be generated in the `bin` folder by default.

> If you want to customize the folder structure, open `.vscode/settings.json` and update the related settings there.

## Dependency Management

The `JAVA PROJECTS` view allows you to manage your dependencies. More details can be found [here](https://github.com/microsoft/vscode-java-dependency#manage-dependencies).
