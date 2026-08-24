# PATD Updates

Canal publico de atualizacoes do sistema SAP-02 PATD para Windows e Linux Mint.

Os executaveis sao publicados somente como **GitHub Releases**. O repositorio
nao contem banco de dados, configuracoes locais, credenciais, fotos, documentos
de processos ou o codigo-fonte do sistema.

Cada versao possui:

- `PATD-Windows-vX.Y.Z.zip` — instalacao completa para Windows;
- `PATD-Windows-vX.Y.Z.zip.sha256` — hash usado antes da instalacao;
- `PATD-LinuxMint-vX.Y.Z.zip` — pacote usado pelo atualizador no Linux Mint;
- `PATD-LinuxMint-vX.Y.Z.zip.sha256` — hash do pacote Linux;
- `SISPatd-LinuxMint-x86_64` — binario portatil para a primeira instalacao no Linux Mint;
- notas da versao com as alteracoes entregues.

O PATD identifica o sistema operacional, consulta a release mais recente, baixa
somente o pacote correspondente e confere o SHA-256. O atualizador e incorporado
ao proprio programa nos dois sistemas. A instalacao anterior e preservada para
rollback em caso de falha.

## Instalar no Linux Mint

Baixe o binario da release mais recente e execute:

```bash
chmod +x SISPatd-LinuxMint-x86_64
./SISPatd-LinuxMint-x86_64
```

No primeiro uso ele se instala em `~/.local/opt/SISPatd`, cria o atalho e abre o
sistema. As atualizacoes seguintes sao feitas em **CONFIGURACOES > ATUALIZACOES**.
