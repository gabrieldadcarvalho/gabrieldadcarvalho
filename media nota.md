nome = str(input('Nome do aluno: ')).capitalize()
nota1 = float(input('Qual a 1º nota: '))
nota2 = float(input('Qual a 2º nota: '))
media = (nota1 + nota2) / 2
if media >= 7:
    situacao = "\33[1;32mAPROVADO\033[m"
else:
    situacao = "\033[1;31mREPROVADO\033[m"
print("=-" * 23)


def tabela():
    print("Nome do aluno\t\tMédia\t\tSituação")
    print('-' * 46)
    print('%s:\t\t\t%.2f\t\t%s' % (nome, media, situacao))
    print('-' * 46)


tabela()
