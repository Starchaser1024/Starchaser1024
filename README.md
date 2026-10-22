<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=30&pause=1200&color=58A6FF&center=true&vCenter=true&width=420&lines=starchaser">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=30&pause=1200&color=0969DA&center=true&vCenter=true&width=420&lines=starchaser" alt="starchaser">
  </picture>
</p>

<p align="center"><sub>MSc CS @ BJUT · ECG signals × LLMs × agents</sub></p>

<table>
  <tr>
    <td width="54%" align="center">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=Starchaser1024&show_icons=true&hide=stars&theme=github_dark&hide_border=true&cache_seconds=1800">
        <img width="100%" src="https://github-readme-stats.vercel.app/api?username=Starchaser1024&show_icons=true&hide=stars&theme=default&hide_border=true&cache_seconds=1800" alt="GitHub stats">
      </picture>
    </td>
    <td width="42%" align="center">
      <picture>
        <source media="(prefers-color-scheme: dark)" srcset="assets/top-langs-dark.svg?v=1">
        <img width="100%" src="assets/top-langs-light.svg?v=1" alt="Most used languages">
      </picture>
    </td>
  </tr>
</table>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-act-graph.rodriaum.com/graph?username=Starchaser1024&theme=github-dark&hide_border=true&area=true">
    <img width="100%" src="https://github-act-graph.rodriaum.com/graph?username=Starchaser1024&theme=github-compact&hide_border=true&area=true" alt="Contribution activity over the last 31 days">
  </picture>
</p>

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

<p align="center">
  <img src="https://hits.sh/github.com/Starchaser1024.svg?label=Profile%20views&color=0969DA" alt="Profile views">
</p>
