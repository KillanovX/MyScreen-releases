# MyScreen Android

Canal oficial de distribuição dos APKs do MyScreen. O código-fonte é mantido em repositório privado.

[Baixar a versão mais recente](https://github.com/KillanovX/MyScreen-releases/releases/latest/download/MyScreen-Android.apk)

Requer Android 9 ou superior. Celular e TV Android/Google TV precisam estar na mesma rede, com depuração autorizada na TV.

A partir da v0.4.1, use **Atualizar app** no próprio MyScreen. O app consulta esta distribuição, baixa a nova versão, confere integridade, pacote e assinatura, e abre a confirmação de instalação do Android. Pode ser necessário permitir atualizações desta origem nas configurações do Android.

Quem está na v0.4.0 deve instalar manualmente a versão mais recente uma vez, sem desinstalar a anterior. As versões são assinadas com o mesmo certificado de desenvolvimento. Preferências e autorização ADB são preservadas em uma atualização normal.

Cada release contém `MyScreen-Android.apk` e `update.json` (versionCode, versionName, URL HTTPS e SHA-256). Novas versões ficam disponíveis no botão após sua publicação; um commit no código-fonte não publica um APK automaticamente.

Instalação e validação física no celular serão registradas separadamente dos builds e testes locais.

## Ligar a TV pelo Wi-Fi

Desde a v0.4.2, **Ligar TV** funciona sem conexão ADB: envia Wake-on-LAN pela rede Wi-Fi e tenta reconectar. Conecte uma vez com a TV ligada para salvar o MAC automaticamente ou informe o MAC Wi-Fi em **Ligar pela rede Wi-Fi**.

Ative **Configurações → Sistema → Energia → Modo de espera → Espera em rede** na TV. Celular e TV devem estar na mesma rede. Desligamento completo pelo menu ou falta de energia impede despertar. O app só confirma ligada depois de resposta ADB/estado Awake; envio de pacote não é confirmação.

Leitura da rede/MAC na TCL real foi validada. O ciclo físico suspender/despertar e a interface no celular permanecem pendentes de teste.

## Interface v0.4.3

**Atualizar app** fica no final da aba **Recursos**, também disponível sem conexão com a TV. **Ligar TV** aparece apenas enquanto desconectado; após conectar, use o Power já existente no controle.

## Acesso rápido v0.4.4

Na aba **Apps**, toque em **Buscar apps** e marque até três estrelas. Os atalhos aparecem lado a lado abaixo do D-pad em **Controle**, com a seleção salva por endereço da TV. Desmarque uma estrela para remover ou liberar vaga. O subtítulo redundante de conexão foi removido.

## Interface v0.4.5

Removidos o título MyScreen do topo, as mensagens de sucesso dos comandos e a barra geral de ações. Erros aparecem somente quando ocorrem; download e instalação mantêm feedback em Recursos → Atualizar app. Favoritos e Power preservados.

## Logos brancas v0.4.6

A aba Apps mostra logo branca com nome e estrela. Os até três favoritos abaixo do D-pad mostram somente a logo, com nome disponível para acessibilidade. Ícones vêm dos aplicativos instalados na TV e ficam no cache local; a conversão pode simplificar detalhes. Ícone ausente ou inutilizável usa o símbolo Material Apps branco. Conectar ou Buscar apps renova o catálogo e as logos.
