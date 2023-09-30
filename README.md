# jogojogo

class Heroi:
    def __init__(self, nome, idade, tipo):
        self.nome = nome
        self.idade = idade
        self.tipo = tipo

    def atacar(self):
        ataques = {
            "mago": "usou magia",
            "guerreiro": "usou espada",
            "monge": "usou artes marciais",
            "ninja": "usou shuriken"
        }
        ataque = ataques.get(self.tipo, "ataque desconhecido")
        return f"o {self.tipo} atacou usando {ataque}"

# Testando a classe:
heroi1 = Heroi("Merlin", 100, "mago")
print(heroi1.atacar())

heroi2 = Heroi("Arthur", 30, "guerreiro")
print(heroi2.atacar())

heroi3 = Heroi("Shifu", 60, "monge")
print(heroi3.atacar())

heroi4 = Heroi("Hanzo", 35, "ninja")
print(heroi4.atacar())

