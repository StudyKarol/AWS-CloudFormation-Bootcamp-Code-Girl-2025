**Bootcamp Code Girl 2025 – Santander**

---

## 1. ☁️ AWS CloudFormation

Durante as aulas, aprendi que o **AWS CloudFormation** é uma ferramenta poderosa de **Infraestrutura como Código (IaC)**.  
Ela permite **criar, gerenciar e atualizar recursos na AWS de forma automatizada**, usando **templates declarativos**.  
Isso garante que a infraestrutura seja **reproduzível e consistente**, evitando erros manuais que podem ocorrer quando se cria recursos manualmente pelo console da AWS.

---

## 2. 🚀 Benefícios do AWS CloudFormation e Formatos de Modelos

**Principais benefícios que destaquei:**

-  **Automação e consistência:** recursos criados de forma repetível.  
-  **Redução de erros humanos:** evita configurações manuais incorretas.  
-  **Versionamento e rastreabilidade:** templates podem ser versionados e armazenados em repositórios.  
-  **Reusabilidade e modularidade:** templates podem ser divididos em módulos e reutilizados em diferentes projetos.  

 **Observação:**  
Os templates podem ser escritos em **YAML** ou **JSON**, sendo o **YAML mais legível** e recomendado para uso em ambientes de estudo e produção.

---

## 3. 🛠️ Acessando o AWS CloudFormation e Criando uma Stack

Durante as práticas, acessamos o **AWS CloudFormation** pelo console da AWS e criamos nossa **primeira stack**.  

 Uma **stack** é um *conjunto de recursos* que podem ser gerenciados como uma unidade única.

 Exploramos o **CloudFormation Designer**, ferramenta que permite visualizar a arquitetura de forma gráfica.

 Testamos:
- Criação de stacks  
- Atualização de parâmetros  
- Exclusão de recursos  

E entendemos o impacto de cada ação nos recursos provisionados.

---

## 4. ⚖️ Diferença entre AWS CloudFormation e Terraform

Durante a aula, discutimos as diferenças entre **CloudFormation** e **Terraform**:

| Ferramenta | Características Principais |
|-------------|-----------------------------|
| **CloudFormation** | Nativo da AWS, gerencia apenas recursos da AWS, integração total com outros serviços AWS. |
| **Terraform** | Ferramenta multi-cloud, suporta diferentes provedores, mas requer configuração adicional para integração profunda com a AWS. |

📌 **Insight:**  
Para ambientes **exclusivamente AWS**, o CloudFormation oferece **integração mais nativa e simplificada**.

---

## 5. 🧩 Entendendo o Desafio

O desafio do bootcamp consistia em **provisionar uma infraestrutura básica automatizada** usando CloudFormation, aplicando os conceitos de IaC e garantindo que a stack fosse:

-  **Reproduzível**  
-  **Modular**  
-  **Documentada**

Durante a prática, percebi que:
-  A clareza do template é essencial para manutenção futura.  
-  É importante testar atualizações em ambientes de desenvolvimento antes de aplicar em produção.  
-  Documentar cada recurso e parâmetro facilita a compreensão e colaboração com outros desenvolvedores.  

---

## 6. 🎯 Conclusão e Insights Pessoais

Essa experiência mostrou como a **automação da infraestrutura é fundamental** para ambientes de nuvem escaláveis e confiáveis.  
Também compreendi que **a leitura e construção de templates CloudFormation é uma habilidade essencial** para qualquer profissional de DevOps ou engenheiro de nuvem.  

###  O que aprendi:

- IaC não é só sobre escrever código, mas também sobre **planejamento, testes e documentação**.  
- Comparar ferramentas (**CloudFormation x Terraform**) ajuda a escolher a melhor abordagem para cada cenário.  
-  **Praticar a criação e modificação de stacks** é a melhor forma de consolidar os conceitos.  

---

### 📎 Exemplo de Template CloudFormation (YAML)

```yaml
AWSTemplateFormatVersion: '2010-09-09'
Description: Karollyne Cabrau - Bootcamp Code Girl 2025

Resources:
  MyS3Bucket:
    Type: AWS::S3::Bucket
    Properties:
      BucketName: exemplo-cloudformation-bootcamp
