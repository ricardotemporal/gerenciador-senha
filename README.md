# Gerenciador de Senhas

Este projeto é um Gerenciador de Senhas desenvolvido em Python, com o objetivo de criptografar, armazenar e recuperar senhas de forma segura. Ele utiliza o módulo cryptography para criptografia com o algoritmo Fernet e permite salvar as senhas em um formato criptografado.

## Funcionalidades

- Criação de Chave de Criptografia: Gera uma chave segura que pode ser salva para uso futuro.
- Armazenamento Seguro: As senhas são criptografadas e armazenadas em um banco de dados local em formato de texto.
- Recuperação de Senhas: Permite descriptografar e recuperar senhas de acordo com o domínio.
- Armazenamento em Arquivo: As senhas e a chave de criptografia podem ser salvas em arquivos.

## Estrutura do Projeto

Projeto/
├── db/                # Diretório onde as senhas criptografadas são salvas
├── keys/              # Diretório para armazenar a chave de criptografia
├── model/             # Contém a model para a representação das senhas
├── templates/         # Contém o arquivo principal do projeto (interface com o usuário)
├── view/              # Contém a lógica de criptografia e manipulação da chave
├── venv/              # Ambiente virtual para dependências do Python
└── README.md          # Arquivo com a documentação do projeto

## Requisitos

- Python 3.10 ou superior
- Biblioteca cryptography

## Instalação

1. Clone este repositório:

- git clone https://github.com/ricardotemporal/gerenciador-senhas.git

2. Navegue até o diretório do projeto:

- cd gerenciador-senhas

3. Crie um ambiente virtual e ative-o:

- python -m venv venv
- source venv/bin/activate  # Linux/macOS
- venv\Scripts\activate     # Windows

## Executando o Projeto:

Para iniciar o gerenciador de senhas, execute o arquivo template.py:
python templates/template.py

Escolha uma Ação:

1. Salvar uma nova senha:
Gere uma nova chave de criptografia (ou forneça uma existente).
Insira o domínio e a senha.

2. Ver uma senha existente:
Insira o domínio e a chave para descriptografar e recuperar a senha.

Exemplo de Interação
Digite 1 para salvar uma nova senha ou 2 para ver uma determinada senha: 1
Chave criada. Guarde-a com segurança.
Chave: [sua chave aqui]
Domínio: example.com
Senha: minha_senha_secreta

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar um pull request para melhorar este projeto.
