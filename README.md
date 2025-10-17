# ☁️ AWS CloudFormation — Laboratório Prático

## 🧩 Descrição
Este laboratório mostra como criar infraestrutura na AWS usando **CloudFormation**, serviço que permite descrever recursos como código.  
Aqui, criamos um **Bucket S3** e uma **Tabela DynamoDB**, documentando o processo e organizando imagens para estudo.

---

## 📚 O que é CloudFormation
O **AWS CloudFormation** permite criar, atualizar e deletar recursos da AWS de forma automática, usando **templates em YAML ou JSON**.  
Principais vantagens:
- Automatiza a criação de recursos (IaC)  
- Garante consistência entre ambientes  
- Permite versionar a infraestrutura junto ao código

- 
### Como funciona
1. Você escreve um **template.yaml** descrevendo os recursos que deseja criar.  
2. O CloudFormation interpreta o template e cria a **stack**, que é um conjunto de recursos interdependentes.  
3. Recursos podem ter **propriedades, dependências e tags**, permitindo controle detalhado.  
4. É possível atualizar a stack a qualquer momento, aplicando alterações de forma segura.

---

## 🛠️ Recursos Criados
- `MyS3Bucket` — Bucket S3 com versionamento habilitado  
- `MyDynamoDBTable` — Tabela DynamoDB com chave primária `ID` e modo PAY_PER_REQUEST  

---

## 🧾 Template
O arquivo principal do projeto é o `template.yaml`, que define os recursos acima de forma automatizada.

---

## Imagens

### Stack Creation.png
### 📘 Criação da Stack no AWS CloudFormation

Nesta imagem vemos o início da criação da pilha lab-s3-dynamodb usando o template template.yaml. É o momento em que os recursos (S3 e DynamoDB) ainda estão sendo provisionados pela AWS.
<img width="1773" height="166" alt="Stack Creation" src="https://github.com/user-attachments/assets/b9a390b5-d4a0-4d25-bafd-bd8d686b42ce" />

---



### stack-status.png
### ✅ Status da Stack – CREATE_COMPLETE
Aqui está o painel principal do CloudFormation mostrando que a stack foi criada com sucesso, com o status CREATE_COMPLETE. Isso confirma que o template foi executado sem erros.

<img width="1298" height="545" alt="stack-status png" src="https://github.com/user-attachments/assets/232869a9-e39b-4702-8c30-4b19f591cc45" />

---


### outputs.png
### 🧾 Saída do comando AWS CLI – Outputs da Stack
 Mostra o resultado do comando

<img width="724" height="443" alt="outputs png" src="https://github.com/user-attachments/assets/4aee1c91-8d8f-48e2-812f-2b27f45d462f" />

---

### s3-bucket.png
### 🪣 Bucket S3 criado pelo CloudFormation
Exibe o bucket S3 gerado pelo template, com o nome meu-bucket-cloudformation-<AccountID>.
Mostra também a região de criação (us-east-1) e confirma a data de provisionamento.

<img width="989" height="309" alt="s3-bucket png" src="https://github.com/user-attachments/assets/d3a545e5-caaf-4e54-9a25-53a91e0c6c44" />





