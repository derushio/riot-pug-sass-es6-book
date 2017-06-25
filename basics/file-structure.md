# ファイル構成について

## ファイル構成

* proj/
    * README.md
    * .gitignore
    * .babelrc
    * webpack.config.babel.js
    * node_modules/
    * src/
        * index.pug
        * script/
            * entry/
                * index.js
            * tag/
        * style/
            * _common.sass
            * entry/
                * index.sass
    * dist/
    * tool/
        * build/

## ファイル解説
 * proj/
     * README.md  
        このプロジェクトについての仕様等が書いてあります。  
        ご一読下さい。

     * .gitignore  
        バージョン管理上で管理しないファイルを管理します。  
        バージョン管理を使用しない場合は無視して下さい。

     * .babelrc  
        es2015(es6)仕様のjavascriptをサポートするためのconfigファイルです。  
        cpコマンドやFinderでコピーしようとすると抜けてしまうことが多いので隠しファイル表示やcpコマンドの実行方法をよく考えて下さい。

     * webpack.config.babel.js  
        webpackの実行オプションです。  
        _エントリポイントが増えた場合はこちらも編集してください。_

     * src/  
        開発者が管理するリソースファイルは全てこのディレクトリ以下に配置して下さい。

     * dist/  
        コンパイル後のファイルはすべてここにコピーされます。

     * tool/  
        コンパイルのためのスクリプトや便利なスクリプトはこちらに配置して下さい。

 * proj/src/
     * index.pug  
        最初からエントリポイントに設定されているpugファイル。

     * script/
         * entry/  
            エントリポイントに対応するjsを配置する場所。

             * index.js  
                index.pugに対応するjsのエントリファイル。

         * tag/  
            Riotのタグファイルを配置する場所。

     * style/
         * _common.sass  
            sassのimport機能で呼び出すsassサブモジュール。

         * entry/  
            エントリポイントに対応するsassを配置する場所。

             * index.sass  
                index.pugに対応するsassのエントリファイル。
