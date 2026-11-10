# Rosekiwi — Downloads

Instaladores oficiais do **Rosekiwi**, o navegador com um agente que lê, preenche e executa
tarefas na web com aprovação nos passos que importam.

Este repositório existe só para hospedar os binários: o código-fonte fica em
[`DominykASI/rosekiwi`](https://github.com/DominykASI/rosekiwi).

## Baixar

Todos os arquivos estão na página de releases:

**https://github.com/DominykASI/rosekiwi-installers/releases/latest**

| Sistema | Arquivo | Como usar |
|---|---|---|
| Windows 10/11 (x64) | `Rosekiwi-0.2.0-Windows-Setup.exe` | Instalador. Instala por usuário e cria atalho. |
| Windows 10/11 (x64) | `Rosekiwi-0.2.0-Windows.exe` | Portátil. Rode direto, sem instalar. |
| Linux (x64) | `Rosekiwi-0.2.0-Linux.AppImage` | Portátil: `chmod +x` e execute. |
| Linux — Debian/Ubuntu/Lubuntu | `Rosekiwi-0.2.0-Linux.deb` | `sudo apt install ./Rosekiwi-0.2.0-Linux.deb` |
| Linux — Fedora/openSUSE | `Rosekiwi-0.2.0-Linux.rpm` | `sudo dnf install ./Rosekiwi-0.2.0-Linux.rpm` |
| macOS | — | Em preparo (late). |

Links diretos do `latest`:

```
https://github.com/DominykASI/rosekiwi-installers/releases/latest/download/Rosekiwi-0.2.0-Windows-Setup.exe
https://github.com/DominykASI/rosekiwi-installers/releases/latest/download/Rosekiwi-0.2.0-Windows.exe
https://github.com/DominykASI/rosekiwi-installers/releases/latest/download/Rosekiwi-0.2.0-Linux.AppImage
https://github.com/DominykASI/rosekiwi-installers/releases/latest/download/Rosekiwi-0.2.0-Linux.deb
https://github.com/DominykASI/rosekiwi-installers/releases/latest/download/Rosekiwi-0.2.0-Linux.rpm
```

## Antes de instalar

- **Sem assinatura de código.** No Windows o SmartScreen vai avisar ("Mais informações" →
  "Executar assim mesmo"). No macOS, um `.dmg` não notarizado exige liberar em
  Ajustes → Privacidade e Segurança.
- **Windows:** o SmartScreen também pode marcar o portátil como desconhecido.
- **Linux:** o AppImage precisa de `chmod +x`; o `.deb`/`.rpm` avisam sobre pacote não
  assinado.
- Verifique o `.sha256` de cada arquivo antes de executar, se quiser conferir a integridade.

## Verificar integridade

Cada release inclui um arquivo `SHA256SUMS.txt`. Para conferir:

```bash
# Linux / macOS
sha256sum -c SHA256SUMS.txt

# PowerShell
Get-FileHash .\Rosekiwi-0.2.0-Windows-Setup.exe -Algorithm SHA256
```

## macOS

Ainda **não** há binário do macOS. O `.dmg` universal existe no CI do repositório de
código, mas depende de notarização (conta Apple Developer) para abrir sem aviso. Enquanto
isso, use Windows ou Linux.

## Licença

O Rosekiwi é distribuído sob **AGPL-3.0-or-later**. Este repositório contém apenas
binários compilados; o código-fonte e a licença completa estão em
[`DominykASI/rosekiwi`](https://github.com/DominykASI/rosekiwi).
