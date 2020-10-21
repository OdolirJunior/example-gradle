# Exemplo criado para a apresentação do Trabalho sobre Gradle em Engenharia de Software ||

## Comandos


### 1° Exemplo 

## Requisitos 
- Gradle instalado e variavel de ambiente configurada
- JDK Instalada

#### Rodar aplicação 
- na raiz do projeto
- gradle -q build


### 2° Exemplo

#### Rodar aplicação direto no Jar

- Editar o nome do arquivo `build.gradle.old` para `build.gradle`
- na raiz do projeto
- gradle -q build
- cd build/libs
- java -jar .\example-1.0.jar

 Obs.: A partir desse jar pode ser feito um script  de deploy por exemplo. 
  
### 3° Exemplo

- Em outro diretório 
- Rodar o comando `Gradle init`
- Em `Select type of project to generate:` selecione 2.
- Em `Select implementation language:` selecione 3.
- Em  `Split functionality across multiple subprojects?:` selecione 1. (Caso queira ter vários builds separados selecionar 2.)
- Em `Select build script DSL:` selecione 1.
- Em `Select test framework:` selecione 1. 
- Mostrar arquivos
- Fazer test
- Fazer build
- Mostrar build.gradle e citar ant e maven
- Jcenter (Similar ao maven central ), onde é compartilhado os pacotes. Similar ao NPM no Node.
- Incluir no build.gradle:
```
jar {
    manifest {
        attributes 'Main-Class': 'example.aula.App'
    }
}
```
