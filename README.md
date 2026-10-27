# Clustter cores — Downloads

## Bridge 0.1.0 · 27/10/2026

[Bridge](BRIDGE.md): teclado e mouse do Windows no Android por conexão direta na rede local. [Download na Clustter](https://vacilao38.github.io/clustter-cores-downloads/#bridge). Setup Windows e APKs ARM64, ARM32 e x64 com hashes verificados. Acessibilidade e Teclado Bridge são ativados manualmente. Gestos, IME e segundo plano ainda precisam de ensaio em Android físico. Código-fonte privado por pedido explícito do usuário; publicação dos binários autorizada no mesmo pedido.

Canal público de distribuição dos aplicativos selecionados de Folk, Lake, Chain, Noon e Pile. O site é [Clustter cores](https://vacilao38.github.io/clustter-cores-downloads/).

Versões atuais: **Folk 1.0.1 · Lake 1.2.1 · Chain 1.3.1 · Noon 0.1.1 · Pile 0.3.0**. Cada release inclui instalador Windows x64 `.exe`, APKs Android ARM64/ARM32/x64 e `SHA256SUMS.txt`. Builds e downloads antigos continuam no histórico.

O instalador Windows é por usuário, cria atalho no menu Iniciar e preserva projetos/preferências ao atualizar. Feche o aplicativo antes de instalar no mesmo local. Usuários de ZIP fazem esta primeira instalação manual. No Android, instale por cima sem desinstalar nem limpar dados: os APKs mantêm o certificado anterior de desenvolvimento. Android físico permanece pendente de validação.

O protocolo **Update** avisa dentro do app sobre uma versão superior publicada e abre a página oficial para baixar. Não instala automaticamente nem avisa com o app fechado. Apps anteriores ao protocolo precisam desta primeira atualização manual. O feed `docs/updates.json` contém apenas metadados públicos e não recebe projetos, arquivos ou identificadores de aparelho.

`docs/catalog.json` e o feed são gerados pelo repositório de código do site; não anunciar versões antes de publicar/verificar os pacotes. Este repositório de distribuição não inclui código privado, bibliotecas de uso ou credenciais. Folk, Lake, Chain e Pile mantêm fontes privadas; Noon e o componente genérico Update são públicos.

- Folk: transcrição offline com modelos incluídos, Windows x64 com AVX2; mantenha aberto durante o processamento.
- Lake: animação vetorial e exportação PNG/SVG; ainda sem MP4/GIF.
- [Chain](CHAIN.md): coleções de links, copiar com um toque e P2P criptografado entre aparelhos, com negociação WebRTC e TURN configurável entre redes.
- Noon: síntese, até oito camadas e 60 segundos, WAV/.noon e script para LLM externa; sem samples/MIDI/VST ou motor em tempo real.
- [Pile](PILE.md): gerenciador visual, prévias e organização local; confira os limites de Android, IA e figurinhas no guia.

Licenças e avisos acompanham os aplicativos. Consulte os requisitos e limites na apresentação de cada produto antes de baixar.

## Chain Companion 1.0.0

Extensão de captura para Chrome/Edge no Windows, distribuída em ZIP para carregar sem compactação. Requer Chain 1.2.0 instalado pelo Setup. Uma janela rápida revisa coleção, título, trilha e etiquetas antes de salvar. Não está publicada em lojas de extensão. [Instalação e limites](CHAIN-COMPANION.md).

Chain 1.2 também inclui regras de cópia com texto antes/depois, padrão ou por hashtag, e compartilhamento Android em janela própria. Validação em Android físico e fluxo completo com a extensão carregada nos navegadores permanecem pendentes.

Chain 1.2.1 corrige o erro de desenho ao passar o mouse no X do aviso de atualização; fechar o aviso preserva a tela em uso. Companion 1.0.0 continua compatível.

Chain 1.3.0: apelidos de aparelhos, comparação/resolução de conflitos, transições com redução de movimento e sons opcionais. Pacotes Windows/Android e feed atualizados; Companion 1.0.0 preservado.

Atualizações de 25/10/2026: Pile 0.3.0 e Chain 1.3.1, com pacotes verificados e fonte privada. Outros produtos preservados. Android físico continua pendente conforme as apresentações.
