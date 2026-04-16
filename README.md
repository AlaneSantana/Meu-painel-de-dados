# 📝 Gerenciador Simples de Tarefas (Python)

<img 
    width="30px"
    style="padding-rigth: 10px;"
    src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-plain-wordmark.svg" 
/>    Este projeto é um pequeno programa em Python que permite ao usuário cadastrar tarefas e receber um feedback baseado na quantidade de atividades registradas. Ele utiliza listas, entrada de dados e estruturas condicionais — ótimo para quem está aprendendo lógica de programação.


# 🚀 Funcionalidades

Solicita o nome e a cidade do usuário.

Permite cadastrar uma lista de tarefas.

Exibe todas as tarefas cadastradas.

Analisa a quantidade de tarefas e retorna uma mensagem personalizada:

Nenhuma tarefa → mensagem informando ausência de tarefas

Até 3 tarefas → rotina leve

Mais de 3 tarefas → rotina cheia


# 📌 Como o programa funciona

O usuário informa:

Seu nome

Sua cidade

Quantas tarefas deseja cadastrar

O programa abre um loop para registrar cada tarefa digitada.

Após o cadastro, ele exibe:

A lista completa de tarefas

Uma mensagem personalizada baseada na quantidade de itens


# 🧩 Código

nome = input("Digite seu nome: ")
cidade = input("Digite sua cidade: ")

tarefas = []
qtd = int(input("Quantas tarefas você vai cadastrar? "))

for i in range(qtd):
    tarefa = input(f"Digite a tarefa {i+1}: ")
    tarefas.append(tarefa)

print("\nTarefas cadastradas:")
for t in tarefas:
    print("-", t)

if len(tarefas) == 0:
    print("Nenhuma tarefa cadastrada.")
elif len(tarefas) <= 3:
    print(f"\n{nome} de {cidade}: rotina leve hoje!")
else:
    print(f"\n{nome} de {cidade}: rotina cheia! Organize prioridades.")


# ▶️ Como executar

Certifique-se de ter o Python 3 instalado.

Salve o código em um arquivo, por exemplo:

Painel de Dados.py

Execute no terminal:

python Painel de Dados.py


# 📚 Conceitos utilizados

Listas (list)

Laços de repetição (for)

Entrada de dados (input)

Condicionais (if / elif / else)

Interpolação de strings com f-strings

