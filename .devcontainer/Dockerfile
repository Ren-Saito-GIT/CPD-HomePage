FROM hcncrobotteam/h-stella-mariadb:latest
# 作業ディレクトリ
WORKDIR /workspace

# 必要なパッケージのインストール
RUN apt-get update \
	&& apt-get install -y --no-install-recommends \
		git \
		build-essential \
		libgl1-mesa-glx \
		libglib2.0-0 \
		libsm6 \
		libxext6 \
		libxrender-dev \
		ffmpeg \
	&& rm -rf /var/lib/apt/lists/*
