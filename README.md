**Image Segmentation using SAM Model**

Este repositório contém um script Python para realizar a segmentação de imagens utilizando o modelo SAM (Segment Anything Model) com uma arquitetura Vision Transformer (ViT). O SAM Model é fornecido pela Facebook Research e é capaz de segmentar objetos em imagens de forma automática.

### Pré-requisitos
- Python 3.6 ou superior
- GPU (opcional, mas altamente recomendado para acelerar o processo)

### Instalação
1. Clone este repositório:
   ```bash
   git clone git@github.com:dheiver/ImageSegmentation.git
   cd nome-do-repositorio
   ```

2. Instale as dependências necessárias:
   ```bash
   pip install -r requirements.txt
   ```

### Uso
1. **Baixe o modelo pré-treinado (SAM ViT) e coloque-o na pasta `weights`.**

- **Para Linux e macOS:**
   ```bash
   wget https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth -P weights/
   ```

- **Para Windows (Git Bash):**
   ```bash
   curl -O https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth -P weights/
   ```

- **Para Windows (PowerShell):**
   ```powershell
   Invoke-WebRequest -Uri https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth -OutFile weights/sam_vit_h_4b8939.pth
   ```

2. Coloque a imagem que deseja segmentar na pasta `data`.

3. No arquivo Jupter 'YourImageSegmentation.ipynb' Execute o script Python com a class ImageSegmentation:
  
4. Visualize o resultado.

### Configuração
- Em 'ExemploImageSegmentation.ipynb' contém um exemplo de uso da classe `ImageSegmentation`. Você pode ajustar os parâmetros, como tipo de modelo, caminho do checkpoint, e tamanhos de grade, de acordo com suas necessidades.

### Contribuições
Contribuições são bem-vindas! Se encontrar problemas ou tiver sugestões de melhorias, sinta-se à vontade para abrir uma issue ou enviar um pull request.

### Licença
Este projeto é licenciado sob a [MIT License](LICENSE).

---

**Créditos:**
Este projeto utiliza o modelo SAM fornecido pelo Facebook Research e as bibliotecas supervision, OpenCV, e PyTorch. Agradecemos a essas comunidades pelo trabalho incrível.
