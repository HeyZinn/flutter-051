App em Flutter feito para praticar os componentes de selecao do Material Design (inputs, pickers, etc).

## Resumo do Desenvolvimento

O app foi feito por etapas. Primeiro coloquei a data e hora puxando os calendarios nativos. Depois adicionei o dropdown pro tipo de evento e o slider pra controlar a quantidade de pessoas. Pra fechar, coloquei os botoes de radio pra visibilidade, os checkboxes pros servicos e os chips pra escolher as tags de comida, alem do switch pro lembrete.

### Respostas do Exercicio

**1) Qual o nome do componente Slider e sua variavel padrao?**
O componente chama Slider mesmo. A variavel que comeca com o valor padrao de 50 é a `_convidadosPadrao`.

**2) Por que usar OutlinedButton e ElevatedButton? Qual a diferenca visual e de parametros?**
Pra deixar claro o que é mais importante. O ElevatedButton tem cor de fundo e sombra (fica destacado) e serve pro "Salvar". O OutlinedButton é vazado, so tem a linha em volta e serve pro "Cancelar". O Outlined aceita o parametro `side` pra mudar a borda, e o Elevated aceita coisas de sombra como `elevation`.

**3) Qual a finalidade do método setState() dentro do RadioGroup?**
Serve pro Flutter avisar a tela que o usuario clicou em outra bolinha. Sem ele, voce clica no Radio e a bolinha marcada nao muda visualmente.

**4) Explique o ".map" no dropdown para uma crianca de 10 anos:**
Imagina que voce tem uma lista de palavras no papel. O `.map` é uma maquina magica que pega cada palavra dessa lista e transforma, uma por uma, em um balao de clicar daqueles que aparecem na tela do celular.

**5) Como é controlado as tags do tipo Chip (FilterChip)?**
Tem uma lista normal de textos chamada `_tagsSelecionadas`. Se o usuario clica no chip e ativa ele, o app da um `.add()` e poe o texto na lista. Se desclicar, da um `.remove()`. Tudo dentro do setState pra atualizar o visual na hora.
