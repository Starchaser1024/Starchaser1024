<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/type-dark.png">
    <source media="(prefers-color-scheme: light)" srcset="assets/type-light.png">
    <img src="assets/type-light.png" alt="Starchaser — ECG signals and large models, set above a thin ECG trace." width="100%">
  </picture>
</p>

I'm a master's student in Computer Science at Beijing University of Technology. My work
lives on the seam between signal processing and large models — a heartbeat is a waveform
with a frequency, a rhythm, a story, and I want a model that can hold all three at once.

I came from the time domain and I'm moving toward the frequency domain: from hand-built
features toward models that learn their own. I don't think the old craft becomes obsolete.
I think it becomes the vocabulary.

## Open source

Four upstream pull requests. Each is one bug fixed at its source, pinned down by a test.

<table>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/langroid/langroid/pull/1124"><b>langroid#1124</b></a></td>
    <td><code>TaskConfig</code> was a mutable default shared by every <code>Task</code>; each task now gets its own.</td>
  </tr>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/bytedance/deer-flow/pull/7140"><b>deer-flow#7140</b></a></td>
    <td>An unusable credential source ended the whole lookup instead of falling through.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/agentscope-ai/agentscope/pull/3382"><b>agentscope#3382</b></a></td>
    <td><code>RedisStorage.upsert_channel</code> let a second channel take over an existing platform bot id.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/NousResearch/hermes-agent/pull/141881"><b>hermes-agent#141881</b></a></td>
    <td>File version was built from content, so a Windows overwrite could look stale. Now it is built from the path.</td>
  </tr>
</table>

Also [wechat-antirevoke-linux](https://github.com/Starchaser1024/wechat-antirevoke-linux) — an
ELF binary patch for WeChat on Linux, with backup, verification and rollback.

## Now

- **Agents** — systems that reason, act, and stay accountable to the people who use them.
- **ECG** — time-domain signals and frequency-domain representations in one model.
- **Review tooling** — making AI-generated changes something you can accept or reject.
