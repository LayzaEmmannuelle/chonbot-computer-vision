🤖 ChonBot - Visão Computacional e Mapeamento de Ambiente Exógeno

Repositório dedicado ao módulo de Visão Computacional e Percepção do projeto ChonBot, desenvolvido no âmbito do curso de Sistemas de Informação no CEFET/RJ. O projeto explora a integração entre sistemas multiagentes (SMA) utilizando o framework JaCaMo e algoritmos de Deep Learning (YOLOv8) para o mapeamento e localização de objetos em ambientes exógenos.

📋 Sobre o Projeto

O objetivo principal desta etapa é construir uma "ponte de dados" confiável que capte o ambiente real através de uma câmara zenital, detete os robôs e os objetos de interesse (como a bola) em tempo real, e extraia coordenadas espaciais precisas para alimentar o raciocínio cognitivo BDI (Crenças, Desejos e Intenções) dos agentes.

🚀 Funcionalidades Atuais

Aquisição e Tratamento de Imagens: Captura de fluxo de vídeo em tempo real através de câmara/webcam.

Deteção com YOLOv8: Modelo treinado com dataset personalizado para alta precisão e baixa taxa de falsos positivos.

🛠️ Tecnologias Utilizadas

Python 3.12+

Ultralytics YOLOv8 (Deep Learning para Deteção de Objetos)

OpenCV (cv2) (Processamento de Imagem)

⚙️ Como Executar o Projeto

1. Clonar o Repositório

git clone https://github.com/teu-utilizador/chonbot-computer-vision.git
cd chonbot-computer-vision


2. Criar e Ativar o Ambiente Virtual (venv)

No Windows (PowerShell):

python -m venv venv_visao
.\venv_visao\Scripts\Activate.ps1


No Linux / macOS:

python3 -m venv venv_visao
source venv_visao/bin/activate


3. Instalar as Dependências

pip install --upgrade pip
pip install opencv-python ultralytics flask


4. Executar o Script de Deteção

python train_local.py
