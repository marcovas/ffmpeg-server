# ffmpeg-server
Tutorial de como proceder com o FFMPEG Server

#### 1.1 O Projeto FFMPEG
Seu código fonte pode ser baixado [neste site](https://ffmpeg.org/download.html). É possível encontrar versões pré-compiladas para Windows e Mac. No caso de uma distribuição Linux baseada no Debian (como Ubuntu), basta usar **apt-get install ffmpeg** na linha de comando. Compilar o projeto é algo mais avançado e não será tratado aqui.

O FFMPEG gera 3 executáveis:

* ffprobe: serve exclusivamente para analizar fluxos de mídia
* ffplay: tocador de fluxos de mídia. Depende da biblioteca [SDL](https://www.libsdl.org/)
* ffmpeg: serve como transcodificador e servidor de fluxos de mídia

Versões antigas do FFMPEG contavam com o executável **ffserver** cujas funcionalidades foram incorporadas ao **ffmpeg**

#### 1.2 Usando o ffmpeg
O **ffmpeg** o uso do ffmpeg é, teoricamente, muito simples. Basicamente:

```ps1
ffmpeg -i [fluxo de entrada] [opções de transcodificação] [fluxo de saída] 
```
