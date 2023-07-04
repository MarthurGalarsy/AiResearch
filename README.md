# AI 調査Topページ
## 一覧
| AI名 | 運営 | 利用者数 | In/Out | タイプ | 使い方 | 料金 | 使用例 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| ChatGPT | Open AI | 2023年1月時点で1億人 | テキスト | テキスト生成系 | 対話・一問一答 | Ver3.5は無料、Ver4は有料 | Bing、LINE公式アカウントなど（https://first-contact.jp/blog/article/chat-gpt-case-study/） |
| Google Bard | Google | 未公表 | テキスト、画像(英語版のみ) | テキスト生成系 | 対話・一問一答 | 無料 | Google、JAL |
| GitHub Copilot | GitHub（Microsoft） | 不明（GitHubは2023年2月時点で１億人以上） | テキスト | コード支援 | 予測変換出力 | 60日間は無償、以降は有料 | OLTAクラウドファンディング、FastLabel、スカイディスク（IDEでMicrosoft、JetBrains） |
| Amazon CodeWhisperer | Amazon | 未公表 | テキスト | コード支援 | 予測変換出力 | 個人は無料、企業は有料 | 未公開（IDEでMicrosoft、JetBrains） |
| Amazon Bedrock | Amazon | 未公表 | - | AIプラットフォーム | API経由 | まだ未公開 | Codaなどが一部先行利用中 |

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
        * オフライン環境では利用できない
    1. 公式Webサイト
        * https://docs.github.com/ja/copilot
1. Amazon CodeWhisperer
    1. 概要
        * Amazon版のGitHub Copilotと言えるAIコーディング支援ツール
        * 主にAmazon内部リポジトリから学習している
        * GitHub Copilotとほぼ同様の強みと弱みがある
    1. 強み
        * 個人であれば無料で利用可能
        * AWSアカウントも不要で利用可能
        * AWS関連のサジェストが強い
        * Amazon公式からJavaやKotlinなどもサポート対象とされている
        * セキュリティやライセンスの検知などが得意とされている
    1. 弱み
        * 公式では日本語に対応していない
        * 現在はバージニアリージョンのみ利用可能なので、情報の取得が遅い可能性がある
    1. 公式Webサイト
        * https://aws.amazon.com/jp/codewhisperer/
## AIプラットフォーム
1. Amazon Bedrock
    1. 概要
        * Amazonが開発したAIサービスを作成するためのプラットフォーム
        * 複数の基盤モデルが存在しており、サービスを作りたい人が目的に適したモデルを選択できる
        * モデルの種類はAI21のJurassic-2モデル（言語処理用）、AnthorpicのClaude（AIアシスタントモデル）、Stability AIのStable Diffusion（画像生成用）、AmazonのTitanモデル（要約・テキスト生成・情報抽出などといったタスクに適した「Titan Text」、テキスト入力を数値表現に変換する「Titan Embeddings」）
    1. 強み
        * 対話型だけではないサービスに応じた複数のモデルを利用することができる
        * モデルを独自のデータでカスタマイズすることが可能
        * AWSとの連携や神話異性が高いと予想される
    1. 弱み
        * まだ正式にサービス開始していないため、詳細や事例が少ない
        * 料金についても不明
    1. 公式Webサイト
        * https://www.aboutamazon.com/news/aws/aws-amazon-bedrock-generative-ai-service
        * https://reinforz.co.jp/bizmedia/4493/(公式ではない) 
## その他AI
下記のWeb記事にたくさんAIが紹介されている
1. https://qiita.com/elliot_tk/items/fd002ade309d4cac0a9f
1. https://www.octoparse.jp/blog/top-20-artificial-intelligenceai-tools-for-2023
1. https://find-a.jp/seotimes/whats-ai-tool-genre/


PKSHA Chatbot

Elyza Pencil
Jasper AI

Midjourney
DALL・E 2

voitra
Prediction One
Neural Network Console
