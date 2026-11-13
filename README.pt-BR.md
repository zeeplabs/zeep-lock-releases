<div align="center">

# Zeep Lock

**Um gerenciador de senhas gratuito e simples para Mac — com um cofre separado para cada parte da sua vida.**

**🇧🇷 Português** · [English](README.md)

[**⬇️ Baixar a versão mais recente**](../../releases/latest)

</div>

<!-- Capturas de tela: coloque as imagens em uma pasta `screenshots/` e referencie aqui, por exemplo:
![Zeep Lock](screenshots/janela-principal.png)
-->

## O que é o Zeep Lock?

A maioria dos gerenciadores de senhas joga tudo no mesmo lugar. O **Zeep Lock mantém separado o que não deve se misturar**: as senhas da empresa em um cofre, as pessoais em outro, um projeto de cliente em um terceiro. Cada cofre é independente, e você cria quantos precisar.

É **gratuito**, funciona **localmente no seu Mac** e **não tem servidores próprios**.

## Recursos

- 🗂️ **Cofres** — separe as senhas da empresa, as pessoais e as de projetos.
- 🔑 **Credenciais** — título, usuário, URL, senha, notas e tags; favoritos e busca por título e URL.
- 🎲 **Gerador de senhas** — escolha o tamanho e os tipos de caractere, e veja a força de cada senha.
- 🛡️ **Auditoria de segurança** — encontre senhas fracas.
- 📥 **Importar e exportar** — importe um arquivo CSV ou JSON exportado de outro gerenciador, e exporte um backup **criptografado** protegido por uma senha que você escolhe.
- 👆 **Touch ID** — opcional, para desbloquear sem digitar a senha mestra.
- ⏱️ **Bloqueio automático** — por inatividade e sempre que o Mac dorme, a tela é bloqueada ou o protetor de tela começa.
- 📋 **Cuidado com a área de transferência** — as senhas copiadas são apagadas depois de um tempo e não vão para o Universal Clipboard.
- ☁️ **Sincronização com o iCloud (beta, opcional)** — veja abaixo.

## Segurança

- Seus dados são **criptografados no seu Mac**. Senhas, usuários, notas, títulos, URLs, tags e nomes de cofres são todos criptografados, não só a senha.
- Uma chave aleatória de 256 bits criptografa os seus dados (AES-GCM). Essa chave é protegida por outra, derivada da sua **senha mestra** (PBKDF2-HMAC-SHA256, 600.000 iterações).
- **A senha mestra não pode ser recuperada.** Se você a esquecer, a única saída é apagar os dados daquele Mac e recomeçar. Guarde-a em um lugar seguro.
- O Zeep Lock **não tem conta nem servidor**. Nada é enviado para a Zeep Labs.

> O Zeep Lock ainda não passou por uma auditoria de segurança independente. Considere isso e mantenha um backup criptografado do que importa.

## Sincronização com o iCloud (beta)

A sincronização é **opcional e vem desligada**. Quando você a liga, ela mantém os seus cofres do iCloud sincronizados entre os seus Macs, pela **sua própria conta do iCloud**, com os dados já criptografados. Um cofre também pode ficar só neste Mac.

É um **beta**: ainda não foi validada com vários Macs. Mantenha um backup criptografado (Ajustes ▸ Import & Export) e não trate a sincronização como a sua única cópia.

## Download e instalação

1. Abra [**Releases**](../../releases/latest) e baixe o arquivo `.dmg`.
2. Abra-o e **arraste o Zeep Lock para Aplicativos**.
3. Abra o Zeep Lock pelo Launchpad ou pelo Spotlight e crie a sua senha mestra.

O app é **assinado e notarizado pela Apple**. O `SHA-256` de cada arquivo está nas notas da versão, se você quiser conferir o seu download.

**Requisitos:** macOS 26.5 ou superior.

## Atualizações

O Zeep Lock **se atualiza sozinho**: quando há uma versão nova, ele avisa e você escolhe se quer instalar. Para isso, o app consulta o feed de atualização deste projeto uma vez por dia, o que revela o seu endereço IP e a versão do app para quem hospeda (o GitHub). Nada além disso é enviado. Cada atualização é verificada com uma assinatura criptográfica antes de ser instalada.

## Perguntas frequentes

**Esqueci a senha mestra. Vocês conseguem recuperar as minhas senhas?**
Não. Não há recuperação, por projeto: ninguém além de você consegue ler os seus dados. Na tela de bloqueio, "Forgot your master password?" permite apagar os dados daquele Mac e começar de novo. Se você guardou uma exportação criptografada, pode importá-la depois.

**Onde as minhas senhas ficam guardadas?**
No seu Mac, criptografadas. Se você ligar a sincronização com o iCloud, uma cópia criptografada também fica na sua própria conta do iCloud.

**É gratuito mesmo?**
Sim.

**Funciona no iPhone ou no Windows?**
Por enquanto não. O Zeep Lock é um app para Mac.

## Feedback e bugs

Abra uma [issue](../../issues) neste repositório. **Nunca inclua senhas, a sua senha mestra ou arquivos de backup** em uma issue.

## Sobre

Este repositório contém apenas as versões publicadas e o feed de atualização. O código-fonte não é público.

© Zeep Tecnologia. Todos os direitos reservados. Feito pela [Zeep Labs](https://github.com/zeeplabs).
