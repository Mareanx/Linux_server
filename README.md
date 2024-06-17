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

***

## Criando nossa Máquina Virtual: 

Com todos os recursos necessários instalados, vamos criar nossa máquina virtual com o arquivo _.iso_ 

## 3. Criando a Máquina Virtual com VirtualBox

Primeiro iremos abrir a VirtualBox: 

![Captura de tela de 2024-06-17 17-24-22](https://github.com/Mareanx/Linux_server/assets/104228036/f9104443-168c-4bb5-9a27-a878385eea64)

Após aberta, clicaremos em **"Novo"**, aparecerá a seguinte tela (**nomeie da forma que desejar**): 

![Captura de tela de 2024-06-17 17-24-51](https://github.com/Mareanx/Linux_server/assets/104228036/c88055ec-9c99-444c-a925-88eb9d348daa)

Vá em próximo e selecione a quantidade de memória RAM que será alocada na máquina virtual (e**u selecionei 8000MB**): 

![Captura de tela de 2024-06-17 17-29-10](https://github.com/Mareanx/Linux_server/assets/104228036/214bd3a4-647f-492d-8eb0-b7ad5853de10)

Prossiga clicando em próximo e selecione a opção de criar um novo disco rígido virtual: 

![Captura de tela de 2024-06-17 17-32-25](https://github.com/Mareanx/Linux_server/assets/104228036/8626f65d-2286-493b-9d28-9ebbe5d3f80b)

Selecione a primeira opção (**VDI**) e clique em próximo: 

![Captura de tela de 2024-06-17 17-33-29](https://github.com/Mareanx/Linux_server/assets/104228036/dcbf4bbb-a736-498a-83a5-5f50e99f7bf3)

Na tela de armazenamento em disco rígido físico selecione a opção de dinamicamente alocado e prossiga clicando em próximo:

![image](https://github.com/Mareanx/Linux_server/assets/104228036/30005448-b61b-4d7f-9edc-5ddaf6383010)

Deixe desta forma e clique em criar: 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/0e326d53-529a-4a41-bb21-9bc8bb0be34d)

Prontinho, a máquina virtual foi criada 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/c33dedaa-c1a9-4fe2-a79e-86c2db6e0f75)

## 3.1 Adicionando o arquivo .iso na máquina virtual: 

Agora com nossa máquina criada clicaremos em iniciar: 


![Captura de tela de 2024-06-17 17-41-02](https://github.com/Mareanx/Linux_server/assets/104228036/5bc13cf6-126f-41c8-83c3-10fca06d03dd)

Ao clicar em iniciar, irá aparece a opção de alterar o arquivo .iso clicando no ícone ao lado do nome do arquivo: 

![Captura de tela de 2024-06-17 17-42-16](https://github.com/Mareanx/Linux_server/assets/104228036/0ec22025-af0e-4a9c-bdff-0e9ac2705f8a)

Após clicar no ícone irá aparecer a seguinte tela, clique em acrescentar: 

![Captura de tela de 2024-06-17 17-42-38](https://github.com/Mareanx/Linux_server/assets/104228036/92e5851b-6a17-4f93-9a3b-80970f9e0c0a)

Ao clicar em acrescentar vá até a pasta na qual o arquivo .iso foi baixado: 

![Captura de tela de 2024-06-17 17-54-04](https://github.com/Mareanx/Linux_server/assets/104228036/168f2004-1806-4f70-9c75-1eb454901259)

Prossiga

![Captura de tela de 2024-06-17 17-54-33](https://github.com/Mareanx/Linux_server/assets/104228036/2bbcf5e1-b8b3-43f2-9e88-4f2d300920d6)

Aparecerá a seguinte tela: 

![Captura de tela de 2024-06-17 17-55-01](https://github.com/Mareanx/Linux_server/assets/104228036/63486559-7bae-4cd7-9feb-48975fddb86a)

Aperte enter com a primeira opção selecionada para realizar a instalação: 

![Captura de tela de 2024-06-17 17-56-01](https://github.com/Mareanx/Linux_server/assets/104228036/8fede69d-9eee-4293-9ba0-09c824633cb5)

Depois da instalação ser concluída aparacerá a seguinte tela: 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/a7802425-6449-4548-a2bd-f9783f83613e)

Selecione o idioma desejado, eu optei por português, mas fica a seu critério: 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/94bf0473-983c-4a68-aec6-7c1ccfa1d633)

Dê enter, vai aparecer a seguinte tela: 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/8d7c1b79-e0d0-4ba3-9217-243b0e0db19e)

Dê enter novamente com a opção "concluído" selecionada.

Deixe a opção de "Ubuntu Server" selecionada e dê enter novamente

![Captura de tela de 2024-06-17 18-02-41](https://github.com/Mareanx/Linux_server/assets/104228036/06c37cc9-6454-4ec1-a6c0-5f6a8b33ef9f)


Nessa etapa, as informações de rede são coletadas automaticamente caso você esteja conectado à internet. Se sua conexão estiver indisponível, não se preocupe! Basta clicar em "Continuar sem rede" para prosseguir com a instalação.

![image](https://github.com/Mareanx/Linux_server/assets/104228036/4aae882f-5149-4805-9718-23a759910f3d)

Não iremos fazer nenhuma alteração, dê enter novamente

![image](https://github.com/Mareanx/Linux_server/assets/104228036/7b04ce66-d610-4cd9-bef8-e0e87f38a9ff)

Neste momento não iremos fazer nenhuma configuração de proxy então prossiga normalmente 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/816b8ddd-13d9-46db-99db-3618a874815c)

Neste momento não iremos fazer nenhuma configuração de disco, então basta prosseguir dando enter. 


![Captura de tela de 2024-06-17 18-12-41](https://github.com/Mareanx/Linux_server/assets/104228036/9a252395-8a05-463a-9db1-23106b79b13b)


![Captura de tela de 2024-06-17 18-12-48](https://github.com/Mareanx/Linux_server/assets/104228036/1c50c7ef-f96a-4aef-9958-e2ac45d2aad3)

Após confirmar que todas as informações estão corretas, clique em "Continuar" para prosseguir com a instalação.

![image](https://github.com/Mareanx/Linux_server/assets/104228036/883870e2-3c35-4388-898d-b56bd631177f)

Agora iremos configurar nosso server: 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/0ea0ab6f-890e-4e3f-baf1-dc58b6e671f5)

Preencha conforme sua preferência: 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/1f2415b5-fec6-4f44-9b68-818c3d189f9b)

Conclua.

Mantenha a opção "skip for now"  

![image](https://github.com/Mareanx/Linux_server/assets/104228036/a1b3c9da-cffc-433d-a21c-0da5c4c22f92)

Prossiga em "Continue"

Nessa etapa, o instalador oferece a opção de instalar o serviço SSH. Como vamos configurá-lo manualmente mais tarde, vamos desativar essa opção por enquanto.

![image](https://github.com/Mareanx/Linux_server/assets/104228036/87058e6e-86ca-4304-8183-835f1566b2ad)

Conclua.

Nesta etapa da instalação, você verá uma janela apresentando os pacotes de software populares do Ubuntu. Apesar de não serem necessários no momento, o instalador os oferece para sua conveniência. Apenas conclua. 

![Captura de tela de 2024-06-17 18-23-45](https://github.com/Mareanx/Linux_server/assets/104228036/d8ecb035-5176-4d81-a217-0b5d2fb7ec40)

Irá aparecer a seguinte tela: 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/3a36402d-f844-4481-8c6a-7414aa8ea518)

Após a instalação ser concluída, vá em "reboot now"

![image](https://github.com/Mareanx/Linux_server/assets/104228036/aa1867e9-ac10-4182-ba92-a8db4764c631)

Prontinho, terminamos a etapa de instalação: 

![image](https://github.com/Mareanx/Linux_server/assets/104228036/cb47cd18-3cf2-49af-abcc-52c0c92d4ce8)









