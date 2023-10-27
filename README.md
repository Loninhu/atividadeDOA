# atividadeDOA
1. A mensagem afirmando os dados que foram obtidos do servidor aparece antes da requisição dos dados ser concluída.
2. Isso ocorre por que a requisição dos dados está sendo feita de forma assíncrona, permitindo que a mensagem seja escrita
   simultâneamente enquanto os dados estão sendo requisitados.
3. Para resolver o problema, basta colocar o código que escreve a mensagem no fim da função request(), fazendo com que a
   mensagem só seja escrita apenas após os dados serem requisitados.
