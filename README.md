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
        <source media="(prefers-color-scheme: dark)" srcset="https://cdn.jsdelivr.net/gh/Starchaser1024/Starchaser1024@86feebd49742821daee6f53378cb59e049cc8dd8/assets/top-langs-dark.svg">
        <img width="100%" src="https://cdn.jsdelivr.net/gh/Starchaser1024/Starchaser1024@86feebd49742821daee6f53378cb59e049cc8dd8/assets/top-langs-light.svg" alt="Most used languages">
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

Fourteen upstream pull requests, seven merged and seven open. Each one starts from the line
that misbehaves and ends in a test that fails without the change.

<table>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/bytedance/deer-flow/pull/7569"><b>deer-flow#7569</b></a></td>
    <td><code>parse_required_secrets</code> collapsed duplicate <code>required-secrets</code> declarations by name but kept whichever came first, so an <code>optional: true</code> line ahead of a bare one made the secret optional and the skill activated without it. Required now wins regardless of order, and the export manifest reports the same thing the parser does.</td>
  </tr>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/bytedance/deer-flow/pull/7462"><b>deer-flow#7462</b></a></td>
    <td><code>LocalSandbox.write_file</code> translated container paths inside every stored file, so a dictated <code>README.md</code> held a host path while <code>read_file</code> masked the rewrite. Translation now applies only to executable content.</td>
  </tr>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/bytedance/deer-flow/pull/7140"><b>deer-flow#7140</b></a></td>
    <td>An unusable credential source ended the whole lookup instead of falling through.</td>
  </tr>
  <tr>
    <td><sub><b>MERGED</b></sub></td>
    <td><a href="https://github.com/deepset-ai/haystack/pull/13381"><b>haystack#13381</b></a></td>
    <td>Five components called <code>&lt;method&gt;_async</code> unconditionally, so a document store that implements only the synchronous protocol raised <code>AttributeError</code> from <code>run_async</code>. They now fall back to a worker thread.</td>
  </tr>
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
    <td><a href="https://github.com/langroid/langroid/pull/1124"><b>langroid#1124</b></a></td>
    <td><code>TaskConfig</code> was a mutable default shared by every <code>Task</code>; each task now gets its own.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/stanfordnlp/dspy/pull/10733"><b>dspy#10733</b></a></td>
    <td><code>ToolCalls.serialize_model</code> dumped each tool result with <code>TypeAdapter.dump_python(mode="json")</code> and no fallback, so one value pydantic cannot encode — a numpy scalar, a dataclass — took the whole stored trace with it, name and arguments included, while the same value already reached the model as its string form.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/bytedance/deer-flow/pull/7600"><b>deer-flow#7600</b></a></td>
    <td>The broad <code>use … to …</code> pattern read any phrase containing “model” as a model name, so “Use a regression model to analyze these sales figures” entered model selection and came back with the analysis method stripped from the task. A broad-form name now has to be spelled out in the visible catalog; unmatched text stays task text.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/agentscope-ai/agentscope/pull/3493"><b>agentscope#3493</b></a></td>
    <td><code>Msg.get_text_content()</code> returns <code>None</code> for a <code>SystemMsg</code> with no <code>TextBlock</code>, and six OpenAI-compatible multi-agent formatters passed that value into the system turn, so the first request of a conversation carried <code>{"role": "system", "content": null}</code> and the endpoint answered 400.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/agentscope-ai/agentscope/pull/3441"><b>agentscope#3441</b></a></td>
    <td>Tool-result truncation sized the retained prefix from the block's average token density, so a mixed-script prefix could exceed <code>tool_result_limit</code>. The prefix is now recounted and binary-searched with the same counter.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/agentscope-ai/agentscope/pull/3382"><b>agentscope#3382</b></a></td>
    <td><code>RedisStorage.upsert_channel</code> let a second channel take over a platform bot id a live record already drove. The check now happens inside the write.</td>
  </tr>
  <tr>
    <td><sub><b>OPEN</b></sub></td>
    <td><a href="https://github.com/NousResearch/hermes-agent/pull/142868"><b>hermes-agent#142868</b></a></td>
    <td>A Microsoft Store / MSIX app registers no uninstall entry and its files sit behind an unlistable <code>WindowsApps</code>, so an installed app read as missing. A new <code>msix_package</code> location kind resolves it through the AppModel repository.</td>
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

<p align="center">
  <img src="https://hits.sh/github.com/Starchaser1024.svg?label=Profile%20views&color=0969DA" alt="Profile views">
</p>
