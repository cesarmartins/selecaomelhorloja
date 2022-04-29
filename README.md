# Você quer ser um desenvolvedor Backend na Melhor Loja Virtal?
Criamos esse teste para avaliar seus conhecimentos e habilidades como desenvolvedor backend.

# O teste
O desafio é desenvolver um sistema de gerenciamento de produtos. Esse sistema será composto de um cadastro de produtos e categorias. Os requisitos desse sistema estão listados nos tópicos abaixo.
Não existe certo ou errado, queremos saber como você se sai em situações reais como esse desafio.

# Instruções
- O foco principal do nosso teste é o backend. Para facilitar você poderá utilizar os arquivos html  disponíveis no diretório assets
- Crie essa aplicação como se fosse uma aplicação real, que seria utilizada pelo WebJump
- Fique à vontade para usar bibliotecas/componentes externos (composer)
- Não utilize nenhum Framework, tais como Laravel, Lumen ou Symphony
- Seguir princípios **SOLID** 
- Utilize boas práticas de programação
- Utilize boas práticas de git
- Documentar como rodar o projeto
- Crie uma documentação simples comentando sobre as tecnologias, versões e soluções adotadas

# Requisitos
- O sistema deverá ser desenvolvido utilizando a linguagem PHP (de preferência a versão mais nova) ou outra linguagem se assim foi especificado para sua avaliação por nossa equipe.
- Você deve criar um CRUD que permita cadastrar as seguintes informações:
	- **Produto**: Nome, SKU (Código), preço, descrição, quantidade e categoria (cada produto pode conter uma ou mais categorias)
	- **Categoria**: Código e nome.
- Salvar as informações necessárias em um banco de dados (relacional ou não), de sua escolha

# Opcionais
- Gerar logs das ações
- Testes automatizados com informação da cobertura de testes
- Upload de imagem no cadastro de produtos

# O que será avaliado
- Estrutura e organização do código e dos arquivos
- Soluções adotadas
- Tecnologias utilizadas
- Qualidade
- Padrões PSR, Design Patterns
- Enfim, tudo será observado e levado em conta

# Como iniciar o desenvolvimento
- **Fork** esse repositório na sua conta do BitBucket.
- Crie uma branch com o nome **desafio**

# Como enviar seu teste
Envie um email para [vempra@melhorlojavirtual.com.br] com o link do seu repositório.

Se o seu repositório for privado, conceda acesso aos emails: vempra@melhorlojavirtual.com.br, cesar@melhorlojavirtual.com.br, samuel@melhorlojavirtual.com.br.

Qualquer dúvida sobre o teste, fique a vontade para entrar em contato conosco.



CREATE TABLE `acde91dd_veneza_6`.`produtos` (
`idprodutos` INT NOT NULL AUTO_INCREMENT,
`skuprodutos` VARCHAR(45) NULL,
`nameprodutos` VARCHAR(255) NULL,
`priceprodutos` FLOAT NULL,
`descriptonprodutos` VARCHAR(45) NULL,
`photoprodutoscol` VARCHAR(255) NULL,
`ativoprodutos` VARCHAR(45) NULL,
PRIMARY KEY (`idprodutos`));

CREATE TABLE `db_desafio`.`produtos_categorias` (
`idprodutos_categorias` INT NOT NULL AUTO_INCREMENT,
`idproduto` VARCHAR(45) NULL,
`idcategoria` VARCHAR(45) NULL,
PRIMARY KEY (`idprodutos_categorias`));

CREATE TABLE `db_desafio`.`categorias` (
`idcategorias` INT NOT NULL AUTO_INCREMENT,
`namecategorias` VARCHAR(255) NULL,
PRIMARY KEY (`idcategorias`));
