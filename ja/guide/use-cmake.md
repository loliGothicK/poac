## cmakeを使う

```yaml
build:
  system: poac
```

現状，systemに対して，poacを指定すると，poac標準のビルドシステムを使うことができますが，
cmake等を使うこともできます．
systemにcmakeを指定すると，poac build時に，プロジェクトルートから，CMakeLists.txtを選択してビルドできます．
```
mkdir _build
cmake ..
make
```
という処理を行ってくれます．
適宜途中の処理は省かれます．
CMakeLists.txtの編集がなければ`make`のみ行われるといった処理．
