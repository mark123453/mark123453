import os

pasta = r'C:\Users\USUARIO\Desktop\pasta'

prefixo = 'backup.txt'
for nome_arquivo in os.listdir(pasta):
    
    caminho_antigo = os.path.join(pasta, nome_arquivo)
    novo_nome = prefixo + nome_arquivo
    caminho_novo = os.path.join(pasta, novo_nome)
    
    os.rename(caminho_antigo, caminho_novo)

print("Arquivos renomeados com sucesso!")
