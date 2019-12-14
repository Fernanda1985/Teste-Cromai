# Teste-Cromai
Teste case_Embarcados
#1. Escreva um modelo conceitual dos dois códigos, por exemplo um diagrama ou
#um pseudocódigo.
#2. Escreva o código de script shell.-(Não foi realizado porque não possuo conhecimento de Linux e a minha
# maquina não possui memoria suficiente para armazenamento)
#3. Escreva o código em python3.-(Foi realizado)
#4. Faça a integração dos dois.-(Não foi realizado)
#5. Descreva quais são as diferenças entre o modelo conceitual descrito por você e o que foi implementado.
#
#6. Suba seu código no github e nos envie o link.

# foi importado algumas bibliotecas 

import schedule # roda o programa em um tempo determinado
import time     # modulo de tempo
import os       # modulo que traz informações sobre o sistema operacional(ID)

print (os.getpid()) #retornar o número do pid(ID)

arquivo=open('9008','a')
texto="""
for c in rangel(0,3):
	print('2:I am alive')
print('2:I gonna die now, bye')
"""

#schedule.cada.tempo.fazer
schedule.every(2).seconds.do(texto)

while 2:
	schedule.run_pending()
	time.sleep(2)

arquivo.write('9008')
arquivo.close()
