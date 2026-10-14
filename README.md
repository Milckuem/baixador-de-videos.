# Baixador de Vídeos

Script em Python para baixar vídeos de páginas da web, baseado no [yt-dlp](https://github.com/yt-dlp/yt-dlp).
Funciona com YouTube, Vimeo, Instagram, TikTok, X/Twitter, Facebook, Reddit e mais de 1000 sites,
além de páginas comuns com vídeo embutido.

## Requisitos

- Python 3.8 ou superior
- [ffmpeg](https://ffmpeg.org/) (para juntar vídeo + áudio e converter para MP3)

## Instalação

```bash
git clone https://github.com/SEU-USUARIO/baixador-de-videos.git
cd baixador-de-videos
pip install -r requirements.txt
```

Instalando o ffmpeg:

| Sistema | Comando |
|---------|---------|
| Windows | `winget install ffmpeg` |
| macOS   | `brew install ffmpeg` |
| Linux   | `sudo apt install ffmpeg` |

## Uso

```bash
python baixar_video.py "https://site.com/pagina-do-video"
```

| Opção | Descrição |
|-------|-----------|
| `-o`, `--saida` | Pasta de destino (padrão: `./downloads`) |
| `-q`, `--qualidade` | Altura máxima em pixels (ex.: 480, 720, 1080) |
| `-a`, `--audio` | Baixar somente o áudio em MP3 |
| `-p`, `--playlist` | Baixar a playlist inteira |
| `-l`, `--legendas` | Baixar legendas (pt/en), quando disponíveis |
| `--cookies-do-navegador` | Usar cookies do navegador (chrome, firefox, edge...) |
| `--cookies-arquivo` | Arquivo de cookies no formato Netscape |

### Exemplos

```bash
python baixar_video.py URL -q 720
python baixar_video.py URL --audio
python baixar_video.py URL -p -o ~/Videos
python baixar_video.py URL1 URL2 URL3
```

## Limitações

- Vídeos protegidos por DRM (Netflix, Disney+, Prime Video etc.) não são suportados.
- Sites mudam com frequência. Se der erro, atualize: `pip install -U yt-dlp`.

## Aviso legal

Use esta ferramenta apenas para conteúdo que você tem o direito de baixar
(seu próprio conteúdo, domínio público, licenças livres ou com permissão do autor).
Respeite os Termos de Uso dos sites e as leis de direitos autorais do seu país.
Os autores não se responsabilizam pelo uso indevido.

## Licença

MIT. Veja o arquivo [LICENSE](LICENSE).
