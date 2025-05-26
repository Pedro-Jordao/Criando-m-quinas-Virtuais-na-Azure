# Criando-maquinas-Virtuais-no-Azure
The following repository was created by me as part of a Bootcamp project for evaluation and approval purposes. Although it covers relatively simple topics and concepts, the work was completed in accordance with the requirements and criteria outlined in the Challenge Description.
# 📘 Projeto de Desafio - Bootcamp DIO

> ⚠️ O seguinte README refere-se a um projeto para a obtenção de nota ou aprovação em um Bootcamp da DIO e está de acordo com a respectiva **"Descrição do Desafio"** que possuir.  
> Em determinados casos, o projeto possui entregas **simplesmente visuais que sejam apresentadas neste README do GitHub**. Neste caso, a entrega do projeto será realizada por **meio deste arquivo**.

---

## 🎯 Objetivos do Projeto

- ✅ Aplicar os conceitos apresentados durante as aulas em um ambiente prático;
- ✅ Documentar o processo técnico de forma clara e estruturada;
- ✅ Utilizar o GitHub como ferramenta de versionamento e compartilhamento da documentação do projeto.

---

## 🛠️ Etapas Realizadas

Os seguintes passos foram realizados utilizando minha conta *Trial* no Azure:

---

### 🔹 Criação da Máquina Virtual

1. Acessei o **Marketplace** do Portal do Azure e busquei por *Virtual Machines*;
2. Cliquei em **Create** e selecionei o tipo de VM desejado;
![Create button](https://github.com/user-attachments/assets/b028e71a-86b9-42aa-90a8-7904d828d2c3)

---

### ⚙️ Tela *Basics*

- Defini a **Subscription** e o **Resource Group**;
- Nomeei a VM como: `PedroHJORlabmachine`;
- Região: `Brazil South`;
- Disponibilidade: *Sem infraestrutura de redundância*;
- Tipo de segurança: *Standard*;
- Imagem/SO: `Windows Server 2022 Datacenter: Azure Edition Hotpatch - x64 Gen2`;
- Tamanho: `Standard_B2s` (2 vCPUs, 4 GiB RAM - $54.90/mês);
- Configurei usuário e senha;
- Porta de entrada: **RDP (3389)**.

![Basicstela](https://github.com/user-attachments/assets/6b7283e4-d543-42f1-bb08-52607dc589ca)


---

### 💾 Tela *Disks*

- Tamanho do disco: `127 GiB`;
- Tipo: `Standard SSD - Locally-redundant storage`;
- Demais configurações mantidas como padrão.

![diskis tela](https://github.com/user-attachments/assets/f48c36ca-a3ae-4954-8de1-98917dd31c4d)

---

### 🌐 Tela *Networking*

Como minhas infraestruturas anteriores haviam sido deletadas, optei por:

- Permitir a criação automática da **VNET**, **IP público** e **Subnet**;
- Gerar o **NSG (Network Security Group)** vinculado à interface de rede da VM;
- Permitir acesso via **RDP (porta 3389)**;
- Configurar para que o **IP público** e a **interface de rede** sejam deletados junto com a VM;
- Não habilitei *Load Balancer*.

> ⚠️ *Reconheço que essas configurações não seguem as melhores práticas de segurança. Contudo, por se tratar de um ambiente de laboratório, optei por priorizar a simplicidade.*

![networkingtela](https://github.com/user-attachments/assets/05e5d237-ecc3-4426-afd8-18cc702c227a)

---

### 🔧 Tela *Management*

Embora a VM esteja destinada à exclusão após a conclusão deste repositório, mantive as configurações padrão, com exceção da ativação do **Auto-Shutdown** — uma boa prática que costumo aplicar em laboratórios, mesmo que não tenha utilidade prática neste caso.

![Management tela](https://github.com/user-attachments/assets/444b8602-fb70-47bd-994a-efffb77bc328)

---

### 📊 Tela *Monitoring*

- Mantive todas as configurações padrão.

---

### 🧪 Tela *Advanced*

- Nenhuma modificação foi realizada — mantido padrão.

---

### 🏷️ Tela *Tags*

- Adicionei **tags** para controle de *billing* e rastreabilidade dos custos associados ao Bootcamp, especialmente em casos de uso ou consumo de disco.

![image](https://github.com/user-attachments/assets/cdae8613-8e00-42b9-8c0a-4536000b3def)

---

### 🚀 Tela *Create & Deployment*

- Após a validação, cliquei em **Create**;
- O processo de **deployment** ocorreu normalmente e foi finalizado com sucesso.

![create tela](https://github.com/user-attachments/assets/cc3c4c37-327b-4e68-9aa8-ee1ce2848584)



![Tela deploy](https://github.com/user-attachments/assets/32adf043-5ff3-4385-b5f1-ff203a21a65a)



---

## 🧾 Notas Finais

Este README segue um modelo reutilizável para projetos desenvolvidos em bootcamps da DIO.  
As etapas descritas foram conduzidas com foco no aprendizado prático e documentação clara.

---
