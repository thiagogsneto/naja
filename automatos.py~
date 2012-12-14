import estado

automatos = {}
#-------------------------- IDENTIFICADOR
estados = []
estados.append(Estado("q0", False))
estados.append(Estado("q1", False))
estados.append(Estado("q2", True))

estados[0].set_transicoes({"minusculo": estados[1],"maiusculo": estados[1],"_": estados[1]})
estados[1].set_transicoes({"minusculo": estados[1],"maiusculo": estados[1],"digito":estados[1],"_": estados[1],"outro":estados[2]})

automatos["identificador"] = Automato(estados, estados[0])


#-------------------------- COMENTARIO
estados = []
estados.append(Estado("q0", False))
estados.append(Estado("q1", False))
estados.append(Estado("q2", True))

estados[0].set_transicoes({"#": estados[1]})
estados[1].set_transicoes({"\r\n": estados[2],"outro":estados[1]})

automatos["comentario"] = Automato(estados, estados[0])



