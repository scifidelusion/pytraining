class Produto:
    def __init__(self, nome, preco, quantidade):
        self.nome = nome
        self.preco = preco
        self.quantidade = quantidade

class ProdutoFisico(Produto):
    def __init__(self, nome, preco, quantidade, peso):
        super().__init__(nome, preco, quantidade)
        self.peso = peso

    def calcular_frete(self, distancia):
        # Simulação de cálculo de frete baseado no peso e na distância
        return self.peso * distancia * 0.1  # Valor fictício de frete

class ProdutoDigital(Produto):
    def __init__(self, nome, preco, quantidade, tamanho_em_mb):
        super().__init__(nome, preco, quantidade)
        self.tamanho_em_mb = tamanho_em_mb

    def calcular_tamanho_em_mb(self):
        return self.tamanho_em_mb


# Exemplo de uso das classes
produto_fisico = ProdutoFisico("Livro", 29.99, 10, 0.5)
frete = produto_fisico.calcular_frete(100)  # Supondo uma distância de 100 km
print("Frete do Produto Físico:", frete)

produto_digital = ProdutoDigital("E-book", 19.99, 50, 10)
tamanho = produto_digital.calcular_tamanho_em_mb()
print("Tamanho do Produto Digital:", tamanho, "MB")



class Produto:
    def __int__(self, nome, preco, quantidade):
        self.nome = nome
        self.preco = preco
        self.quantidade = quantidade

class ProdutoFisico(Produto):
    def __int__(self, nome, preco, quantidade, peso):
        super().__init__(nome, preco, quantidade)
        self.peso = peso

    def calcular_frete(self, distancia):
        return self.peso * distancia * 0.1

class ProdutoDigital(Produto):
    def __int__(self, nome, preco, quantidade, tamanho_em_mb):
        super().__init__(self, nome, preco, quantidade)
        self.tamanho_em_mb = tamanho_em_mb
