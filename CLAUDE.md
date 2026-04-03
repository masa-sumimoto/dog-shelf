# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**DOG SHELF** は、Claude デスクトップアプリの **Cowork** を活用して、Web 関連の最新情報を自動収集・整理するリポジトリ。

## Core Workflow

```
Cowork (スケジュール実行)
    → Web ニュースを収集
    → GitHub Issues に投稿 (1件1issue)
    → README.md を自動更新 (ダイジェスト表示)
```

## Cowork について

Claude デスクトップアプリ専用のタスク実行・スケジューリング機能。
このリポジトリのルーティン業務（情報収集・Issues投稿・README更新）は Cowork で定義・管理する。

**Cowork プロジェクト名**: `dog-shelf`

## Conventions

- **Issues**: ニュースエントリーの媒体。1件1issue を基本とする
- **README.md**: 収集した情報のダイジェストを表示するハブとして機能する
