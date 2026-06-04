# peer-voice

A Claude skill that strips **condescending, talking-down tone** out of client-facing /
B2B copy and rewrites it in a **peer-level voice**. The Chinese name for the failure
it targets is **爹味** ("daddy tone" — sounding like you're lecturing the reader).

一个 Claude skill:把发给客户(甲方)的文案里的**"爹味"**(居高临下、评判客户、教客户做事)
去掉,改写成**平视**语气。

---

## The idea / 内核

Every condescending line secretly says **"I understand your business better than you do."**
This skill rewrites it into:

> **"You know your business best; I only know the one thing in my hands — so let's look
> at it side by side."**

每一句爹味的潜台词都是"我比你更懂你的事";这个 skill 把它改成"你的事你最懂,我只懂手里这点,我们平起平坐一起看"。

It works by five moves: **attribute the problem outward** (industry / structure, not the
reader's negligence), **leave the judgment with the reader**, **speak upward** (lift quality,
don't patch their leaks), **earn trust by track record, not by belittling them**, and
**change the subject from "you" to "we"**. Full rules in [`SKILL.md`](SKILL.md).

五个动作:①归因外部 ②判断留客户 ③向上语言 ④立信靠资历不靠贬低 ⑤主语从"你"换成"我们"。详见 [`SKILL.md`](SKILL.md)。

## When it triggers / 何时触发

Writing or editing a sales deck, proposal, pre-sales doc (售前), kickoff / leave-behind,
cold email, or any customer-facing memo — and you want it to not sound preachy, arrogant,
or like you're grading the customer. Just ask Claude to "remove the 爹味 / make this
peer-level / stop lecturing the client".

写或改售前方案、提案、商务沟通、客户邮件时,让它别说教、别打分。直接说"去爹味 / 改平视一点"即可。

## Example / 例子

> ❌ 判断不一致 = 法务暴露 + 财务漏损,你一直在漏钱。
> ✅ 口径越统一,法务和财务越省心。

More worked rewrites: [`references/examples.md`](references/examples.md).
Trigger-word scanner: [`references/trigger-words.md`](references/trigger-words.md).

## Install / 安装

Drop the folder into your Claude skills directory:

```bash
git clone https://github.com/lucyliufromchina-cpu/peer-voice.git ~/.claude/skills/peer-voice
```

Then Claude can invoke it whenever you work on client-facing copy.
之后 Claude 在处理客户面文案时即可调用。

## Scope / 适用范围

Tuned for Chinese B2B / vendor-to-client writing. The **principle is universal**; the
trigger list and examples are Chinese-specific — for other languages, keep the five moves
and the self-check ruler, rebuild the trigger list.

为中文 B2B 文案调校;内核普适,触发词表与例子针对中文。

## 致谢 / Credits

本技能的「平视 / 去爹味」内核,蒸馏自 [weihu.xie](https://github.com/weihuxie) 的沟通方式与表达智慧。谨此致谢。

The peer-voice kernel of this skill was distilled from the communication style and
wisdom of [weihu.xie](https://github.com/weihuxie). With gratitude.

## License

MIT — see [`LICENSE`](LICENSE).
