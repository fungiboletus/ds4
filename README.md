Some fork of "DwarftStar", some inference engine for DeepSeek V4 Flash.

*Changes:*

- Wired HTTP disconnect detection into the existing cooperative cancellation system, addressing [issue #333](https://github.com/antirez/ds4/issues/333).
- Stops non-streaming generation when the client disappears.
- Ported OpenAI tool-call continuation from [PR #611](https://github.com/antirez/ds4/pull/611).
- Ported transient metadata KV reuse from [PR #378](https://github.com/antirez/ds4/pull/378).
- Added regression tests for disconnect detection and both KV improvements.
