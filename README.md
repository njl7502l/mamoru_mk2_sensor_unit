# kicad-template

このテンプレート使用の際はリポジトリクローン後に以下のコマンドを実行.

```
zsh init
```

コマンド実行後、以下の処理が走り、kicad開発環境を自動生成する

1. 各種作業ファイル生成

    `Untitled`になっている`kicad_pcb`, `kicad_pro`, `kicad_sch`の3ファイルをプロジェクト名に変更

2. KiCadのフットプリント・シンボルライブラリのクローン

    以下2つのリポジトリをサブモジュールとしてクローンする

- https://github.com/njl7502l/njl7502l-kicad-library
- https://github.com/Digi-Key/digikey-kicad-library

3. シンボルライブラリテーブルの自動生成

    digikeyのシンボルライブラリは更新によって数が増減するかもしれないので、clone毎に関連付けを自動生成する

4. githubへのpush
