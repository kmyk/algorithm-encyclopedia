---
layout: entry
changelog:
  - summary: 記事作成
    authors: kimiyuki
    reviewers:
    date: 2020-01-16T00:00:00+09:00
algorithm:
  aliases: ["箱根DP", "箱根駅伝", "箱根"]
description: 区間の集合を構成するような DP であって「左端は決まったが右端はまだ決まってない区間の数」と「右端は決まったが左端はまだ決まってない区間の数」を状態とする DP のこと。
---

# 箱根駅伝 DP

箱根駅伝 DP とは、区間の集合を構成するような DP であって「左端は決まったが右端はまだ決まってない区間の数」と「右端は決まったが左端はまだ決まってない区間の数」を状態とする DP のこと。状態が何であるかに基づく DP の分類のひとつ。

## 例題

-   [AOJ 2439: 箱根駅伝](https://judge.u-aizu.ac.jp/onlinejudge/description.jsp?id=2439)<sup>[archive.org](https://web.archive.org/web/20210102030307/https://judge.u-aizu.ac.jp/onlinejudge/description.jsp?id=2439)</sup>
    -   この問題が呼称の由来である。
-   [AtCoder Beginner Contest 134: F - Permutation Oddness](https://atcoder.jp/contests/abc134/tasks/abc134_f)<sup>[archive.org](https://web.archive.org/web/20201203225527/https://atcoder.jp/contests/abc134/tasks/abc134_f)</sup>
