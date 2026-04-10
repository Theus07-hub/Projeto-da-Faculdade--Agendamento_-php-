# Projeto-da-Faculdade--Agendamento\_-php-

O Arquivo vai ser criado para aprendizado Institucional e Profissional, ele ira direcionar-se a um sistema de agendamento de passeador de animais.

teste

prompt utilizado com CHATGPT para o auxilio dessa ativiadade: 

Quero ajuda para criar um UML de um sistema de agendamento
Depois quero melhorar ela com sua opinião
Depois quero colocar o README no GitHub usando CMD (Aprendizado para não esquecer)
Após quero que me ensine PHP do zero, com passo a passo detlhado se pular etapas.

# Sistema de Agendamento de passeador com animais.




\## Descrição

Projeto desenvolvido para gerenciar agendamentos de clientes para passear com seus animais(pet).



\## UML



```mermaid

classDiagram

class Tutor {
+nome: string
+telefone: int
}

class pet {
+nome: string
+idade: int
+porte: string
}

class Passeador {
+nome: string
+experiencia: string
}

class Agendamento {
+dataHora: datetime
+status: string
}

class Servico {
+tipo: string
+duracao: int
+valor: float
}

Tutor "1"--> "N"  Pet
Tutor "1"-->"N" Agendamento
Passeador "1" --> "N" Agendamento
Pet "1" --> "N" Agendamento
Servico "1" --> Agendamento


