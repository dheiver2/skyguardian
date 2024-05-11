
# Detecção de Objetos em Vídeos com YOLO-NAS-L

Este é um projeto de detecção de objetos em vídeos usando o modelo YOLO-NAS-L. O YOLO-NAS-L é um modelo de detecção de objetos eficiente e preciso, adequado para aplicações em tempo real.

## Como Usar

### Requisitos

- Python 3
- OpenCV (cv2)
- NumPy

### Instalação

1. Clone este repositório:

    ```bash
    git clone https://github.com/seu-usuario/detecao-objetos-video-yolo-nas-l.git
    cd detecao-objetos-video-yolo-nas-l
    ```

2. Instale as dependências:

    ```bash
    pip install -r requirements.txt
    ```

### Uso

Para executar a detecção de objetos em um vídeo, execute o seguinte comando:

```bash
python detect_objects.py --input /caminho/para/video.mp4 --output /caminho/para/saida.mp4 --filter classe
```

Argumentos:
- `--input`: Caminho para o vídeo de entrada. Pode ser um arquivo local ou uma URL de vídeo.
- `--output`: Caminho para o vídeo de saída (opcional). Se não especificado, a detecção será exibida em tempo real.
- `--filter`: Classe de objeto para filtrar as detecções (opcional).

### Exemplos

1. Executar detecção em um arquivo de vídeo local:

    ```bash
    python detect_objects.py --input video.mp4 --output saida.mp4 --filter person
    ```

2. Executar detecção em um vídeo online (URL):

    ```bash
    python detect_objects.py --input https://example.com/video.mp4 --output saida.mp4 --filter car
    ```

3. Executar detecção em tempo real sem salvar o vídeo de saída:

    ```bash
    python detect_objects.py --input 0 --filter dog
    ```

Este comando detectará apenas cachorros em uma entrada de vídeo da webcam e exibirá a detecção em tempo real.

## Contribuindo

Contribuições são bem-vindas! Por favor, abra um problema ou envie uma solicitação de pull se desejar contribuir com melhorias ou correções.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
