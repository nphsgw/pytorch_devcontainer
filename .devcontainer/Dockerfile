FROM pytorch/pytorch:1.11.0-cuda11.3-cudnn8-devel
# ベースイメージによってはdocker build時にGPGエラーが発生して途中で止まる。
# その場合、<https://zenn.dev/takakurasato/scraps/d3e0ee6132a5c5>を参考にして解決する。
RUN apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/ubuntu1804/x86_64/3bf863cc.pub
RUN apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/ubuntu1804/x86_64/7fa2af80.pub

RUN apt-get update && apt-get install -y \
    git wget libgl1-mesa-glx libglib2.0-0\
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN pip install jupyter black flake8 mypy numpy pandas matplotlib scikit-learn opencv-python torchinfo torchsummary