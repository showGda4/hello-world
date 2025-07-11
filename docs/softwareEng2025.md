---
layout: page
title: "software Eng. lecture note"
permalink: /docs/softwafeEng2025
---

# ソフトウェア工学の内容まとめ
## 第1回
この講義ではソフトウェア・エンジニアリングスキルの基礎知識の理解及び実務的なスキルの習得を目標とする。本講義の講師を務める堤田先生は非情報学分野からITエンジニアになっており、ソフトウェア開発の経験を有している。現在、AI Agentによるソフトウェア開発が盛んになっており、監督者としての能力がより求められている。
## 第2回
ソフトウェアは情報を扱うプロダクトそのものであり、プロダクトを提供する手段である。ソフトウェアはコンピュータプログラム、データ構造、プログラム操作や使用法を記した情報で定義され、ハードウェアと異なり劣化しないが、悪化はする。ソフトウェア工学は「品質」、「コスト」、「納期」の最適なバランスを実現するための手法・方法論のことである。
## 第3回
ソフトウェアライフサイクルとはソフトウェアの誕生から開発・運用を経て廃止に至るまでの一連の流れのことを指す。ライフサイクルの中でも計画、要件定義、設計、製作、テスト・デバッグ、運用・保守というように分けられている。要件定義とは実現する機能と実現しない機能を明確にすることであり、その定義を様々な相手に共有する。作成された要件定義書を設計書にし、その設計書に従ってシステム構築を行う。制作には内製と外製がある。複数人でのソフトウェア開発にはドキュメンテーションが必要になる。
## 第4回
プロジェクトは独自性をもつ仕事であり、目標が明確に設定されてあるバックキャスティングの性質を持つ。ソフトウェア開発には品質（Qualitiy）、コスト（Cost）、納期（Delivery）があり、システムの性質によって優先度が変わる。ソフトウェア評価の方法として、ステップ数を基にしたバグ発生率、ファンクションポイント法、使い勝手などがある。開発プロセスとしてウォータフォール、アジャイル、計画駆動型、スパイラル、反復型などがあるが一長一短であり、場面・要求によって選ぶ必要がある。また、ハイブリッド型で開発を進めることも多い。
## 第5、6回
WBSとはプロジェクト目標を達成し、必要な要素成果物を生成するために、プロジェクトチームが実行する作業を、要素成果物を主体に階層的に要素分解したものである。WBSを作成することでスコープが明確になることや作業を洗い出せること、全体管理と作業計画が明確化されることなどのメリットがある。WBSを作るために、まずスコープを明確にする。その後、大きな作業をグルーピングし、グルーピングした作業の相互関連を考え、各グループの作業を洗い出す。
## 第7回
コードは書くことよりも読まれることのほうが多く、ソフトウェア開発にあたり読みやすくなるようにコーディングすることが必須となる。コーディング規則の例としてPEP8がある。PEP8では、１行の長さ、レイアウト、スペース、改行、命名に規則がある。例えば、１行の長さは79文字以内にする、演算子の前後にはスペースを前後に一つずつ空けるなどがある。PEP8に基づくコードチェックツールとしてflake8がある。
## 第8、10回
バージョン管理では、「誰が」、「いつ」、「どのように」変更したかを管理し、これによって、多数のメンバーでも共同でコード開発ができるようになる。バージョン管理には、集中管理型と分散管理型がある。集中管理型は、リモートレポジトリでのみバージョン管理を行うため、同期に時間がかかりやすく、コンフリクトも発生しやすい。分散管理型はローカルレポジトリでもバージョン管理を行うため、リモートへのアクセスが減り、障害に強くなる。gitとは分散管理型のバージョン管理システムのことである。ファイルの作成・変更・削除の記録をコミットで行う。コミットにより登録された変更をgit pushでリモートレポジトリへ反映し、git pullでリモートレポジトリの内容をローカルレポジトリに反映させる。ブランチを使用して作業を枝分かれさせることで共同作業・へ移行作業が可能となる。.gitignoreを用いてgitに管理してほしくないファイルを指定することができる。
## 第11回
githubはリモートレポジトリのホスティングサービスの1つであり、オープンソースソフトウェアの主要なポータルサイトである。cloneでgithub上のリポジトリをローカルにダウンロードし、forkで他人のリポジトリを自分のgithubアカウントにコピーする。レポジトリに関する質問を挙げるための機能としてissuesがあり、issuesなどを管理するためのテーブルとしてprojectsがある。
## 第12回
Continuous Integration(CI)とはコード変更を共有リポジトリに頻繁に統合するプロセスのことである。自動テストとビルドを定期的に実行し、バグの早期発見と修正を可能にする。これにより、開発のスムーズな進行を促進する。Continuous Delivery(CD)とはコード変更をテスト環境や本番環境に自動的にデプロイするプロセスのことである。これによりユーザーフィードバックを迅速に反映することが可能となる。Github Actionsを使用してCI/CDを実現することができる。
## 第13回
Github Pagesを用いてGithubにあるリモートレポジトリの内容をwebpageとして公開することができる。HP更改はCI/CDにより自動化されており、Jekyllを使用することでmarkdownファイルを自動でhtml化することができる。これにより、開発者はmarkdownファイルを作成すればよいということになる。