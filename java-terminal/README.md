## Anotações

### Gerar documentação

`javadoc -encoding UTF-8 -docencoding ISO-8859-1  -d ../docs  src/*.java`

### Executar programa Java via terminal

 - Localizar arquivo .class na pasta bin do seu projeto
 - Acessar este caminho da pasta pelo terminal ou cmd ou powershell
 - Supondo que sua classe se chame `MinhaClasse.java`, rodar comando `java MinhaClasse` no terminal. Não se deve informar a extensão `.class` ao rodar comando

### Para que serve o parâmetro `String[] args` do método main?

 - Serve para passar parâmetros do tipo String quando você executar alguma classe do seu projeto através do cmd, PowerShell ou terminal, através do comando
 
 `java NomeDaSuaClasse parametro1 parametro2 parametro3 parametro4...`,

 Exemplo:

 `java AboutMe GLEYSON SAMPAIO 28 1.58`

  - Para usar os parâmetros passados dentro do método main, como parâmetro args é um array de strings, para informar o índice do array que você quer acessar. Você pode inclusive salvar o conteúdo que está neste índice do array em uma variável.

  Exemplo:

  `String nome = args [0];`

### Passando valores aos argumentos pelo VsCode.

 - Run -> Add Configuration -> Java
 - Dentro da pasta `.vscode`, será criado um arquivo `launch.json`. Dentro dele, é possível criar um parâmetro para sua classe chamado `"args"`, onde você pode informar os valores que deseja passar como parâmetro.

 Exemplo:

 ```
 {
    "version": "0.2.0",
    "configurations": [
        {
            "type": "java",
            "request": "launch",
            "mainClass": "AboutMe",
            "args": ["GLEYSON", "SAMPAIO", "28", "1.58"]
        }
    ]
}
 ```

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
