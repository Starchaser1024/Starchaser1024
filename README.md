<div align="center">

# Starchaser

### ECG Signals × LLMs · Learning to Build Agents

[About](#about) · [Open Source](#open-source) · [Now](#now)

</div>

## About

I'm a master's student in Computer Science at Beijing University of Technology.

My work lives on the seam between two disciplines. On one side is signal processing — the older, quieter craft, where a heartbeat is a waveform with a frequency, a rhythm, a story. On the other is the age of large models, where language becomes a way of reasoning about that waveform. I am learning to hold both.

I came from the time domain and I'm moving toward the frequency domain: from hand-built features toward models that learn their own. I don't think the old craft becomes obsolete. I think it becomes the vocabulary.

## Open Source

Two merged, two open — all of them small, focused bug fixes with regression tests.

| Pull request | What it fixes |
| --- | --- |
| **[langroid#1124](https://github.com/langroid/langroid/pull/1124)** · merged | `TaskConfig` was a mutable default shared by every `Task` instance; now each task gets its own. |
| **[deer-flow#7140](https://github.com/bytedance/deer-flow/pull/7140)** · merged | An unusable credential source ended the whole lookup instead of falling through to the next one. |
| **[agentscope#3382](https://github.com/agentscope-ai/agentscope/pull/3382)** · open | `RedisStorage.upsert_channel` let a second channel take over an existing platform bot id. |
| **[hermes-agent#141881](https://github.com/NousResearch/hermes-agent/pull/141881)** · open | File version was built from content, so a Windows overwrite could look stale; now it's built from the path. |

Each one follows the same shape: find the bug, isolate it in a test, change as little as possible.

Elsewhere: **[wechat-antirevoke-linux](https://github.com/Starchaser1024/wechat-antirevoke-linux)** — an ELF binary patch for WeChat on Linux, with backup, verification and rollback.

## Now

- **Agents** — how to design systems that reason, act, and stay accountable to the people who use them.
- **ECG** — bringing time-domain signals and frequency-domain representations into the same model.
- **Review tooling** — making AI-generated changes something you can actually accept or reject.

