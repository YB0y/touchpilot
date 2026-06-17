---
id: messages
title: Messages
description: Draft and review SMS or messaging actions with explicit user approval before sending.
risk: high
aliases:
  - messages
  - sms
  - text message
  - messaging
  - draft a text
  - write a message
  - send a text
allowed_tools:
  - observe_screen_context
  - open_app
  - tap
  - long_press
  - type_text
  - clear_text
  - dismiss_keyboard
  - scroll
  - swipe
  - press_back
  - wait_for_idle
  - wait_for_app
success_criteria:
  - The message draft is visible in the compose field.
  - The recipient and message body are visible before any send action is considered.
  - The agent stops before sending unless the user gives explicit approval at the approval prompt.
examples:
  - draft a text to Alex saying I am running late
  - write a message but do not send it
  - open messages and prepare a reply
  - draft a text to Alex
  - open messages and compose a reply
  - prepare an SMS but do not send it
---

# Messages

Messaging actions are high risk. Draft messages first, keep the recipient and
body visible, and ask for user approval before sending anything.

When possible, stop after preparing the draft. Do not tap Send, Submit, or any
equivalent send control unless the user explicitly approves the policy prompt.
Do not invent recipients or message content.

Never tap send, share, or confirm buttons unless the user explicitly approves
the outgoing message content.

Allowed initial tools:

- `observe_screen_context`
- `open_app`
- `tap`
- `long_press`
- `type_text`
- `clear_text`
- `dismiss_keyboard`
- `scroll`
- `swipe`
- `press_back`
- `wait_for_idle`
- `wait_for_app`
