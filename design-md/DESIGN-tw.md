---
spec: google-labs-design-md/v1
version: 1.2.0
framework: tailwind-css
config:
  prefix: ""
  strategy: class

# 1. DESIGN TOKENS (Machine Readable)
tokens:
  colors:
    brand:
      primary: { hex: "#3B82F6", tailwind: "blue-500" }
      secondary: { hex: "#10B981", tailwind: "emerald-500" }
    functional:
      success: { hex: "#22C55E", tailwind: "green-500" }
      error: { hex: "#EF4444", tailwind: "red-500" }
      warning: { hex: "#F59E0B", tailwind: "amber-500" }
    neutral:
      surface: "#FFFFFF"
      canvas: "#F9FAFB" # gray-50
      border: "#E5E7EB" # gray-200
      text-main: "#111827" # gray-900
      text-muted: "#6B7280" # gray-500

  spacing:
    base: 4px
    scale:
      none: 0
      xs: 4px    # tailwind: 1
      sm: 8px    # tailwind: 2
      md: 16px   # tailwind: 4
      lg: 24px   # tailwind: 6
      xl: 32px   # tailwind: 8
      "2xl": 48px # tailwind: 12

  typography:
    families:
      sans: "Inter, system-ui, sans-serif"
      mono: "JetBrains Mono, monospace"
    weights:
      normal: 400
      medium: 500
      bold: 700

  shadows:
    sm: "0 1px 2px 0 rgb(0 0 0 / 0.05)"
    md: "0 4px 6px -1px rgb(0 0 0 / 0.1)"
---

# Design System Specification

## 1. Intent & Principles
本プロジェクトは、効率的でアクセシブルな管理画面の構築を目的とする。
- **Predictability:** 全てのコンポーネントは Tailwind の基本スケールに従う。
- **AI-Native:** コード生成AIがこのドキュメントを唯一の参照元（SSOT）として扱う。

## 2. Foundations
すべての要素は `tokens` セクションに定義された数値を使用すること。
独自の16進数（HEX）を直接コードに記述することは禁止し、必ず Tailwind Config 経由のクラス名を使用する。

## 3. Components

### [Button]
標準的なアクション要素。

**Structure:**
- `<button class="inline-flex items-center justify-center transition-all ...">`
- Icon: 左側に配置、`w-5 h-5` を標準とする。

**Variants:**
| Variant | Tailwind Classes | Usage |
| :--- | :--- | :--- |
| **Primary** | `bg-brand-primary text-white hover:bg-blue-600 shadow-sm` | 主要なアクション |
| **Secondary** | `bg-white border border-neutral-border text-neutral-text-main hover:bg-gray-50` | 補助的なアクション |
| **Ghost** | `text-neutral-text-muted hover:bg-gray-100 hover:text-neutral-text-main` | 低優先度のアクション |

**States:**
- **Disabled:** `opacity-50 cursor-not-allowed`
- **Loading:** `.animate-spin` を持つアイコンを表示し、テキストは維持する。
- **Focus:** `outline-none ring-2 ring-brand-primary ring-offset-2`

---

### [Card]
コンテンツをグループ化する基本コンテナ。

**Structure:**
- Container: `<div class="bg-neutral-surface border border-neutral-border rounded-xl shadow-sm overflow-hidden">`
- Header: `border-b border-neutral-border p-md`
- Body: `p-md`
- Footer: `bg-neutral-canvas border-t border-neutral-border p-md flex justify-end gap-sm`

**Interaction:**
- `is-clickable` クラスが付与された場合、`hover:shadow-md hover:border-brand-primary transition-shadow cursor-pointer` を適用する。

---

## 4. Patterns & Layouts

### Data Entry
- フォームラベルは `text-sm font-medium text-neutral-text-main` を使用し、常にインプットの上に配置する。
- エラーメッセージは `text-xs text-functional-error mt-xs` で表示する。

### Feedback Loop
- 成功時のトースト通知は `bg-functional-success` を用い、5秒後に自動消滅する。

## 5. Accessibility (A11y)
- **Contrast:** `text-main` と `surface` のコントラスト比を 7:1 以上に保つ。
- **Focus:** すべてのインタラクティブ要素には視覚的なフォーカスインジケータを必須とする。

## 6. Engineering & Sync Workflow
1. **Figma to Code:** デザイナーが Figma Variables を変更した場合、`Figma MCP` を使用して `tokens` セクションを自動更新する。
2. **Code to Preview:** `DESIGN.md` の変更後、Claude Code は `tailwind.config.js` を生成・更新し、Storybook や開発環境に反映させる。