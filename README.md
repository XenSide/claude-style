# Colleague output style for Claude Code

Install on any device:

    claude plugin marketplace add XenSide/claude-style
    claude plugin install colleague@xenside

Then make it the default: set `"outputStyle": "colleague:Colleague"` in ~/.claude/settings.json.
(`force-for-plugin` should do this automatically, but Claude Code doesn't apply it yet: anthropics/claude-code#64914.)

To change the style, edit plugins/colleague/output-styles/colleague.md, bump the version in plugin.json and push.
Devices pick it up with:

    claude plugin marketplace update xenside
    claude plugin update colleague@xenside
