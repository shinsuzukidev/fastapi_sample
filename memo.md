# FastAPI サンプル

## python の仮想環境構築

### 仮想環境を構築する

次のサイトを参考に仮想環境と構築する。

https://www.python.jp/install/windows/venv.html

### 仮想環境作成

環境構築はコマンドプロンプトから行う。

#### プロジェクトのフォルダを作成

```cmd
C:\Users\user1>mkdir sample1
```

#### 仮想環境を作成

```cmd
C:\Users\user1\sample1>python -m venv .venv
```

### 仮想環境操作用に Bat ファイル を作成する。

```bat
# 仮想環境のルートに _activate.bat を作成
# 仮想環境に切り替える
%~dp0.venv\Scripts\activate.bat
```

```bat
# 仮想環境のルートに _deactivate.bat を作成
# 仮想環境の終了を実行
%~dp0.venv\Scripts\deactivate.bat
```

```bat
# 仮想環境のルートに _requirements.bat を作成
# パッケージのリストを出力
pip freeze > requirements.txt
```

### 仮想環境に切り替え

Scripts\activate.bat を実行。仮想環境に切り替える。  
コマンドプロンプトに(.venv)と表示される。仮想環境で実行中であることを示す。

```cmd
C:\Users\user1\sapmle1>.venv\Scripts\activate.bat
(.venv) C:\Users\user1\sample1>
```

### 仮想環境の終了

```cmd
(.venv) C:\Users\user1\sample1> deactivate
C:\Users\user1\sample1>
```
