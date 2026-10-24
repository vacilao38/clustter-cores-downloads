# Pile 0.1.0

Organização local de arquivos para Windows 10/11 x64 e Android 7+ (celular e tablet).

- Categorias e pastas customizáveis, prévia e opção de organizar em um clique.
- Coleções, etiquetas, capas, temas e leitura local de EXIF por ano/coordenadas.
- Regras opcionais executadas sob demanda, sem monitoramento em segundo plano.
- Duplicados por SHA-256 separados das imagens visualmente parecidas. Cópias podem ir para revisão; nada é apagado automaticamente.
- Histórico para desfazer a última operação, sem sobrescrita.
- IA opcional via OpenRouter: chave própria e autorização por lote de imagens. Miniaturas sem EXIF, revisão das sugestões antes de aplicar. O conteúdo visual ainda pode conter dados pessoais; políticas de terceiros e cotas se aplicam.

## Instalar

Windows: baixe o ZIP, extraia a pasta completa e abra pile.exe. Mantenha DLLs e data juntos. Runtimes C++ acompanham o pacote.
Android: ARM64 é recomendado para a maioria dos aparelhos atuais; ARM32 para dispositivos antigos compatíveis e x64 para essa arquitetura. APKs usam assinatura de desenvolvimento nesta versão inicial; instalação direta, sem Play Store.

## Validação e limites

Análise estática sem problemas, 27 testes de domínio/IO/widgets aprovados e 1 teste de integração Windows aprovado para organizar e desfazer pela interface. Layouts verificados em celular, tablet e desktop com texto ampliado. Builds Windows e Android compilados.

Uso em Android físico e chamadas reais de IA ainda precisam de validação. O seletor Android pode bloquear a raiz de Downloads e Android/data; escolha uma subpasta local. Etiquetas ficam no índice do Pile e não acompanham movimentos externos. Desfazer não substitui backup.

SHA256SUMS.txt permite conferir a integridade dos quatro pacotes. Não há telemetria ou backend do Pile. O código-fonte permanece em repositório privado por decisão do proprietário.
