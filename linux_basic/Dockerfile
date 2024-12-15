# 軽量なDebianを使用
FROM debian:bullseye-slim

# ツールのインストール
RUN apt-get update && apt-get install -y --no-install-recommends \
    bash \
    mlocate \
    procps \
    htop \
    vim \
    file \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# デフォルトの作業ディレクトリ
WORKDIR /workspace

# デフォルトのエントリーポイント
CMD ["/bin/bash"]