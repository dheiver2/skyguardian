
# Detecção de Objetos em Vídeo

Este projeto implementa um sistema de detecção de objetos em vídeos utilizando a rede neural YOLO-NAS-L e OpenCV.

## Funcionalidades

- Detecta objetos em vídeos.
- Suporta diferentes tipos de entrada: imagem, vídeo e link de streaming.
- Salva um novo vídeo com as previsões desenhadas.
- Registra todas as previsões em um arquivo de log.

## Instalação

1. Clone o repositório:

    ```
    git clone https://github.com/seu_usuario/nome_do_repositorio.git
    ```

2. Instale as dependências:

    ```
    pip install -r requirements.txt
    ```

## Utilização

1. Execute o script `object_detection.py` passando o caminho do vídeo de entrada como argumento:

    ```
    python object_detection.py /caminho/do/video.mp4
    ```

2. O vídeo resultante com as previsões será salvo no diretório de trabalho como `output_video.mp4`.
3. O arquivo de log com todas as previsões será salvo como `predictions_log.txt`.

## Requisitos

- Python 3
- OpenCV
- Super Gradients

## Licença

Este projeto é distribuído sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.
