# Chain 1.2.1 · Windows e Android

Windows 10/11 x64: use o instalador `.exe` e abra pelo menu Iniciar. Feche o Chain antes de atualizar; os dados de suporte são preservados. Android 7+: prefira ARM64 em aparelhos atuais, instalando o APK por cima sem desinstalar ou limpar dados.

Organize links em coleções com capas, títulos, notas, etiquetas e favoritos. Cada link tem botão de copiar, adaptado ao celular e às telas maiores. Exporte `.chain` para guardar backups com as capas. Biblioteca e exportações locais não são um cofre criptografado.

## Conectar aparelhos

1. Abra esta versão nos dois aparelhos. Para redes diferentes, use **Conexões → Configurar conexão entre redes** e informe o array ICE da sua credencial TURN em cada aparelho. Nenhuma credencial pessoal acompanha o pacote. Não use a Secret Key da conta.
2. Crie uma chave de pareamento e cole no outro aparelho. A chave vale dez minutos e é consumida no primeiro pareamento. Chaves antigas da versão 1.0 só possuem endereços locais; faça o pareamento com uma chave atual para WebRTC.
3. Depois, toque no aparelho de confiança para reconectar e use **Enviar alterações** ou **Puxar mais recentes**, sem nova chave a cada envio. Mantenha ambos os apps abertos.

WebRTC prioriza conexão direta. PeerServer Cloud negocia identificadores e informações de conexão, incluindo IPs. Um TURN configurado retransmite os pacotes criptografados se o caminho direto falhar. Esses serviços não recebem a biblioteca em texto legível nem a chave de pareamento. O Open Relay público padrão não respondeu aos testes desta rede: configure e valide um TURN próprio para contar com fallback. Disponibilidade, franquias e políticas de firewall se aplicam; nenhuma conexão é garantida em qualquer rede.

Na mesma rede, **Criar chave apenas para rede local** usa TCP 49494 sem internet. Permita rede privada no firewall do Windows se solicitado. AES-256-GCM protege os dois transportes; credenciais de confiança e TURN ficam no armazenamento seguro do aparelho. **Esquecer aparelho** revoga a confiança neste dispositivo.

Revisões divergentes geram cópias de conflito; exclusões não se propagam. Limites: 500 coleções, 20.000 links e 16 MiB por biblioteca/exportação. Guarde backups.

## Update e validação

O aviso de nova versão aparece dentro do app e abre a página oficial para download. A primeira atualização a partir de versões antigas é manual; não existe instalação automática ou notificação com o app fechado.

Análise e testes automatizados aprovados; integração Windows validou conexão direta, TURN forçado e o aviso Update. Instalador e APKs foram compilados e conferidos. Teste celular/PC nas redes reais e uso em Android físico continuam pendentes. Instalador Windows sem certificado de editor; APKs mantêm a assinatura anterior de desenvolvimento. Confira `SHA256SUMS.txt`.

## Copiar e guardar com menos passos

Em **Regras de cópia** no menu da biblioteca, configure um padrão geral ou regra por hashtag, com texto antes/depois do endereço. Exemplo: `M!play ` antes do link. A primeira regra de etiqueta ativa tem prioridade; o padrão vale para os demais. Espaços e quebras são preservados. Use o botão Copiar para o texto preparado ou **Copiar apenas endereço** para ignorar a regra. A colagem continua sendo uma ação sua no aplicativo de destino. Regras ficam neste aparelho.

No Android, escolha **Compartilhar → Guardar no Chain** no YouTube/navegador. Revise coleção existente/nova, título, trilha e etiquetas na janela rápida e confirme. Não precisa navegar pela biblioteca; não há monitoramento da área de transferência, sobreposição ou serviço permanente. No Windows, use [Chain Companion](CHAIN-COMPANION.md) para Chrome/Edge; o Setup 1.2 registra a ponte local. A abertura da janela não significa que o link já foi salvo: confirme nela.

A trilha acompanha links em exportações/transferências entre versões atualizadas. Atualize ambos os aparelhos para preservar esse campo nas edições. Salvar em uma janela não descarta inclusões de outra; editores de coleção antigos pedem reabrir antes de gravar.

Análise, 19 testes automatizados e duas integrações Windows aprovados. Ponte nativa real com validação de origem/payload e janela visível confirmada. Android físico e fluxo completo após carregar a extensão no navegador ainda precisam de validação.

## Correção 1.2.1

Corrigido o tooltip do X no aviso de atualização. Passar o mouse não causa mais erro de desenho/área branca e fechar mantém a tela/rascunho. Regressão comprovada antes/depois e integração Windows aprovadas. Instale o Setup atualizado ou o APK por cima; bibliotecas e preferências preservadas.


## Chain 1.3.0

Em Conexões, renomeie aparelhos já pareados. Em Revisar conflitos, compare as duas versões e escolha manter ambas, usar uma ou combinar links; depois use Enviar alterações. A combinação reúne exclusivos e pode recuperar links apagados só de um lado. Atualize os dois aparelhos. Exclusões não se propagam; histórico limitado a 64 revisões.

Biblioteca e aplicativo → Movimento e sons permite desativar transições e experimentar sons originais com controle de volume. Sons começam desligados, navegação/cópia têm opção adicional e não há áudio ao passar o mouse. A redução de movimento do sistema tem prioridade. Android físico e modos silencioso/Não Perturbe ainda precisam de validação.


# Chain 1.3.1

Navegação com indicador deslizante, menus com fade integral e rolagem com desaceleração curta, sem barra persistente. Redução de movimento do sistema e preferência do aplicativo preservadas. Sem alteração dos protocolos de sincronização, conflitos ou sons.

Validação: análise sem problemas, 37 testes Flutter, três integrações nativas Windows e instalação/substituição/desinstalação isoladas. APKs ARM64/ARM32/x64 conferidos: versões, certificado original e alinhamento nativo. Android físico e avaliação de FPS permanecem pendentes.

Feche o Chain e instale o Setup no mesmo local para preservar os dados. Android: instale por cima com a mesma arquitetura; não desinstale. Código-fonte privado; esta release contém somente distribuição e checksums.
