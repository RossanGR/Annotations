# Annotations
General Annotations

# Springboot
## Arquitetura de pasta - MVC

 1. <b>Package Principal (base package):</b> Comece definindo um pacote principal para o seu projeto, geralmente usando o domínio reverso da sua empresa. Por exemplo, se o domínio da sua empresa for `com.example`, o pacote principal pode ser `com.example.myproject`.

Imagem 01

2. <b>Controllers:</b>
 Coloque os controladores (classes que respondem às requisições HTTP) em um pacote separado, como `controller` ou `api`.

Imagem 02

3. <b>Services:</b> Coloque as classes de serviço em um pacote como service. Essas classes geralmente contêm a lógica de negócios.

Imagem 03

4. <b>Repositories:</b> Se estiver usando o Spring Data JPA para acessar o banco de dados, você pode colocar suas interfaces de repositório em um pacote como `repository`.

Imagem 04

5. <b>Models:</b> Coloque suas classes de modelo (entidades) em um pacote como `model` ou `entity`. 
 

Imagem 05


6. <b>Configuration:</b> Para classes de configuração do Spring, como configurações de segurança, coloque-as em um pacote como `config`.
 

Imagem 06


7. <b>Exceptions:</b> Se você tiver classes de exceção personalizadas, coloque-as em um pacote como `exception` ou `error`.
 

Imagem 07


8. <b>Resources:</b> Mantenha arquivos de recursos, como arquivos de propriedades, no diretório `resources`.


Imagem 08


# Ordem de codificação

1. Models/Entity (Tabelas e relacionamentos do banco de dados).
2. Repository (Funções que "conversam" com os models).
3. Services (Possuí as regras de negócios, e é feito uma injeção de dependência do repository).
4. DTOS (São as classes de dados, que possuem os atributos pertencentes a essa entidade).
5. Controller (Onde é feito as chamadas HTTP).
