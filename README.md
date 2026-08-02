# PATD Updates

Canal privado de atualizacoes do sistema SAP-02 PATD.

Os executaveis sao publicados somente como **GitHub Releases**. O repositorio
nao contem banco de dados, configuracoes locais, credenciais, fotos, documentos
de processos ou o codigo-fonte do sistema.

Cada versao possui:

- `PATD-Windows-vX.Y.Z.zip` — instalacao completa para Windows;
- `PATD-Windows-vX.Y.Z.zip.sha256` — hash usado antes da instalacao;
- notas da versao com as alteracoes entregues.

O PATD consulta a release mais recente, baixa o pacote autenticado, confere o
SHA-256 e chama o atualizador externo. A instalacao anterior e preservada para
rollback em caso de falha.
