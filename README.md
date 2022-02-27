# WSL2 TIPS

Algumas dicas para melhor utilização do WSL2
## Tips

- O arquivos (Disk C) do Windows estão disponiveis em /mnt

- Para executar o WSL2 a partir de qualquer Terminal CMD/PowerShell basta digitar 
```bash
  wsl 
  ou 
  C:\Windows\System32\wsl.exe
```

- Para acessar o arquivos do WSL2 pelo Windows Explorer, digite:
```bash
  \\wsl$
```

- Verificar as versões de Linux instaladas e seu status (parado ou rodando).
```bash
  wsl -l -v
```

- Desligar todos as distribuições Linux do WSL2
```bash
  wsl --shutdown
```

- Desligar uma distruibição específica
```bash
  wsl --t <distribution name>
```
## Observação Importante

- O desempenho do WSL 2 é voltado a tudo que está rodando dentro do LINUX, devido a isso é EXTREMAMENTE recomendavel executar os projetos dentro dos diretórios LINUX, ou seja NÃO É recomendavel executar projetos no caminho /mnt/c, pois assim haverá perda de desempenho no WSL2.
