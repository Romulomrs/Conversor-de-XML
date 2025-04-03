Extrator de Informações de Notas Fiscais em XML

Este projeto tem como objetivo extrair informações de notas fiscais eletrônicas (NFe) em formato XML e exportá-las para um arquivo Excel (.xlsx).
📌 Funcionalidades

Lê arquivos XML de notas fiscais armazenados no diretório nfs.

Extrai informações relevantes, como:

Número da nota fiscal

Empresa emissora

Nome do cliente

Endereço do cliente

Peso da mercadoria transportada (caso disponível)

Gera um arquivo NotasFiscais.xlsx contendo todas as informações extraídas.


🛠 Tecnologias Utilizadas

Python

Bibliotecas:

xmltodict (para conversão do XML em dicionário Python)

pandas (para manipulação de dados e geração do Excel)

os (para manipulação de arquivos e diretórios)

📁 Projeto
│-- 📁 nfs
│   │-- arquivo1.xml
│   │-- arquivo2.xml
│   │-- ...
│-- extrair_nfes.py
│-- NotasFiscais.xlsx (gerado automaticamente)🚀 Como Utilizar

1️⃣ Instalar Dependências
Antes de executar o código, certifique-se de ter instalado as bibliotecas necessárias. Caso não tenha, execute o seguinte comando:
pip install xmltodict pandas

2️⃣ Adicionar os arquivos XML

Coloque os arquivos XML das notas fiscais dentro da pasta nfs.

3️⃣ Executar o Script

Execute o seguinte comando para extrair os dados e gerar o arquivo Excel:
python extrair_nfes.py

4️⃣ Verificar o Arquivo Gerado

Após a execução, um arquivo chamado NotasFiscais.xlsx será gerado na pasta do projeto, contendo as informações extraídas das notas fiscais.
❗ Observações

Caso uma nota fiscal não contenha informações sobre o peso, o script adicionará "Não informado" nessa coluna.

O script reconhece tanto arquivos XML com estrutura padrão (NFe) quanto arquivos encapsulados (nfeProc).

📞 Contato

Caso tenha dúvidas ou sugestões, fique à vontade para contribuir ou entrar em contato!
