
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
- `--input`: Caminho para o vídeo de entrada.
- `--output`: Caminho para o vídeo de saída (opcional). Se não especificado, a detecção será exibida em tempo real.
- `--filter`: Classe de objeto para filtrar as detecções (opcional).

### Exemplo

```bash
python detect_objects.py --input /caminho/para/video.mp4 --output /caminho/para/saida.mp4 --filter person
```

Este comando detectará apenas pessoas no vídeo de entrada e salvará o vídeo de saída com as detecções destacadas.

## Contribuindo

Contribuições são bem-vindas! Por favor, abra um problema ou envie uma solicitação de pull se desejar contribuir com melhorias ou correções.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
