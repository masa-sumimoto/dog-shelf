---
version: alpha
name: kobe-harbor-ticket
description: 神戸の海沿いエリアを巡るデジタルチケットの販売促進LP

colors:
  # Harbor Blue — 神戸の深海と広大な空を象徴する青
  primary-50:  "#E3F2FD"
  primary-100: "#BBDEFB"
  primary-200: "#90CAF9"
  primary-300: "#64B5F6"
  primary-400: "#42A5F5"
  primary-500: "#2196F3"
  primary-600: "#1E88E5"
  primary-700: "#1976D2"
  primary-800: "#1565C0"
  primary-900: "#0D47A1"
  primary-950: "#0A2558"
  # Stylish Pink — スイーツ、華やかさ、港町のモダンなアクセント
  secondary-50:  "#FCE4EC"
  secondary-500: "#E91E63"
  secondary-950: "#880E4F"
  # Neutrals
  neutral-canvas:    "#F8FAFC"
  neutral-surface:   "#FFFFFF"
  neutral-ink:       "#0F172A"
  neutral-ink-muted: "#475569"
  neutral-rule:      "#E2E8F0"

typography:
  base:
    fontFamily: "'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: "1.8"
    letterSpacing: "0em"
  display:
    fontFamily: "'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif"
    fontSize: "72px"
    fontWeight: 700
    lineHeight: "1.15"
    letterSpacing: "-0.01em"
  heading-2:
    fontFamily: "'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif"
    fontSize: "44px"
    fontWeight: 700
    lineHeight: "1.3"
    letterSpacing: "-0.01em"
  heading-3:
    fontFamily: "'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif"
    fontSize: "24px"
    fontWeight: 700
    lineHeight: "1.4"
    letterSpacing: "0em"
  heading-4:
    fontFamily: "'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif"
    fontSize: "17px"
    fontWeight: 700
    lineHeight: "1.4"
    letterSpacing: "0em"
  lead:
    fontFamily: "'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: "1.8"
    letterSpacing: "0em"
  small:
    fontFamily: "'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: "1.8"
    letterSpacing: "0em"
  caption:
    fontFamily: "'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif"
    fontSize: "12px"
    fontWeight: 700
    lineHeight: "1.0"
    letterSpacing: "0.22em"
  price:
    fontFamily: "'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif"
    fontSize: "44px"
    fontWeight: 700
    lineHeight: "1.0"
    letterSpacing: "-0.02em"

rounded:
  sm:   "6px"
  md:   "12px"
  lg:   "20px"
  full: "9999px"

spacing:
  "0":  "0"
  "1":  "4px"
  "2":  "8px"
  "3":  "12px"
  "4":  "16px"
  "6":  "24px"
  "8":  "32px"
  "12": "48px"
  "16": "64px"
  "24": "96px"
  "32": "128px"

components:
  button-primary:
    backgroundColor: "{colors.primary-900}"
    textColor: "{colors.neutral-surface}"
    rounded: "{rounded.full}"
    padding: "0 {spacing.8}"
    height: "44px"
  button-primary-hover:
    backgroundColor: "{colors.primary-950}"
  button-secondary:
    backgroundColor: "{colors.secondary-500}"
    textColor: "{colors.neutral-surface}"
    rounded: "{rounded.full}"
    padding: "0 {spacing.8}"
    height: "44px"
  button-secondary-hover:
    backgroundColor: "{colors.secondary-950}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.primary-900}"
    rounded: "{rounded.full}"
    padding: "0 {spacing.8}"
    height: "44px"
  button-ghost-hover:
    backgroundColor: "{colors.primary-50}"
  button-large:
    height: "56px"
    padding: "0 {spacing.12}"
  card:
    backgroundColor: "{colors.neutral-surface}"
    rounded: "{rounded.lg}"
  card-hover:
    backgroundColor: "{colors.neutral-surface}"
    rounded: "{rounded.lg}"
  plan-featured:
    backgroundColor: "{colors.neutral-surface}"
    rounded: "{rounded.lg}"
  ticket-mock:
    backgroundColor: "{colors.neutral-surface}"
    rounded: "22px"
  buybar:
    backgroundColor: "{colors.neutral-surface}"
    height: "84px"
---

# Overview

このLPは「神戸の洗練と開放感」を体感させるためのものです。**Harbor Breeze** というデザイン哲学を軸に、スクロールするたびに海風を感じるようなホワイトスペースと余白感を重視してください。

- 深い紺青（`primary-950`）と清涼感のある白（`neutral-surface`）のコントラストが骨格
- ピンク（`secondary-500`）はアクセントとして使用し、主張しすぎない
- 行間 `1.8` を基本とし、日本語テキストの美しさと可読性を確保する

**感情的な目標：** チケットを購入した瞬間に「神戸に行きたい」という期待感が生まれること。

# Colors

## Primary — Harbor Blue

神戸の深海と広大な空を象徴する青。11段階のスケールで構成される。

| Token | Hex | 用途 |
|---|---|---|
| `primary-950` | `#0A2558` | Hero背景・フッター・メインCTA |
| `primary-900` | `#0D47A1` | ボタン・見出し強調 |
| `primary-500` | `#2196F3` | 装飾・グラデーション中間色 |
| `primary-200` | `#90CAF9` | Hero内サブテキスト |
| `primary-50`  | `#E3F2FD` | カード背景・ホバー状態 |

## Secondary — Stylish Pink

スイーツ・華やかさ・港町のモダンなアクセント。控えめに使うことで視線を誘導する。

| Token | Hex | 用途 |
|---|---|---|
| `secondary-500` | `#E91E63` | CTAボタン・アイキャッチ・eyebrow |
| `secondary-950` | `#880E4F` | ホバー状態 |
| `secondary-50`  | `#FCE4EC` | 背景アクセント |

