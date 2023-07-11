# sample_resume_generator

## 機能概要

履歴書の自己PR文の例を自動生成します。LangChain の勉強のために作成したサンプルプログラムです。
- 入力項目
  - 応募先企業の説明文
  - あなたの長所
- 出力項目
  - 応募先企業のSWOT分析(強み（Strength）、弱み（Weakness）、機会（Opportunity）、脅威（Threat）)の予測結果。
  - 応募先企業が直面している課題の予測結果。
  - あなたの履歴書の自己PR文の例。あなたの長所を活用することで、あなたが、応募先企業の課題解決に貢献できることをアピールする内容。

## 処理概要

以下のようなステップを踏んで自動生成を行っています。

1. 応募先企業のSWOT分析
    - 「応募先企業の説明文」から、SWOT分析を行う。
2. 応募先企業の課題分析
    - 1.の分析結果から、課題分析を行う。
3. 応募先企業への自己アピール文の生成
    - 2.の分析結果で得られた課題の解決に、「あなたの長所」が貢献できることをアピールする内容の文を生成する。

## 実行方法

sample_resume_generator.ipynb を google colaboratory 上で実行してください。以下のリンクから実行することもできます。
- [open in Colab](https://colab.research.google.com/github/kagiya00/sample_resume_generator/blob/main/sample_resume_generator.ipynb)

## 主な利用ライブラリ/サービス

- LangChain
- OpenAI の gpt-3.5-turbo
