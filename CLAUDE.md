# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## プロジェクト概要

- プロジェクト名: quiz-app
- 内容: 一般常識クイズアプリ
- 技術スタック: HTML / CSS / JavaScript(素のフロントエンド構成。フレームワークやビルドツールは使用しない）

現時点でこのリポジトリにはまだソースコードが存在しない（初期状態）。今後 `index.html` / `style.css` / `script.js` などのファイルが追加されていく想定。

## 開発コマンド

ビルドツールは使用しない静的サイト構成のため、npm 等のパッケージ管理は基本的に不要。

- ローカルでの動作確認: `index.html` をブラウザで直接開く、または簡易サーバーを立てる
  - `python -m http.server` （Python がある場合）
  - VS Code の Live Server 拡張機能を使う
- テスト/リント/ビルドの仕組みは未導入。導入した場合はこのセクションを更新すること。

## アーキテクチャ方針

- 素の HTML/CSS/JavaScript で実装し、外部フレームワーク（React 等）は使用しない。
- クイズの問題データ（問題文・選択肢・正解）は JavaScript の配列・オブジェクトとして管理する想定。
- 画面遷移（出題→回答→採点→結果表示）は SPA 的に DOM の表示切り替えで行う想定（複数 HTML ページに分割するかは実装時に判断）。

※ 実装が進んだら、実際のファイル構成・データ管理方法・画面遷移の仕組みに合わせてこのセクションを具体化すること。
