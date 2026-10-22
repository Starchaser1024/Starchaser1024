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

Eight upstream pull requests, four merged and four open. Each one is a single defect traced
back to its source and pinned down by a test.

<table>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/agentscope-ai/agentscope/pull/3401"><b>agentscope#3401</b></a></td>
    <td><code>WordParser</code> kept blank paragraphs that carry no run but dropped the ones that still carry one — a space-only line, a <code>Shift+Enter</code> break — so the empty lines Word renders disappeared from the extracted text.</td>
  </tr>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/ayuayue/PiDeck/pull/394"><b>PiDeck#394</b></a></td>
    <td>Binding a Feishu bot to a DSH session looked the agent up in the pi-only manager, so it always answered “runtime unavailable”. It now takes the same gateway lookup the message bridges already use.</td>
  </tr>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/bytedance/deer-flow/pull/7140"><b>deer-flow#7140</b></a></td>
    <td>An unusable credential source ended the whole lookup instead of falling through.</td>
  </tr>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/langroid/langroid/pull/1124"><b>langroid#1124</b></a></td>
    <td><code>TaskConfig</code> was a mutable default shared by every <code>Task</code>; each task now gets its own.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/NousResearch/hermes-agent/pull/142868"><b>hermes-agent#142868</b></a></td>
    <td>A Microsoft Store / MSIX app registers no uninstall entry and its files sit behind an unlistable <code>WindowsApps</code>, so an installed app read as missing. A new <code>msix_package</code> location kind resolves it through the AppModel repository.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/deepset-ai/haystack/pull/13381"><b>haystack#13381</b></a></td>
    <td>Five components called <code>&lt;method&gt;_async</code> unconditionally, so a document store that implements only the synchronous protocol raised <code>AttributeError</code> from <code>run_async</code>. They now fall back to a worker thread.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/NousResearch/hermes-agent/pull/141881"><b>hermes-agent#141881</b></a></td>
    <td>File version was built from content, so a Windows overwrite could look stale. Now it is built from the path.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/agentscope-ai/agentscope/pull/3382"><b>agentscope#3382</b></a></td>
    <td><code>RedisStorage.upsert_channel</code> let a second channel take over a platform bot id a live record already drove. The check now happens inside the write.</td>
  </tr>
</table>

Also [wechat-antirevoke-linux](https://github.com/Starchaser1024/wechat-antirevoke-linux) — an
ELF binary patch for WeChat on Linux, with backup, verification and rollback.

## Now

- **Agents** — systems that reason, act, and stay accountable to the people who use them.
- **ECG** — time-domain signals and frequency-domain representations in one model.
- **Review tooling** — making AI-generated changes something you can accept or reject.
