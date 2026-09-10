# NOT Block
Puzzle de blocos para lives. Complete linhas/colunas para limpar o tabuleiro e criar combos.

## Interações do Conector / Projeto Daniel
- `random_block`: adiciona 1..20 células aleatórias livres.
- `swap_tray`: troca as três peças disponíveis sem aviso no gameplay.
- `fake_block`: camufla 1..3 peças. `duration=0` mantém a camuflagem até a peça ser jogada; valor >0 revela após N segundos. A colisão/encaixe sempre usa a forma real, portanto a peça falsa não ganha encaixe impossível.
- `live_restart`: reinicia.

## Combo
Uma linha/coluna completa vale 100 pontos. Limpar múltiplas no mesmo lance adiciona bônus progressivo e efeito visual leve via CSS, sem partículas pesadas.

A arquitetura segue o padrão modular usado em Frutas: game runtime, ações de live e bridge do painel separados.