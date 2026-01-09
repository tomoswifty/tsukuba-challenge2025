# つくばチャレンジ2025のソースコードメタパッケージ
- ROS 2 humble

## vcs のインストール
インストールされている場合，この手順をスキップしてください．

1) vcstool のインストール
Ubuntu / Debian 系
```
sudo apt update
sudo apt install -y python3-vcstool
```

macOS（Homebrew）
```
brew install vcstool
```

pip（どの環境でも）
```
python3 -m pip install -U vcstool
```

# インストール
```
cd ros2_ws/src/
git clone https://github.com/tomoswifty/tsukuba-challenge2025.git
mkdir -p src
vcs import src < repos.yaml
```

取得できたか確認
```
vcs status src
```

すでに取得済みのリポジトリを更新（pull相当）
```
vcs pull src
```