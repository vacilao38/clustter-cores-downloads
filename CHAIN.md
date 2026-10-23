# Chain 1.0 · Windows

Windows 10/11 x64. Extraia a pasta inteira do ZIP e abra **chain.exe**. As DLLs, o runtime C++ e a pasta `data` precisam permanecer junto do executável. Não é necessário instalar o Flutter.

Crie uma coleção, escolha um nome, categoria e capa e adicione seus links. Títulos, notas, etiquetas, favoritos e ordem são editáveis. Ctrl+N cria coleção; Ctrl+F busca.

As coleções são salvas no diretório de suporte da aplicação, no perfil do Windows. Exporte `.chain` pelo menu para guardar um backup com as capas. Importar um arquivo cria cópias. Exportações não possuem senha; guarde-as onde considerar apropriado.

## Conectar seus aparelhos

1. Abra o Chain nos dois aparelhos na mesma rede Wi-Fi ou hotspot.
2. Em Conexões, crie uma chave e copie-a para o campo de pareamento do outro aparelho.
3. O convite vale dez minutos e é consumido no primeiro pareamento. Os aparelhos passam a lembrar um ao outro.
4. Depois, toque no aparelho lembrado para reconectar e use **Enviar alterações** ou **Puxar mais recentes**. A conexão ativa permite vários envios sem outra chave.

Se o firewall do Windows solicitar, permita acesso à rede privada. O canal usa TCP 49494. Os próprios aparelhos trocam os dados; não há servidor intermediário nem necessidade de internet na mesma rede. Mantenha o Chain aberto nos dois lados. Se o IP mudar, atualize o endereço nas opções do aparelho lembrado.

Para redes diferentes, um endereço precisa ser acessível diretamente por IPv6 público ou por redirecionamento de porta no roteador. CGNAT e firewalls podem impedir esse acesso. Não há travessia automática de NAT.

As mensagens são autenticadas e criptografadas com AES-256-GCM. As credenciais lembradas ficam no armazenamento seguro do sistema. **Esquecer aparelho** revoga a confiança neste dispositivo.

## Preservar seu trabalho

As versões são comparadas pelo histórico de revisões. Alterações divergentes geram uma cópia **· conflito**; exclusões não se propagam. Enviar/puxar não apaga silenciosamente sua versão local.

Limites: 500 coleções, 20.000 links e 16 MiB por biblioteca/exportação. Capas são reduzidas para até 960 px por eixo. O aplicativo não é um cofre criptografado para arquivos locais.

O pacote foi compilado e sua inicialização foi verificada no Windows. A troca entre aparelhos físicos e os seletores Android ainda precisam de validação em hardware. Licenças dos componentes acompanham a pasta `licenses` e a tela **Sobre o Chain → Ver licenças**.
