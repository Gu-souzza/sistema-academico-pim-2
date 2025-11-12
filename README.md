Projeto Integrado Multidisciplinar do curso de ADS.
# 🎓 Sistema de Gestão Acadêmica (PIM)

Este é um Projeto Integrado Multidisciplinar (PIM) para o 2º Semestre, focado no desenvolvimento de um sistema de gerenciamento acadêmico. A aplicação permite o controle completo de alunos, disciplinas, turmas e o respectivo desempenho acadêmico.

## 🚀 Funcionalidades Principais

O sistema permite realizar as seguintes operações (CRUD):

* **Alunos:** Cadastrar, consultar, alterar e excluir alunos.
* **Disciplinas:** Cadastrar, consultar, alterar e excluir disciplinas.
* **Turmas:** Cadastrar, consultar, alterar e excluir turmas.
* **Matrículas:** Matricular alunos em turmas/disciplinas.
* **Boletim:** Lançar notas (NP1, NP2, PIM), controlar faltas e consultar o boletim final com média e status (Aprovado/Reprovado).

## 🛠️ Arquitetura e Tecnologias

Este projeto utiliza uma arquitetura híbrida para otimizar o desempenho:

* **Python (`app.py`):**
    Usado para a interface principal do usuário (menu) e para orquestrar a lógica de alto nível.

* **Linguagem C (`database.c`):**
    Usada para o *core* do sistema. As funções de manipulação de arquivos (ler, escrever, buscar) foram escritas em C e compiladas em uma biblioteca (`.dll`) para máxima velocidade.

* **Arquivos `.dat` (Banco de Dados):**
    Os dados (alunos, matérias, etc.) são armazenados em arquivos binários (`.dat`) para persistência de dados.

## 🏁 Como Executar

1.  Certifique-se de que a biblioteca `database.dll` está compilada e na mesma pasta.
2.  Execute o script principal Python:

```bash
python app.py
