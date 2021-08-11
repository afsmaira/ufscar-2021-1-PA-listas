# CIgrader-professor
Corretor automático para laboratório de ensino baseado em CI

O corretor ficará público e o CI no repositório do aluno baixará a cada correção que for fazer, portanto se precisar esconder o corretor, compile o mesmo. Uma possibilidade para python é usando:

```bash
pyinstaller --onefile arquivo.py
```

Cada pasta do repositorio e referente a uma lista/trabalho, a pasta do aluno deve ter o mesmo nome para que o corretor seja executado. Se houver um arquivo chamado `due_to.txt` na pasta com um `datetime` no formato `YYYY-mm-ddTHH:MM:SS` o trabalho somente sera corrigido se entregue antes desse horario (esse controle pode tambem ser feito pelo corretor) 