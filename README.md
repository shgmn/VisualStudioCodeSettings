# Visual Studio Codeのユーザ設定同期方法

## for Mac
1. Visual Studio Codeをインストールする
2. このリポジトリをクローンする

    /path/to/setting/

3. macブランチを切り替える
4. Visual Studio Codeの設定ディレクトリに移動する

    cd ~/Library/Application Support/Code/

5. シンボリックリンクを張る

    rm -rf /path/to/setting/User  
    ln -s /path/to/setting/User User

## for Windows
1. Visual Studio Codeをインストールする
2. このリポジトリをクローンする

    /path/to/setting/

3. windowsブランチに切り替える
4. Visual Studio Codeの設定ディレクトリに移動する

    cd ~/AppData/Roaming/Code

5. シンボリックリンクを張る(要管理者権限)

    mklink /D User /path/to/setting/User
