# ex-h4-hello2

- [h4-hello · PyPI](https://pypi.org/project/h4-hello/)
- [heiwa4126/h4-hello: A practice project for publishing Python projects created with uv to PyPI with PEP740 signatures.](https://github.com/heiwa4126/h4-hello)

を使う直接参照のサンプル。
GitHub リポジトリから直接取得(Direct reference)する。

具体的には

```sh
uv add "h4-hello@git+https://github.com/heiwa4126/h4-hello.git"
```

したもの。

## 実行

clone したら、プロジェクトのルートで

```sh
uv run ex-h4-hello2
```

## 注意

uv で
GitHub リポジトリから直接取得する場合、
コミットハッシュを uv.lock に保存している。

`@ref`をつけなかった場合でもそれは同じで、
参照元が更新されて HEAD が進んだ場合でも追従しない。
