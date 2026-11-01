# Paperform for Claude

Build forms, run workflows and get documents signed from Claude. This plugin connects Claude to your Paperform account and adds skills that show Claude how to use Paperform, Stepper and Papersign together.

## What you can ask for

- **Forms (Paperform).** Describe the form you need, or share a PDF or a list of questions, and Claude drafts it in your account. Refine the questions and layout together, then publish it when you're happy. Claude can also find your existing forms and summarise their responses.
- **Workflows (Stepper).** Ask Claude to act on new submissions or other triggers: add a row to Google Sheets, send an email, update your CRM. Claude builds the workflow, tests each step against your connected apps and explains what happened when a run fails.
- **Signatures (Papersign).** Pick a template, tell Claude who signs and what to fill in, and it prepares the document and sends it once you confirm.

Try:

- "Make a client intake form, add new clients to my Google Sheet, and send each one our engagement letter to sign."
- "Summarise this week's responses to the customer feedback form."
- "Turn this PDF into an online form I can share."

## Skills

| Skill | Use it to |
| --- | --- |
| `build-a-form` | Build a form from a description and publish it |
| `document-to-form` | Turn a PDF, document or pasted questions into a form |
| `event-registration-with-payment` | Build a registration form that takes payment |
| `build-a-workflow` | Build, test and publish a Stepper workflow |
| `send-for-signature` | Prepare a Papersign document and send it for signature |
| `summarise-responses` | Summarise a form's responses with real counts |
| `client-onboarding` | Set up an intake form, a workflow and a signed agreement together |

## How it works

The plugin contains skills (Markdown instructions) and one remote MCP connector, `https://api.paperform.app/mcp`. It runs no code on your computer and has no hooks, scripts or local servers.

When you connect, you sign in with your Paperform account (or create one) through Paperform's own sign-in page, and choose what Claude may do. Claude then works only in the account and spaces you approved. Requests go from Claude to Paperform's server over HTTPS; the plugin sends data nowhere else. Anything that publishes, sends or deletes asks you first.

You can disconnect at any time from Claude's connector settings.

## Links

- About the connector: https://paperform.com/mcp/
- Help: https://paperform.com/help/
- Privacy policy: https://paperform.com/privacy/
- Terms: https://paperform.com/terms/

## Licence

MIT. See [LICENSE](LICENSE).
