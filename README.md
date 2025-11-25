# 🏷️ タグ入力補助 for イロミライ ＆ ちちぷい (autoTagsFiller) v7.3

このスクリプトは、**AIイラスト投稿サイト**「**イロミライ (Iromirai)**」および「**ちちぷい (Chichi-pui)**」の投稿ページで、テーマタグの入力を補助するUserScriptです。

繰り返し使うタグをテンプレートとして保存し、**ワンクリックで入力から確定までを自動**で行うことで、投稿作業の**手間を大幅に削減**します。

---

## 🚀 インストール方法

UserScriptのインストールは、**GreasyFork**から行うのが**最も簡単**です。

**[✨ GreasyForkでインストールする ✨](https://greasyfork.org/scripts/542540)**

### 拡張機能の準備

このスクリプトを使うには、UserScript管理のための拡張機能が必要です。

   * **Tampermonkey**: [https://www.tampermonkey.net/](https://www.tampermonkey.net/)
   * **ScriptCat**: [https://scriptcat.org/](https://scriptcat.org/)

---

## 🎀 機能紹介と使い方

このスクリプトは、単なる入力補助ではなく、**タグ管理機能**を内蔵しています。

### 📌 タグの入力と確定について
* **保存タグの区切り**: テンプレートに保存するタグは、**半角カンマ**（**,**）で区切って入力します。
* **自動タグ確定**: タグを適用すると、自動的にサイト側の「**タグ追加**」**ボタンをシミュレーション**し、一つずつ確定させます。
* **Enter不要**: `change`イベントを利用しているため、タグ入力後、**入力エリア外をクリック**するだけでもタグが追加・確定されます。半角カンマ区切りのタグをコピペした後も利用可能です。

### 🏷️ タグ管理機能の使い方
* **並び替え**: テンプレートリストは**ドラッグ＆ドロップ**で簡単に順番を変更できます。
* **フィルター**: 名前（テーマタグ名）でも、タグの文字列でも**絞り込み**が可能です。
* **インポート**: 外部拡張機能「**TextFill**」でエクスポートしたデータも読み込むことができ、テンプレートとして利用できます。
* **エクスポート**: このスクリプトでエクスポートしたデータは、TextFillで読み込むことは可能ですが、コマンドや説明が空欄になります。（※TextFillのデータ構造との互換性によるものです。）

---

## 💻 技術的な特徴

* **マルチサイト対応**: イロミライとちちぷいの両方のDOM構造を判別し、適切に動作します。
* **イベントシミュレーション**: タグの自動確定は、DOMの`input`イベントや`click`イベントをシミュレーションして行われ、サイトの機能を最大限に活用しています。
* **GM_configによる設定**: テンプレートデータは`GM_getValue/GM_setValue`を使って安全に永続化されます。

---

## 🛡️ ライセンスについて (License)

このアプリケーションのソースコードは、ねおんが著作権を保有しています。  
The source code for this application is copyrighted by Neon.

* **ライセンス**: **[CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/deed.ja)** です。（LICENSEファイルをご参照ください。）
* **商用利用不可**: 個人での利用や改変、非営利の範囲内での再配布はOKです。**商用目的での利用はご遠慮ください**。  
  **No Commercial Use**: Personal use, modification, and non-profit redistribution are permitted. **Please refrain from commercial use.**  
※ ご利用は自己責任でお願いします。（悪用できるようなものではないですが、念のため！）

---

## 開発者 (Author)

**ねおん (Neon)**
<pre>
<img src="https://www.google.com/s2/favicons?domain=bsky.app&size=16" alt="Bluesky icon"> Bluesky       :<a href="https://bsky.app/profile/neon-ai.art">https://bsky.app/profile/neon-ai.art</a>
<img src="https://www.google.com/s2/favicons?domain=github.com&size=16" alt="GitHub icon"> GitHub        :<a href="https://github.com/neon-aiart">https://github.com/neon-aiart</a>
<img src="https://www.google.com/s2/favicons?domain=greasyfork.org&size=16" alt="Greasy Fork icon"> Greasy Fork   :<a href="https://greasyfork.org/ja/users/1494762">https://greasyfork.org/ja/users/1494762</a>
<img src="https://www.google.com/s2/favicons?domain=www.chichi-pui.com&size=16" alt="chichi-pui icon"> chichi-pui    :<a href="https://www.chichi-pui.com/users/neon/">https://www.chichi-pui.com/users/neon/</a>
<img src="https://www.google.com/s2/favicons?domain=iromirai.jp&size=16" alt="iromirai icon"> iromirai      :<a href="https://iromirai.jp/creators/neon">https://iromirai.jp/creators/neon</a>
<img src="https://www.google.com/s2/favicons?domain=www.days-ai.com&size=16" alt="DaysAI icon"> DaysAI        :<a href="https://www.days-ai.com/users/lxeJbaVeYBCUx11QXOee">https://www.days-ai.com/users/lxeJbaVeYBCUx11QXOee</a>
</pre>

---
