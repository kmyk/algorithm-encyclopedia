---
layout: entry
authors:
reviewers:
date: 2021-02-05T00:00:00+09:00
updated_at:
algorithm:
  input: パターン文字列 $P$ とテキスト文字列 $T$
  output: パターン文字列 $P$ がテキスト文字列 $T$ に含まれるかどうか。含まれるならその位置も
  time_complexity: 前処理は $O(\vert P \vert)$ である。検索は、ランダムな文字列に対しては $O(\vert T \vert / \vert P \vert)$ だが最悪ケースは $O(\vert P \vert \cdot \vert T \vert)$ である。
  space_complexity:
  aliases: []
  level: orange
description: Boyer-Moore 法は、文字列検索アルゴリズムのひとつ。どこで不一致が起きたらパターン文字列をいくつずらせばよいかの情報を $O(\vert P \vert)$ かけて構築しておき、パターン文字列をその末尾から順にテキスト文字列と照合していく。ランダムな文字列に対しては $O(\vert T \vert / \vert P \vert)$ だが、最悪ケースでは $O(\vert P \vert \cdot \vert T \vert)$ かかる。
draft: true
draft_urls: []
---

# Boyer-Moore法

## 参考文献

-   Robert S. Boyer and J. Strother Moore. 1977. A fast string searching algorithm. Commun. ACM 20, 10 (Oct. 1977), 762–772. DOI:<https://doi.org/10.1145/359842.359859>
    -   このアルゴリズムが提案された論文

## 関連項目

-   [Boyer-Moore-Horspool法](/boyer-moore-horspool)
    -   Boyer-Moore-Horspool 法は Boyer-Moore 法を簡略化したアルゴリズムである。
-   [Knuth-Morris-Pratt法](/knuth-morris-pratt)
    -   Knuth-Morris-Pratt 法は Boyer-Moore 法と並んで競技プログラミングでよく用いられる単一パターン文字列検索アルゴリズムである。

## 外部リンク

-   [boyer_moore_searcher - cpprefjp C++日本語リファレンス](https://cpprefjp.github.io/reference/functional/boyer_moore_searcher.html)
    -   C++ の標準ライブラリには Boyer-Moore 法を用いた関数オブジェクトが `std::boyer_moore_searcher` として含まれている。
