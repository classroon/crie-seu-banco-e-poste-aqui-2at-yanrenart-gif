[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/SUFPmDGs)
# 2AT--Crie-seu-banco

Crie-seu-banco-e-poste-aqui
📊 Atividade: Primeiros Passos com SQLite3
Nesta tarefa, você demonstrará que sabe operar o banco de dados SQLite diretamente pelo terminal, criando um arquivo de banco de dados, estruturando uma tabela e populando-a com informações.

🎯 Objetivo
Criar um banco de dados relacional contendo uma tabela de contatos e garantir que os dados sejam persistidos (salvos) e enviados para o seu repositório.

🛠️ Passo a Passo
Criar o Banco de Dados No terminal do seu Codespace, crie o arquivo do banco de dados utilizando o seu nome. Substitua seu_nome pelo seu nome real:
bash sqlite3 seu_nome.db

Use o código com cuidado.

2. Criar a Tabela
Dentro do prompt do SQLite (sqlite>), crie uma tabela chamada contatos com a seguinte estrutura: id: Número inteiro e Chave Primária (com incremento automático). nome: Texto (obrigatório). telefone: Texto. email: Texto (único). Comando:

sql CREATE TABLE contatos ( id INTEGER PRIMARY KEY AUTOINCREMENT, nome TEXT NOT NULL, telefone TEXT, email TEXT UNIQUE ); Use o código com cuidado.

3. Inserir Registros
Insira pelo menos 3 registros diferentes na tabela para popular o banco. Exemplo de comando:

sql INSERT INTO contatos (nome, telefone, email) VALUES ('Ana Silva', '11 98888-7777', 'ana@email.com'); Use o código com cuidado.

(Repita o processo mudando os dados para completar os 3 registros).

4. Validar e Sair
Para garantir que deu tudo certo: Digite SELECT * FROM contatos; e verifique se os 3 nomes aparecem. Saia do SQLite digitando .exit ou .quit.

#📤 Entrega (Git) Para que eu possa corrigir, você precisa enviar o arquivo .db para o GitHub. Use os comandos abaixo no terminal:

bash git add seu_nome.db git commit -m "Tarefa SQLite: Banco e tabela de contatos criados" git push origin main Use o código com cuidado.

⚠️ Observações Importantes:
Não esqueça o ponto e vírgula (;) ao final dos comandos SQL. O arquivo .db deve estar na raiz do projeto. Atenção: Se você ficar "preso" no prompt ...> , digite ; e dê Enter.
