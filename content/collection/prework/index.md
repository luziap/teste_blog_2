---
date: "2021-01-01"
draft: false
excerpt: How to prepare ahead of time.
subtitle: ""
title: Introdução ao R
weight: 1
---
Todas as análises de dados estão sendo realizadas usando o R e o RStudio. 

O R é um software livre e de código aberto com uma imensa comunidade de desenvolvedores e usuários nacionais e internacionais e cresce muito rapidamente. Dessa forma, há muito material disponível com exemplos em R. Assim sendo, com pequenas modificações em códigos prontos disponíveis é possível, por exemplo, realizar análises gráficas, ajustar modelos de previsão, criar aplicativos web, sites e muito mais. 
O RStudio é uma plataforma integrada ao R e oferece vários recursos que facilitam a importação, a edição dos comandos e a visualização dos resultados obtidos. 

O R e o RStudio são compatíveis com Windows, linux e mac. 


## Para instalar o R e o RStudio

A instação do R e do RStudio pode ser realizada, respectivamente, pelos links https://cran.r-project.org/ e https://rstudio.com/products/rstudio/download/. 

Caso surjam dúvidas durante a instalação vocês podem consultar, por exemplo, o roteiro para instalação do R e RStudio que preparei disponível neste [link]( https://drive.google.com/file/d/1J7MjR0CXjNwk_wYcpx9RElHoKTxToWgV/view?usp=sharing). Entretanto, esse roteiro foi feito para que utiliza o sistema operacional Windows.

Escolha as versões mais atualizadas. 

## Configurar o RStudio Cloud

Também é possível usar o R na nuvem, o que requer uma conexão com a internet. 

O RStudio Cloud pode ser acessado pelo link https://rstudio.cloud, sendo necessário criar uma conta no RStudio Cloud. Recomenda-se efetuar o login usando a sua conta Google para não ser necessário guardar uma nova senha.

Dê preferência para a instalação desses softwares em seu PC, pois poderá haver algumas incompatibilidades.


## Para instalar e carregar os pacotes no R

O R constituído por pacotes (packages) ou bibliotecas que são instaladas de acordo com a necessidade. Os pacotes ficam disponíveis no repositório do CRAN e todos são documentados.

Neste exemplo, estamos considerando os pacotes necessários para obter os gráficos do tutorial disponibilizado na OFICINA: Gerando gráficos com R e RStudio - excelência na análise de dados.

Uma forma para instalar os pacotes:

+ estando conectado a internet, copiar e colar a linha de comandos a seguir no editor do RStudio 

    ```r
    install.packages(c("summarytools", "fdth", "ggplot2", 
                       "readxl", "readr"))
    ```
Para rodar uma linha de comando devemos colocar o cursor em algum lugar da linha e clicar em **Run** no Menu superior no editor do RStudio.

Uma forma para carregar os pacotes:

+ copiar e colar as linhas de comandos a seguir no editor do RStudio 

    ```r
    require(summarytools)
    require(fdth)
    require(ggplot2)
    require(readxl)
    require(readr)

    ```

## Para entrada de dados no R 

#### Leitura de dados digitados


Algumas vezes quando se tem poucos dados pode ser conveniente digitá-los. Os exemplos a seguir ilustram a entrada de dados de variáveis qualitativa e quantitativa. Os exemplos utilizados são do livro de Anderson, David R.

##### Exemplo: variável qualitativa 

```r 
# Comandos de Entrada para ler os dados de uma variável qualitativa e armazená-los em ex1  

ex1 <- c("Coke Classic","Diet Coke","Pepsi","Diet Coke",
"Coke Classic","Coke Classic","Dr. Pepper","Diet Coke",
"Pepsi","Pepsi","Coke Classic","Dr. Pepper","Sprite","Coke Classic",
"Diet Coke","Coke Classic","Coke Classic","Sprite","Coke Classic","Diet Coke",
"Coke Classic","Diet Coke","Coke Classic",
"Sprite","Pepsi","Coke Classic","Coke Classic","Coke Classic",
"Pepsi","Coke Classic","Sprite","Dr. Pepper",
"Pepsi","Diet Coke","Pepsi","Coke Classic","Coke Classic",
"Coke Classic","Pepsi","Dr. Pepper","Coke Classic","Diet Coke",
"Pepsi","Pepsi","Pepsi","Pepsi","Coke Classic","Dr. Pepper","Pepsi","Sprite")

ex1 # para visualizar os dados

```


##### Exemplos: variável quantitativa 

```r 
ex2 <- c(2, 5, 10, 12, 4, 4, 5, 17, 11, 8, 9, 8, 12, 21, 6, 8, 7, 13, 18, 3) # tempo de espera em minutos de pacientes

ex2 # para visualizar os dados

x<- c(2, 5, 1, 3, 4, 1, 5, 3, 4, 2)  # número de comerciais

y<- c(50, 57, 41, 54, 54, 38, 63, 48, 59, 46)  # valores vendas (em milhares de reais)

x;y # para visualizar os dados

```


