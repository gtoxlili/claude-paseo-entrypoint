# claude-paseo entrypoint

When installed and enabled, this plugin adds `CLAUDE_CODE_ENTRYPOINT=claude-paseo` to Claude agents each time a session opens. Other providers are unchanged.

It is a fork of [getpaseo/claude-code-entrypoint-env](https://github.com/getpaseo/claude-code-entrypoint-env), which uses the value `Paseo`. This fork names the label like the other Claude hosts, `claude-vscode` and `claude-desktop`.

This is an optional community workaround for [Claude Code issue #97074](https://github.com/anthropics/claude-code/issues/97074).

```sh
paseo plugin add git:https://github.com/gtoxlili/claude-paseo-entrypoint.git
```

Enable plugins in Paseo Settings if needed. There are no additional settings.

Only the launch environment changes. Claude Code sends the label with provider requests; the plugin makes no network requests and stores no data.
