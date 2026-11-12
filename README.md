# Transcritor

Transcreve reuniões **100% no seu computador**, com o Whisper rodando na GPU. Nada sai da máquina: nem o áudio, nem o
texto. Também organiza as gravações numa biblioteca, com busca em tudo o que foi dito, player sincronizado e nota de
confiança em cada trecho.

Este repositório só guarda os instaladores. Baixe a versão mais nova em
**[Releases](https://github.com/OtavioMendesSantos/transcritor-releases/releases/latest)**.

## Linux

| Arquivo | Para quem |
|---|---|
| `Transcritor_X.Y.Z_amd64.AppImage` | Qualquer distro recente (Ubuntu 22.04+, Debian 12+, Fedora 36+, Arch). Não instala nada no sistema. |
| `Transcritor_X.Y.Z_amd64.deb` | Ubuntu, Debian, Mint, Pop!_OS |
| `Transcritor-X.Y.Z-1.x86_64.rpm` | Fedora, openSUSE |

**AppImage:**

```bash
chmod +x Transcritor_*.AppImage
./Transcritor_*.AppImage
```

**.deb:** `sudo apt install ./Transcritor_*_amd64.deb` · **.rpm:** `sudo dnf install ./Transcritor-*.rpm`

Na primeira vez, o app baixa o modelo do Whisper que você escolher (o padrão tem ~550 MB). Depois disso, transcrever
não usa internet.

**GPU:** usa Vulkan, que funciona com placas NVIDIA, AMD e Intel com o driver instalado. Sem GPU, cai para a CPU (mais
lento).

## Conferir o download

Cada release tem um `SHA256SUMS`:

```bash
sha256sum -c SHA256SUMS --ignore-missing
```

## Windows e macOS

Ainda não. Estão planejados.
