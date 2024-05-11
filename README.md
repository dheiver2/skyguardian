
# Detecção de Pessoas em Vídeo usando YOLO-NAS-L

Este é um script Python que usa o modelo YOLO-NAS-L para detectar pessoas em um vídeo e desenha caixas delimitadoras ao redor delas.

## Requisitos

- Python 3
- OpenCV (cv2)
- Super Gradients (super_gradients)
- NumPy (numpy)

## Instalação

Você pode instalar as dependências usando pip:

```
pip install opencv-python super_gradients numpy
```

## Uso

1. Baixe o vídeo de entrada e salve-o em seu computador.
2. Altere o caminho do vídeo de entrada no código para o caminho correto em sua máquina.
3. Execute o script.

O vídeo resultante com as detecções será salvo no mesmo diretório do script com o nome `output_video.mp4`.

## Personalização

Você pode personalizar a detecção ajustando o limite de confiança para detecções de pessoas. Isso pode ser feito alterando o valor da variável `confidence_threshold` no código.

## Créditos

Este script utiliza o modelo YOLO-NAS-L fornecido pela biblioteca Super Gradients.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

```

Você pode salvar este conteúdo em um arquivo chamado `README.md` no mesmo diretório do seu código. Certifique-se de ajustar os detalhes conforme necessário para o seu projeto.
