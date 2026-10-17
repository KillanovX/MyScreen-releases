# MyScreen Android

Canal oficial de distribuição dos APKs do MyScreen. O código-fonte é mantido em repositório privado.

[Baixar a versão mais recente](https://github.com/KillanovX/MyScreen-releases/releases/latest/download/MyScreen-Android.apk)

Requer Android 9 ou superior. Celular e TV Android/Google TV precisam estar na mesma rede, com depuração autorizada na TV.

A partir da v0.4.1, use **Atualizar app** no próprio MyScreen. O app consulta esta distribuição, baixa a nova versão, confere integridade, pacote e assinatura, e abre a confirmação de instalação do Android. Pode ser necessário permitir atualizações desta origem nas configurações do Android.

Quem está na v0.4.0 deve instalar manualmente a v0.4.1 uma vez, sem desinstalar a anterior. As versões são assinadas com o mesmo certificado de desenvolvimento. Preferências e autorização ADB são preservadas em uma atualização normal.

Cada release contém `MyScreen-Android.apk` e `update.json` (versionCode, versionName, URL HTTPS e SHA-256). Novas versões ficam disponíveis no botão após sua publicação; um commit no código-fonte não publica um APK automaticamente.

Instalação e validação física no celular serão registradas separadamente dos builds e testes locais.
