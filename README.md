🌌 Projeto: Sistema Solar 2D Interativo com Canvas
aluno: Miguel Loureiro Aquino de Menezes
prof: Pedro Ximenes
📌 Descrição
Este projeto consiste na criação de uma cena 2D interativa utilizando HTML, JavaScript e o elemento Canvas. O objetivo é demonstrar o uso de transformações geométricas (translação, rotação e escala), conforme aprendido em aula.
O tema escolhido foi um Sistema Solar, contendo:
☀️ Sol central
🌍 Planeta orbitando o sol
🌙 Lua orbitando o planeta
🚀 Nave controlável pelo usuário
⭐ Fundo com estrelas

🎯 Objetivo
Demonstrar o domínio das transformações geométricas em 2D utilizando a API Canvas do HTML5, aplicando:
Translação
Rotação
Escala
Composição de transformações
Transformações com ponto fixo
Animação com controle de matriz

🛠️ Tecnologias Utilizadas
HTML5
JavaScript
Canvas 2D

🔄 Transformações Utilizadas
🔹 1. Translação (ctx.translate)
Utilizada para mover objetos na cena.
Exemplos:
Posicionar o sol no centro da tela
Definir a distância do planeta em relação ao sol
Movimentar a nave com o teclado

🔹 2. Rotação (ctx.rotate)
Utilizada para criar movimento circular.
Exemplos:
O planeta gira ao redor do sol (órbita)
A lua gira ao redor do planeta
A nave gira levemente ao se mover lateralmente

🔹 3. Escala (ctx.scale)
Utilizada para alterar o tamanho dos objetos.
Exemplo:
A lua é desenhada menor que o planeta utilizando escala

🔹 4. Composição de Transformações
Combinação de múltiplas transformações.
Exemplo:
Rotação + translação para simular órbita do planeta

🔹 5. Transformação com Ponto Fixo (T → R → T)
Foi utilizado o padrão:
Transladar até o ponto de referência (centro do sol)
Aplicar rotação
Transladar novamente para definir a órbita
Resultado:
O planeta gira corretamente ao redor do sol

🎬 Animação
A animação foi implementada utilizando:
requestAnimationFrame()
A cada frame:
A matriz é resetada com setTransform
A tela é limpa
Todos os objetos são redesenhados
Os ângulos de rotação são atualizados

💾 Controle de Estado
Foram utilizadas as funções:
ctx.save()
ctx.restore()
Essas funções permitem isolar transformações, evitando que um objeto afete o outro.

⭐ Funcionalidades Extras (Bônus)
🎮 Interatividade
A nave pode ser controlada com as setas do teclado


🔗 Hierarquia de Transformações
A lua depende do planeta
O planeta depende do sol
Isso cria uma estrutura hierárquica de movimentos.

🧱 Organização do Código
O código foi estruturado em funções para melhor organização:
drawSun()
drawPlanet()
drawMoon()
drawShip()
drawStars()

📷 Resultado Esperado
Sistema solar animado
Planeta orbitando o sol
Lua orbitando o planeta
Fundo com estrelas
Nave controlável pelo teclado

