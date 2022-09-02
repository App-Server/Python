# Python
# pyodbc
# terminal
# install pyodbc

import pyodbc
dados_conexao = (
    "Driver=;" 
    "Server=DESKTOP-T2JV7P5;"
    "Database=;"
)
# Prompt de Comando
    # C:\Users\Python>hostname
    # DESKTOP-T2JV7P5
    # C:\Users\Python>
conexao = pyodbc.connect(dados_conexao)
print("Conexão Bem Sucedido")
cursor = conexao.cursor()
id = 
cliente = "Lira Python"
Produto = "Carro"
data = "25/08/2021"
preco = "50000"
quantidade = 1
comando = f"""INSERT INTO
    Vendas(
    id_venda,
    cliente,
    produto,
    data_venda,
    preco,
    quantidade
    )
VALUES  
    ({id}, '{cliente}', '{produto}', '{data}', {preco}, {quantidade})"""
cursor.execute(comando)
cursor.comit()
