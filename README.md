**Image Segmentation using SAM Model**

Este repositório contém um script Python para realizar a segmentação de imagens utilizando o modelo SAM (Segment Anything Model) com uma arquitetura Vision Transformer (ViT). O SAM Model é fornecido pela Facebook Research e é capaz de segmentar objetos em imagens de forma automática.

### Pré-requisitos
- Python 3.6 ou superior
- GPU (opcional, mas altamente recomendado para acelerar o processo)

### Instalação
1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/nome-do-repositorio.git
   cd nome-do-repositorio
   ```

2. Instale as dependências necessárias:
   ```bash
   pip install -r requirements.txt
   ```

### Uso
1. Baixe o modelo pré-treinado (SAM ViT) e coloque-o na pasta `weights`. Você pode usar o seguinte comando:
   ```bash
   wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth -P weights/
   ```

2. Coloque a imagem que deseja segmentar na pasta `data`.

3. Execute o script Python:
   ```bash
   python main.py
   ```

4. Os resultados serão salvos na pasta `output`.

### Configuração
- O script `main.py` contém um exemplo de uso da classe `ImageSegmentation`. Você pode ajustar os parâmetros, como tipo de modelo, caminho do checkpoint, e tamanhos de grade, de acordo com suas necessidades.

### Contribuições
Contribuições são bem-vindas! Se encontrar problemas ou tiver sugestões de melhorias, sinta-se à vontade para abrir uma issue ou enviar um pull request.

### Licença
Este projeto é licenciado sob a [MIT License](LICENSE).

---

**Créditos:**
Este projeto utiliza o modelo SAM fornecido pelo Facebook Research e as bibliotecas supervision, OpenCV, e PyTorch. Agradecemos a essas comunidades pelo trabalho incrível.
