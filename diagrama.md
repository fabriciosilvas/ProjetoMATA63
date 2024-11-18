'''mermaid 
classDiagram
Responsável "1" -- "*" Estudante : possui
Estudante "1" -- "*" Irmao : possui
Estudante "1" -- "*" Alergia : possui
Estudante "1" -- "*" Restricao : possui
Estudante "1" -- "*" CuidadoEspecial : possui
Estudante "1" -- "*" Observacao : possui
Educador "1" -- "*" Observacao : realiza
Turma "1" -- "*" Estudante : possui
Caderneta "1" -- "1" Turma : possui
Caderneta "1" -- "*" Estudante : possui
Usuário <|-- Responsável
Usuário <|-- Estudante
Usuário <|-- Funcionário
Funcionário <|-- Secretário
Funcionário <|-- Gestor
Funcionário <|-- Educador

class Usuário {
    nome
    cpf
    rg
}
class Responsável {
    contato
    email
}
class Estudante {
    dataNascimento
    endereco
    certidaoNascimento
    serie
}
class Funcionário {
    
}
class Secretário {
    
}
class Gestor {
    
}

class Educador {
    
}

%%Não acredito ser necessário ter uma classe só para irmão, mas adicionei a fim de visualização
class Irmao {
    nome
}
class Alergia {
    produto
}
class Restricao {
    tipo
    descricao
}
class CuidadoEspecial {
    tipo
    descricao
}
class Observacao {
    %% tipo
    descricao
}
class Turma {
    serie
    educador1
    educador2
}
class Caderneta {
    
}
'''
