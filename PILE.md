# Pile 0.1.1 — gerenciador visual de arquivos

- Galeria e lista com seleção compartilhada, busca por nomes/caminhos/etiquetas como Cute e filtros por tipo.
- Prévias de imagens com zoom, miniaturas e reprodução local de vídeos conforme os codecs do sistema.
- Navegação e criação de pastas, mover/renomear com prévia, proteção contra sobrescrita e desfazer da última operação.
- Interface mais clara, ações compactas, ícones leves e novo ícone de pastas empilhadas. IA permanece opcional e secundária.
- Figurinhas estáticas Android: preparar e revisar imagens, salvar pacotes privados e abrir a confirmação oficial no WhatsApp/Business. A aceitação final em aparelho real ainda precisa de validação. O Windows permite revisão, sem prometer importação de pacotes.
- Avisos de atualização no aplicativo e instalador Windows por usuário, com preservação das preferências.

## Instalação

Windows 10/11 x64: use Pile-0.1.1-Windows-x64-Setup.exe e abra pelo menu Iniciar. Feche a versão antiga antes de instalar. Quem usa a versão ZIP deve fazer essa primeira instalação manual.

Android 7+: escolha ARM64 (maioria dos aparelhos), ARM32 ou x64. Os APKs mantêm o certificado da versão 0.1.0: instale por cima, sem desinstalar nem limpar dados. O aviso de atualizações começa nesta versão; versões antigas precisam desta atualização manual.

## Validação e limites

32 testes automatizados e duas integrações Windows aprovados com arquivos sintéticos. Instalador testado em ambiente local isolado, inclusive preservação de arquivo extra ao desinstalar. Versões, ABIs, certificado, alinhamento e SHA-256 dos pacotes conferidos. Sem certificado de editor Windows; APKs ainda usam a assinatura de desenvolvimento preservada.

Android físico, permissões SAF e confirmação das figurinhas no WhatsApp/Business continuam pendentes. Pacotes de 3–30 imagens estáticas, até dez pacotes locais; animações/vídeos não entram no pacote estático. Não há remoção automática do fundo. Mantenha o Pile instalado. Codecs dependem do sistema.

Regras rodam sob demanda. Duplicados são comparados por conteúdo e separados sem exclusão automática. Etiquetas pertencem ao índice local e não acompanham movimentos externos. Mantenha backups. Copiar/lixeira e gestão completa de pastas ainda não estão disponíveis.

Organização e prévias são locais. O aviso Update consulta metadados do catálogo público. IA usa OpenRouter/provedor externo somente com autorização por lote e chave própria; pixels ainda podem conter dados pessoais. Figurinhas são disponibilizadas ao WhatsApp após a ação explícita de adicionar. Nenhuma conversa ou banco do WhatsApp é acessado.

Este release contém apenas binários e checksums. O repositório do código permanece privado. Confira SHA256SUMS.txt.

<!-- clustter-update-release-v1 -->
