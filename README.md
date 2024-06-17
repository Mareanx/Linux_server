# 
![wallpaperflare-cropped](https://github.com/Mareanx/Linux_server/assets/104228036/89a393fd-92f0-427b-802f-1c624a30b74c)




# Ubuntu Server

***

## 1.Introdução

**Este wiki foi criado como parte de um trabalho para a disciplina de Redes 2 do curso de Ciência da Computação, ministrada pelo Professor Paulo Henrique.** O **objetivo** deste trabalho é fornecer aos alunos da disciplina um recurso abrangente e atualizado sobre o Ubuntu Server, ajudando-os a compreender e utilizar este poderoso sistema operacional em ambientes de rede. 

Ao longo deste wiki, os alunos poderão encontrar tutoriais detalhados sobre instalação, configuração e gerenciamento do Ubuntu Server, além de documentação oficial, dicas e truques, e acesso à comunidade de suporte vibrante. Espero que esta documentação seja um material de apoio valioso para os alunos da disciplina de Redes 2, contribuindo para o seu aprendizado e aprofundamento em conceitos de redes e sistemas operacionais Linux.

## 1.2 O que é o Ubuntu Server?

O Ubuntu Server se destaca como um sistema operacional gratuito e de código aberto baseado em Linux, projetado sob medida para o gerenciamento de servidores e infraestrutura de TI. Reconhecido por sua facilidade de uso, estabilidade, segurança robusta e um vasto leque de recursos, o Ubuntu Server se tornou a escolha preferida de administradores de rede e profissionais de TI em todo o mundo.


## 1.3 Mas o que realmente o torna tão especial?

### **Facilidade de Uso:**

* **Instalação descomplicada:** O processo de instalação é intuitivo e direto, mesmo para usuários iniciantes, minimizando a curva de aprendizado.

* **Interface amigável:** A interface gráfica padrão oferece um ambiente familiar e de fácil navegação, simplificando o gerenciamento das tarefas diárias.

* **Gerenciamento de pacotes eficiente:** O sistema de gerenciamento de pacotes apt permite a instalação, atualização e remoção de softwares com extrema praticidade, através de comandos simples e precisos.

### **Estabilidade Inabalável:**

* **Confiabilidade à prova de falhas:** O Ubuntu Server é reconhecido por sua estabilidade excepcional, minimizando o risco de travamentos e falhas inesperadas, garantindo a operação contínua dos seus servidores.

* **Atualizações frequentes:** As atualizações regulares de software e segurança garantem que seu sistema esteja sempre protegido contra as últimas ameaças e vulnerabilidades, mantendo a estabilidade e a confiabilidade ao longo do tempo.

### **Segurança Blindada:**

* **Fortaleza integrada:** O Ubuntu Server oferece diversos recursos de segurança integrados, como firewalls, autenticação robusta e criptografia de dados, protegendo seus servidores contra ataques cibernéticos e acessos não autorizados.

* **Comunidade vigilante:** Uma comunidade ativa e dedicada de desenvolvedores e especialistas em segurança trabalha incansavelmente para identificar e corrigir vulnerabilidades rapidamente, garantindo a proteção contínua do seu sistema.


## 1.4 **Agradecimentos:**

* Ao Professor Paulo Henrique pela oportunidade de desenvolver este trabalho e pela orientação durante a disciplina.

* À comunidade Ubuntu Server por fornecer recursos valiosos e uma plataforma de código aberto robusta.


## 1.5 **Observações:**

Este wiki é um trabalho em andamento e está sujeito a atualizações frequentes.

**Link Oficial da Documentação:** https://ubuntu.com/server/docs/tutorial

# Instalação dos recursos necessários

Este capítulo oferece uma visão geral do processo de instalação do Ubuntu Server. 

## 2.1 Requisitos do sistema

O Ubuntu Server Edition fornece uma base comum e minimalista para uma variedade de aplicativos de servidor, como serviços de arquivo/impressão, hospedagem na web, hospedagem de e-mail, etc. Esta versão oferece suporte a quatro arquiteturas de 64 bits:

* amd64 (Intel/AMD 64 bits)
* arm64 (ARM de 64 bits)
* ppc64el (POWER8 e POWER9)
* s390x (IBM Z e LinuxONE)

### 2.1.1 Os requisitos mínimos de sistema recomendados para este tutorial são:

* RAM: 2 GiB ou mais
* Disco: 5 GiB ou mais

## 2.2 Especificação do computador utilizado neste tutorial: 

* 13ª geração Intel® Core™ i5-13450HX (10-core, cache de 20MB, até 4.6GHz)
* Memória RAM: 16GB DDR5 (2x8GB) 4800MT/s
* Placa de Vídeo: NVIDIA® GeForce® RTX™ 3050, 6GB GDDR6
* Armazenamento: SSD de 512GB PCIe NVMe M.2
* Sistema Operacional: Linux Ubuntu 22.04


***

## 2.3 Baixe o ISO do servidor e a Máquina Virtual:

Você pode obter o download do servidor em https://ubuntu.com/download/server.: 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/cd561995-6bfe-4edc-babf-08ac22ef7cf5)

Outro software utilizado é a Oracle VM, caso seja preciso acesse o link https://www.virtualbox.org/wiki/Downloads e faça download para o sistema de sua preferência. 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/0c31ee25-6bd7-4bed-9e18-1b002c0983ca)




