# PorchLyte AI Agent Hub

The Claude plugin for PorchLyte members: Voice, Brand, Local, and the nine-agent team, wired to your PorchLyte account so Claude reads and writes your real Foundations instead of chat memory.

This replaces the two older marketplaces (`porchlyte-foundations` and `porchlyte-agents`). One plugin now covers everything they did.

## Install

In the Claude desktop app:

1. Open **Customize** in the left sidebar, go to **Plugins**, click **Add**, then **Add marketplace**, then **Add from a repository**.
2. Paste this and sync:

   ```
   PorchLyte/porchlyte-ai-agent-hub
   ```

3. Find **porchlyte-ai-agent-hub** in the synced marketplace and click **+** to install.

Then add the connector so your agents can reach your account. **Settings → Connectors → Add custom connector**, paste:

```
https://aiagents.porchlyte.com/api/mcp/mcp
```

Click Connect and sign in with your PorchLyte membership email. Full walkthrough, including migrating an older setup: <https://aiagents.porchlyte.com/connect-and-migrate.html>

## Updates

Click the **···** next to the **porchlyte-ai-agent-hub** marketplace under **Customize > Plugins** and choose **Update**. Your Voice, Brand, Local, and hired agents live in your PorchLyte account, so updates never touch your personalization.

If an update ever seems stuck, you can delete the marketplace and install the zip instead — download it from your hub at <https://aiagents.porchlyte.com>. Both installs behave identically; only the update mechanism differs.

## Moving from the old plugins

If you previously installed `porchlyte-foundations` or `porchlyte-agents`, remove both after you've migrated. Running the old and new plugins together means two versions of the same skill can answer the same request. See the walkthrough linked above for the `/migrate` step that carries your existing setup over.

## Questions

Email tracy@porchlyte.com or visit porchlyte.com.

— Tracy

---

## Maintainers

**Do not edit `plugins/` in this repo by hand.** This repo is published from
`porchlyte-agent-platform`, where `claude-plugin/porchlyte-ai-agent-hub/` is the
single source of truth for both this marketplace and the downloadable zip.
Edit there, then run `npm run publish:marketplace` to push changes here.
Hand-editing this repo will be overwritten on the next publish.
