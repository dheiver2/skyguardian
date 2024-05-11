

# Object Detector

Este é um detector de objetos que utiliza o modelo YOLO-NAS-L para detectar objetos em imagens ou vídeos. Ele suporta várias fontes de entrada, incluindo webcam, arquivos de vídeo locais e URLs de vídeo online.

## Instalação

Para executar este detector de objetos, é necessário ter o Python e algumas bibliotecas instaladas. Você pode instalar as dependências executando o seguinte comando:

```bash
pip install opencv-python numpy urllib3 super_gradients
```

## Uso

Você pode usar este detector de objetos executando o script `object_detector.py`. Aqui estão alguns exemplos de como usar o detector com diferentes fontes de entrada:

### Exemplo 1: Usando uma webcam

```bash
python object_detector.py --source webcam
```

Isso iniciará o detector de objetos usando a webcam do seu computador como fonte de entrada.

### Exemplo 2: Usando um arquivo de vídeo local

```bash
python object_detector.py --source video --input_path /path/to/your/video.mp4
```

Isso iniciará o detector de objetos usando um arquivo de vídeo local como fonte de entrada.

### Exemplo 3: Usando uma URL de vídeo online

```bash
python object_detector.py --source video --input_url https://example.com/your/video.mp4
```

Isso iniciará o detector de objetos usando uma URL de vídeo online como fonte de entrada.

### Exemplo 4: Salvando o vídeo de saída

```bash
python object_detector.py --source webcam --output_path output.mp4
```

Isso iniciará o detector de objetos usando a webcam e salvará o vídeo de saída como `output.mp4`.

### Exemplo 5: Definindo um limite de confiança

```bash
python object_detector.py --source video --input_path /path/to/your/video.mp4 --confidence_threshold 0.5
```

Isso iniciará o detector de objetos usando um arquivo de vídeo local como fonte de entrada e definirá o limite de confiança para 0.5.

### Exemplo 6: Filtrando objetos por label

```bash
python object_detector.py --source video --input_path /path/to/your/video.mp4 --filter_label person
```

Isso iniciará o detector de objetos usando um arquivo de vídeo local como fonte de entrada e filtrará apenas os objetos da classe "person".

Você pode combinar várias opções para personalizar o comportamento do detector de objetos de acordo com suas necessidades.