## Neutrals

| Token | Hex | 用途 |
|---|---|---|
| `neutral-canvas`    | `#F8FAFC` | ページ背景 |
| `neutral-surface`   | `#FFFFFF` | カード・ヘッダー |
| `neutral-ink`       | `#0F172A` | 本文テキスト |
| `neutral-ink-muted` | `#475569` | サブテキスト・ラベル |
| `neutral-rule`      | `#E2E8F0` | ボーダー・区切り線 |

# Typography

フォントスタック：`'Helvetica Neue', 'Arial', 'Hiragino Kaku Gothic ProN', sans-serif`

行間は基本 `1.8` で日本語を読みやすく。見出しは `1.15〜1.4` でコンパクトに引き締める。

| Token | Size | Weight | lineHeight | 用途 |
|---|---|---|---|---|
| `display` | 72px (clamp 40〜72) | 700 | 1.15 | Hero H1 |
| `heading-2` | 44px (clamp 28〜44) | 700 | 1.3 | セクション見出し |
| `heading-3` | 24px | 700 | 1.4 | カード見出し |
| `heading-4` | 17px | 700 | 1.4 | ステップ・FAQ見出し |
| `lead` | 17px | 400 | 1.8 | Hero リード文 |
| `base` | 16px | 400 | 1.8 | 本文 |
| `small` | 14px | 400 | 1.8 | カード本文・説明文 |
| `caption` | 12px | 700 | 1.0 | Eyebrow・ラベル |
| `price` | 44px | 700 | 1.0 | 料金表示 |

# Layout

## Grid

- コンテナ最大幅：`1180px`、左右パディング：`spacing.6 (24px)`
- 12カラムグリッド（エリアセクションで使用）
- カラムガップ：`spacing.6 (24px)`

## Section Spacing

すべての主要セクションは `padding-block: spacing.24 (96px)` 以上を確保すること。これが Harbor Breeze の「海風感」を生むホワイトスペースの最小値。

## Mobile

- ブレークポイント：`880px`（グリッドはシングルカラムに切り替え）
- モバイルナビは非表示。代わりに `buybar` コンポーネントを bottom に固定表示

# Elevation & Depth

シャドウは「浮遊感」ではなく「接地感」のある控えめな表現にとどめる。

| 名称 | 値 | 用途 |
|---|---|---|
| `shadow-card` | `0 4px 20px rgba(0,0,0,0.10)` | カード・チケットモック |
| `shadow-card-hover` | `0 12px 36px rgba(13,71,161,0.18)` | カードホバー時 |
| `shadow-hero-ticket` | `0 30px 80px rgba(0,0,0,0.45)` | Heroのチケットモック |

Hero背景のグラデーションレイヤー（Harbor Blue + Stylish Pink の radial-gradient）は depth を演出するが、テキスト可読性を損なわないよう `rgba` で制御すること。

# Shapes

角丸はコンポーネントの「柔らかさ」を統一する。

| Token | 値 | 用途 |
|---|---|---|
| `rounded.sm` | 6px | 小さいバッジ・アイコン装飾 |
| `rounded.md` | 12px | 中サイズUI要素 |
| `rounded.lg` | 20px | カード・エリアカード・CTA Strip |
| `rounded.full` | 9999px | ボタン・バッジ・ドット |

チケットモックのみ例外的に `22px` を使用（実物チケットの物理的な角丸を再現）。

# Components

## Button

最小タップターゲット `44px`（a11y 要件）を厳守。

- `button-primary` — Header/CTA用。背景 `primary-900`
- `button-secondary` — メインCTA。背景 `secondary-500`（ピンク）
- `button-ghost` — サブアクション。透明背景 + ボーダー
- `button-large` — Hero・CTA Strip用の大型バリアント（`height: 56px`）

## Card

`shadow-card` を常に適用。hover時は `shadow-card-hover` + `translateY(-2px)` で浮遊感。

要素構成：`card__header` / `card__body` / `card__footer`（border-top区切り）

## Ticket Mock

Hero右カラムのビジュアル要素。`rotate(-3deg)` で傾けて「手に持つ感」を表現。

実画像は `images/ticket-preview.png` に差し替え可能（現在はプレースホルダー）。

## Buybar（モバイル限定）

`≤760px` でのみ表示される固定購入バー。`env(safe-area-inset-bottom)` で iPhone のホームバー領域を考慮。

## Asset Paths

```
images/hero-harbor-view.jpg   — Hero・エリアAREA01
images/kitano-area.jpg        — AREA02 北野
images/nankin-machi.jpg       — AREA03 南京町
images/rokko-night-view.jpg   — AREA04 六甲
images/sweets-cafe.jpg        — AREA05 スイーツ
```

# Do's and Don'ts

## Do

- `primary-950` と `neutral-surface` の高コントラストコンビを軸に使う
- セクション間のホワイトスペースは `spacing.24 (96px)` を下限とする
- 日本語テキストの `line-height` は常に `1.8`
- ボタンは最小 `44px` のタップターゲットを確保する
- CSS Custom Properties（`--color-primary-950` 等）でトークンを実装する
- BEM命名規則（`c-button`, `c-button--primary`）を厳守する

## Don't

- `secondary-500`（ピンク）を広い面積の背景には使わない（視覚的にうるさくなる）
- 外部ライブラリ・フレームワーク（React, Tailwind 等）は使用しない
- `primary-950` 背景上で `neutral-ink` テキストは使わない（コントラスト不足）
- カードの `shadow-card` を省略しない（フラットになりすぎる）
- Hero内の `ghost` ボタンに通常の `primary-200` ボーダーは使わない（`rgba(255,255,255,0.4)` を使う）
