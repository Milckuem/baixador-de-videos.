# baixador-de-videos.
Ferramenta de linha de comando desenvolvida em Python para baixar vídeos e áudios de diferentes plataformas da internet utilizando a biblioteca yt-dlp. Oferece seleção de qualidade, extração de áudio em MP3, download de playlists, legendas, suporte a cookies do navegador e acompanhamento do progresso dos downloads.

yt-dlp

# Baixador de Vídeos

Script em Python que baixa vídeos de diversos sites usando yt-dlp.

## Instalação
pip install -r requirements.txt
(instale também o ffmpeg)

## Uso
python baixar_video.py "URL" -q 720

## Caso queira apenas o audio
python baixar_video.py "https://site.com/pagina-do-video" --audio
##em https colocar o link do site para downlaod pode ser o youtube.

## Aviso
Use apenas para conteúdo que você tem direito de baixar e respeite os termos de uso dos sites.
