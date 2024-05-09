# Atividade_09-05_front
Apenas para entrega solicitada.

Problema proposto foi Apesentar a maior data informada, Calcular a diferença de ambas e Apresentar o horário atual em que foi calculado.

Funções para Apresentar a Maior data
  Apenas realizei uma validação de qual seria maior e retornei no formato que queria.
  Obs: "+ 1" em Date é por causa que diminui 3 horas comparando o meridiano de Greenwich (ex: 17/11/2005 21:00:00, mas na verdade seria 18/11/2005 00:00:00)
  Obs2: "+ 1" em Month é porque começa em 0 (janeiro = 0, ...).

Funçãos para Calcular a Diferença 
  Primeiramente validei se a primeira data era mais antiga do que a segunda
  Salvei em uma constante o valor da diferença em Milessegundos por conta do formato Unix Epoch com a função Math.abs subtraindo o valor da 2 data com a 1 data
  Fui transformando em dias ( x milessegundos / 1000 (milesegundos -> segundos) * 60 (segundos -> minutos) * 60 (minutos -> hora) * 24 (horas -> 1 dia))
  Tranforamndo em meses ( x dias / 30 ) -> generalizei 
  Transformando em anos (x meses / 12 ) 
  Retornei os valores obtidos.
  Obs: Math.floor arredonda para menor.

Função para Apresenar o horário Atual
  Constante Hora = getHours (Pegar as horas), toString (Transforma em String), padStart(2, '0') (Adiciona 0 a esquerda se necessário).
  Constante Minutos = getMinutes (Pegar os minutos), toString (Transforma em String), padStart(2, '0') (Adiciona 0 a esquerda se necessário).
  Constante Dia = getDate (Pegar o dia), toString (Transforma em String), padStart(2, '0') (Adiciona 0 a esquerda se necessário).
  Constante Dia = getDate (Pegar o dia), toString (Transforma em String), padStart(2, '0') (Adiciona 0 a esquerda se necessário).
  Constante Dia = getFullYear (Pegar o ano), toString (Transforma em String)).

Por Fim, fiz um innerHTML com o id da Div para passar os calculos realizados em JS apresentando na página HTML.
