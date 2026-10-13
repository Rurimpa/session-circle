# Session Circle

Let two or three running Claude Code sessions think through one question together, with this session as the facilitator.

When you run several Claude Code sessions for different parts of your work, some decisions need what each of them knows. Asking them one by one gives you separate answers that never meet. A circle connects them with SendMessage and runs the discussion in a fixed order:

- **Skeleton first.** The facilitator sends what must be decided, where the paths split, and the holes not yet filled — not a finished proposal. A finished proposal makes everyone hunt for flaws; a skeleton makes them fill holes.
- **Views are light, the closing word is heavy.** Views can be sent any number of times with no format. Each session gives one closing word on the final proposal.
- **The facilitator never rules or recommends.** It lays out agreements, disagreements, and what nobody checked.
- **You stay in charge.** The facilitator reports to you after every stage and waits for your OK before closing.

## How to use

1. Say what you want decided and which sessions to invite.
   - Example: `open a circle with docs-work and api-work about how we name the new endpoints`
2. This session checks, for each invited session, whether the circle really needs it (only that session holds the files or logs), and sends the skeleton.
3. You get a short report after each stage.
   - Example: `Stage 2 done: both sessions agree on the prefix; they disagree on plural names. Next: revise the skeleton.`
4. At the end you get the layout and are asked whether the circle may close.
   - Example: `Both sessions agree on the prefix; one still prefers singular names. Nobody checked the old clients. May I close the circle?`

## What it runs, stores, and sends

- **Runs:** one skill (`session-circle`). No hooks, no scripts.
- **Stores:** the facilitator writes each round's replies to a Markdown file in your working folder, word for word, so they are not lost when a session closes.
- **Sends:** messages between sessions on your computer with Claude Code's SendMessage. Nothing over the network.

## Known limitations

- Needs Claude Code sessions that are already running on the same machine and can be reached with SendMessage.
- Up to three invited sessions by default. For four or more, the facilitator asks you first.
- It is a procedure, not a lock: nothing stops a session from breaking the order.

## 日本語

動いている Claude Code の席（会話）を2つか3つ集めて、1つの問いを一緒に考えさせるスキルです。開いた席が進め役になります。

- 最初に配るのは、出来上がった案ではなく骨格です（決めたいこと・分かれ目・まだ埋まっていない穴）。
- 意見は形式なしで何度でも集め、骨格を直してから案にします。最後に各席から一言ずつもらいます。
- 進め役は裁かず、おすすめもしません。合意点・相違点・誰も確かめていないことを並べます。
- 段ごとに、頼んだ人へ結果を報告します。閉じる前に、頼んだ人の OK を待ちます。
- 各回の返事は、言葉どおりに作業フォルダのファイルへ写します。席が閉じても消えません。
- 同じパソコンの上で動いていて、SendMessage で届く席だけを呼べます。
- 呼ぶ席は3つまでです。4つ以上のときは、進め役が先にあなたに聞きます。
- 決まった順番で進める手順で、鍵ではありません。席が順番を破っても止める仕組みはありません。
- インターネットへは何も送りません。動くのは Claude Code の中だけです。

## Questions and issues

Issues are welcome, but replies are not guaranteed. The author may answer in their own words, or may not answer at all.

GitHub の issue（質問・不具合の知らせ）は歓迎しますが、返事をお約束はできません。作者が自分の言葉で返事をすることもあれば、返事をしないこともあります。

## Author

Author: Rurimpa

## License

MIT. See `LICENSE`.
