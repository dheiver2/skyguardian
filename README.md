
# Object Detector

O Object Detector é uma ferramenta poderosa que utiliza o modelo YOLO-NAS-L para detectar objetos em imagens ou vídeos. Este detector suporta várias fontes de entrada, incluindo webcam, arquivos de vídeo locais e URLs de vídeo online. Ele fornece uma maneira simples e eficaz de identificar e rastrear objetos em tempo real ou em vídeos gravados.

## Instalação

Antes de usar o Object Detector, é necessário instalar algumas dependências. Certifique-se de ter o Python instalado em seu sistema e execute o seguinte comando para instalar as bibliotecas necessárias:

```bash
pip install opencv-python numpy urllib3 super_gradients
```

## Uso

O Object Detector pode ser usado de várias maneiras, dependendo da fonte de entrada e das configurações desejadas. Aqui estão alguns exemplos de como usar o detector:

### Utilizando uma Webcam

```bash
python object_detector.py --source webcam
```

Este comando iniciará o detector de objetos usando a webcam do seu computador como fonte de entrada. Você verá uma janela mostrando a saída do detector em tempo real.

### Utilizando um Arquivo de Vídeo Local

```bash
python object_detector.py --source video --input_path /path/to/your/video.mp4
```

Este comando iniciará o detector de objetos usando um arquivo de vídeo local como fonte de entrada. Ele detectará objetos no vídeo e exibirá a saída ou salvará o vídeo processado, se desejado.

### Utilizando uma URL de Vídeo Online

```bash
python object_detector.py --source video --input_url https://example.com/your/video.mp4
```

Este comando iniciará o detector de objetos usando uma URL de vídeo online como fonte de entrada. Ele baixará o vídeo da URL especificada e executará a detecção de objetos.

### Personalizando as Configurações

Você pode personalizar várias configurações do detector de objetos, incluindo o limite de confiança para detecção de objetos e a filtragem por label. Aqui está um exemplo:

```bash
python object_detector.py --source video --input_path /path/to/your/video.mp4 --confidence_threshold 0.5 --filter_label person
```

Este comando iniciará o detector de objetos usando um arquivo de vídeo local como fonte de entrada. Ele definirá o limite de confiança para 0.5 e filtrará apenas os objetos da classe "person".

## Créditos

Este projeto foi desenvolvido por Dr Dheiver Francisco Santos como parte de um projeto de detecção de objetos.
