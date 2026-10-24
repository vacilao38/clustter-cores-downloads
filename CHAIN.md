# Chain 1.1.1 · Windows e Android

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
