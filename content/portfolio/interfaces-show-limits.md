+++
title = "Interfaces should explain their own limits"
slug = "interfaces-should-show-their-limits"
url = "/ideas/interfaces-should-show-their-limits/"
description = "An interface should show when information is missing, uncertain, delayed, or outside its scope."
image = "images/interface-limits.svg"
image_alt = "An interface panel that marks missing information and offers a clear next action."
weight = 2
+++
This essay argues that an interface should explain uncertainty and boundaries where people make decisions. A quiet panel can mean that no results exist, a request failed, or the system has not finished. Those states need different responses.

## Name the state

Tell people whether information is current, incomplete, unavailable, or estimated. Show a time or source when it helps them judge freshness. Distinguish a true zero from information that could not load.

## Give a useful next step

When something fails, explain what the person can do next. They might retry, change a filter, reconnect, or ask an administrator for access. When the system cannot offer a safe action, say what remains unknown.

## Avoid false certainty

Do not make an estimate look exact. Do not hide a partial result behind a complete-looking screen. Use plain language for limits, then keep the detail near the control or result that it affects.

This does not require every screen to explain every technical detail. It requires the interface to expose limits that can change a choice. Clear states help people decide when to continue, when to wait, and when to verify another source.
