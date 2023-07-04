# AI 調査Topページ
## 一覧
| AI名 | 運営 | 利用者数 | In/Out | タイプ | 使い方 | 料金 | 使用例 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ChatGPT | Open AI | 2023年1月時点で1億人 | テキスト | 生成系 | 対話・一問一答 | Ver3.5は無料、Ver4は有料 | Bing、LINE公式アカウントなど（https://first-contact.jp/blog/article/chat-gpt-case-study/） |
| Google Bard | Google | 未公表 | テキスト、画像(英語版のみ) | 生成系 | 対話・一問一答 | 無料 | Google、JAL |
| GitHub Copilot | GitHub（Microsoft） | 不明（GitHubは2023年2月時点で１億人以上） | テキスト | コード支援 | 予測変換出力 | 60日間は無償、以降は有料 | OLTAクラウドファンディング、FastLabel、スカイディスク（ある意味Microsoft、JetBrains） |

## 各AIの特徴
### テキスト生成系
1. ChatGPT
    1. 概要
        * Generative Pre-trained Transformer（GPT）を使用(https://zero2one.jp/ai-word/gpt/)
        * インターネット上のテキストデータセットを学習
        * 対話、テキストの生成に焦点を当てた微調整がされている
    1. 強み
        * インターネット上の膨大なテキストをデータセットとしているため、テキストの生成や対話において自然なやり取りが可能
        * テキストデータにはプログラムも含まれているため、特にVer4ではプログラム言語、フレームワーク、ビルドツールなどを指定するだけでも簡単なアプリケーションを作成することが可能
        * 他言語に対応している
        * リアルタイムに回答を生成するが一度学習しているレスポンスは速い
        * APIが存在するため、別のアプリケーションに組み込むことも可能（Bingなど）
        * データセットに基づいたものであればクリエイティブな作業もできる
    1. 弱み
        * データセットが2021年9月までのものであるため、情報が古い可能性がある（今後アップデート予定）
        * 間違った情報や無関係な情報を出力することがある
        * いわゆる行間や細かい感情を読む必要がある作業は苦手
        * 何もないところからアイデアを生み出す作業は苦手
    1. 公式Webサイト
        * https://openai.com/chatgpt
1. Google Bard
    1. 概要
        * Googleが開発したテキストベースの生成系AI
        * Pathways Language Model(PaLM2)を使用(https://arxiv.org/pdf/2204.02311.pdf)
        * Google検索からデータセットを学習している
        * ChatGPTとほぼ同様の強みと弱みがある
    1. 強み
        * 無料で使用可能
        * Google検索を学習しているため、最新情報まで出力される
        * 使った際、参考にしたWebサイトのリンクが付与されてくる
        * Web上で生成系AIを作成するためのツールが公開予定(MakerSuite)
        * 英語版のみだが、画像のI/Oに対応している
    1. 弱み
        * 試験運用中のため、突然使えなくなる可能性がある
        * ChatGPTと違ってスレッドが１つしかない
        * 出力結果がChatGPTと比べて内容が薄い
        * 主要な言語には対応しているが、現在は8ヶ国語までしか対応していない
        * APIがまだ公開されていない(今後公開予定→PaLM API)
    1. 公式Webサイト
        * https://bard.google.com/
### コード支援
1. GitHub Copilot
    1. 概要
        * GitHub（Microsoft傘下）とOpen AIが共同開発
        * 内部はGPTベースのAIを使用
        * VSCode、IntelliJ IDEAのプラグインとして実行可能
        * 学習データはGitHub上に公開されているソースコード
        * コードやコメントを記載していくと何が必要か予測してサジェストしてくれる
    1. 強み
        * 単純にソースコードを書く時間が短縮されるため、生産性が上がる可能性が高い
        * よく使われるIDEで使用することができる（VSCode、IntelliJ、Android Studioなど）
        * 慣れていないプログラム言語でコーディングする場合のキャッチアップ支援となる
        * コメントを記載するだけで、関数レベルでのプログラミングが可能（例・・・次の閏年を計算するなど→https://giginc.co.jp/blog/giglab/github-copilot）
        * Python、JavaScript、TypeScript、Ruby、Go、C#、C++が特に適しているとされているが、それ以外にもJavaやPHPなど主要言語はカバーできる
    1. 弱み
        * 有料プランしかない
        * 未だ一部で根強いEclipseはサポート対象外となっている
        * 出力されたコードを確認する作業は必要
        * 複雑な業務ロジックを生成するにはコメントを多く記載する必要がある
    1. 公式Webサイト
        * https://docs.github.com/ja/copilot
## その他AI
下記のWeb記事にたくさんAIが紹介されている
1. https://qiita.com/elliot_tk/items/fd002ade309d4cac0a9f
1. https://www.octoparse.jp/blog/top-20-artificial-intelligenceai-tools-for-2023
1. https://find-a.jp/seotimes/whats-ai-tool-genre/
