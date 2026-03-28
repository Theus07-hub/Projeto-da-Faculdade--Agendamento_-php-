# Projeto-da-Faculdade--Agendamento\_-php-

O Arquivo vai ser criado para aprendizado Institucional e Profissional, ele ira direcionar-se a um sistema de agendamento de barbearia.

teste

prompt utilizado com CHATGPT para o auxilio dessa ativiadade: 
(
Crie um diagrama UML de classes para um sistema de agendamento de barbearia.

Requisitos:
O diagrama deve usar Mermaid (classDiagram)
Deve conter as classes: Cliente, Barbeiro, Servico e Agendamento
Incluir atributos básicos em cada classe
Mostrar os relacionamentos entre as classes (1:N)

Além disso:
Explique de forma simples o que o diagrama representa.

# Sistema de Agendamento de Barbearia



\## Descrição

Projeto desenvolvido para gerenciar agendamentos de clientes em uma barbearia.



\## UML



```mermaid

classDiagram

class Cliente {
+nome: string
+idade: int
}

class Agendamento {
+ dataHora: datetime
+ status: string
}

class Servico {
+valor: float
+nome: string
+duracao: int
}

class Barbeiro {
+ nome: string
}


Cliente "1"--> "N"  Agendamento
Barbeiro "1"-->"N" Agendamento
Agendamento "1" --> "1" Servico


