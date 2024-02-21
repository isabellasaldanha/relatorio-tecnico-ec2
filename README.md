# 📋 Relatório Técnico sobre Acesso SSH no EC2

## 🤔 Introdução

O Amazon EC2 é um serviço que fornece computação em nuvem com máquinas virtuais escaláveis de acordo com a demanda, enquanto o SSH é um protocolo que garante a segurança do acesso remoto a sistemas e servidores. Eles são comumente usados em conjunto, possibilitando que os administradores de sistemas possam controlar e configurar suas instâncias EC2 de forma protegida.

## ☝️ Objetivo

Este relatório abordará o processo de instalação de uma instância EC2 na AWS e demonstrará como acessá-la utilizando SSH por meio da ferramenta PUTTY.

## 📒 Materiais

Navegador com acesso a internet  
Conta na AWS  
PUTTY instalado  

# Método

## Logando na conta AWS e selecionando o EC2

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_1.png?raw=true">

Ao entrar em sua conta AWS, acesse o serviço EC2 para criar sua instância.

## Criando a primeira instância

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_2.png?raw=true">

Depois de acessar o EC2 e suas respectivas instâncias, selecione o botão "Executar instância" para acessar a tela de criação de instância.

## Nomeando a instância

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_3.png?raw=true">

Agora, nomeie sua instância de acordo com seu projeto pessoal, nesse caso de exemplo será "ec2-bella".

## Escolhendo o tipo de imagem

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_4.png?raw=true">

Rolando para baixo você encontrará a opção para escolher qual imagem de máquina irá utilizar. Para esse exemplo será utilizado o Amazon Linux. Ao selecionar a imagem do Amazon Linux, consideramos sua ampla compatibilidade e otimização para ambientes de nuvem.

## Escolhendo o tipo de instância

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_5.png?raw=true">

Em seguida, você deverá escolher qual instância irá utilizar, como esse projeto se trata de um exemplo iremos utilizar a t1.micro. Em casos de projetos maiores talvez seja necessário utilizar outros tipos de instâncias.

## Criando o par de chaves

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_6.png?raw=true">

Ao rolar para baixo você poderá encontrar a opção de criar um novo par de chaves, selecione ela. É essencial criar um novo par de chaves para garantir a segurança da instância. 

## Configurando o par de chaves

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_7.png?raw=true">

Certifique-se de nomear a chave de acordo com suas preferências e selecione o formato ".ppk" para permitir a conexão SSH via PuTTY.

## Execute a instância

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_8.png?raw=true">

Após todas as configurações serem realizada, selecione "Executar instância" para verificar se tudo foi feito corretamente.

## Instância executada

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_9.png?raw=true">

Caso tudo tenha sido feito corretamente, a instância será executada com sucesso.

## Salvando o IP 

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_10.png?raw=true">

Após iniciar a instância, é importante copiar e salvar o endereço IP atribuído. Este endereço será necessário para acessar a instância posteriormente.

## Abra o aplicativo PUTTY

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_11.png?raw=true">

Após isso, abra o PUTTY e cole seu endereço IP no "Host Name".

## Adicione suas credenciais

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_12.png?raw=true">

Ainda dentro do PUTTY, acesse "Credentials" no menu lateral e faça o upload do seu par de chaves salvo anteriormente em "Private key file for autentication" e em seguida selecione "Open".

## Acesse sua máquina

<img width="960" src="https://github.com/isabellasaldanha/relatorio-tecnico-ec2/blob/main/img/passo_14.png?raw=true">

Após aparecer o terminal, digite "ec2-user" e aperte enter. Agora sua maquina já estará rodando!

# 🤩 Resultado

Após todos os procedimentos serem realizados de forma correta, será possível ter criado uma instância EC2 e acessá-la usando SSH.

# 😎 Conclusão

Por meio desse relatório, conseguimos entender detalhamente o passo a passo da criação de uma instância no EC2, bem como suas configurações e criação de um par de chaves SSH que possibilitou o acesso via PUTTY por meio dessas credenciais, trazendo segurança para nosso serviço.


