# talkative package reference

Written by every talkative release from the app itself. Do not edit by hand.

## Sound events

| Event | Plays when | Longest file |
| --- | --- | --- |
| `mute` | you mute your microphone | 10 s |
| `unmute` | you unmute your microphone | 10 s |
| `deafen` | you deafen yourself | 10 s |
| `undeafen` | you undeafen yourself | 10 s |
| `camera-on` | your camera turns on | 10 s |
| `camera-off` | your camera turns off | 10 s |
| `stream-watch` | you start watching a stream | 10 s |
| `stream-viewer-join` | someone starts watching your stream | 10 s |
| `stream-viewer-leave` | someone stops watching your stream | 10 s |
| `ring-out` | you call someone and it rings | no limit |
| `ring-in` | someone calls you | no limit |
| `channel-join` | someone joins the voice channel you are in | 10 s |
| `channel-leave` | someone leaves the voice channel you are in | 10 s |
| `self-join` | you join a voice channel or call | 10 s |
| `self-leave` | you leave a voice channel or call | 10 s |
| `stream-start` | you start streaming | 10 s |
| `stream-end` | you stop streaming | 10 s |
| `call-end` | the call you are in ends | 10 s |
| `call-declined` | the person you called declines | 10 s |
| `connection-lost` | the call connection drops | 10 s |
| `connection-back` | the call connection returns | 10 s |
| `message` | a message arrives | 10 s |
| `mention` | someone mentions you | 10 s |
| `direct-message` | a direct message arrives | 10 s |
| `message-sent` | you send a message | 10 s |
| `app-start` | the app starts | 10 s |
| `welcome` | the sign-in screen opens into the app | 10 s |
| `click` | anything clickable, and buttons when the pack has no button-click | 1 s |
| `button-click` | a button is clicked | 1 s |

## Parts

Select them as `[data-part='composer']`.

| Part | Marks |
| --- | --- |
| `window-header` | the bar at the top of the window |
| `window-control` | the minimise, maximise and close buttons |
| `navigation` | the rail of servers and places |
| `place-switch` | the control that switches between places |
| `channel-list` | the channels of a server |
| `channel-row` | one channel in the list |
| `voice-members` | the people inside a voice channel |
| `member-list` | the members of a server |
| `user-panel` | your name, status and call controls under the sidebar |
| `message` | one message |
| `mention` | a mention inside a message |
| `composer` | the box where you write a message |
| `avatar` | the picture of a person |
| `presence-dot` | the status dot of a person |
| `menu` | menus and popovers |
| `dialog` | dialogs |
| `button-primary` | the main button of a dialog or form |
| `field` | a text field |
| `segmented` | a row of choices where one is picked |
| `segmented-option` | one choice in a segmented row; the picked one has data-state="checked" |
| `segmented-highlight` | the highlight that slides behind the picked choice |

## Attributes on the root element

| Attribute | Values | Meaning |
| --- | --- | --- |
| `data-theme` | `dark`, `light` | the mode in use |
| `data-tint` | `servers`, `talk`, `events` | the place the app is in; on any element it sets the hue of --color-accent inside it |
| `data-motion` | `reduced` | set when the person asks for less motion |
| `data-performance` | `on` | set in performance mode |

## Tokens

CSS variables a theme may override. Light shows the value of `data-theme='light'` when it differs.

| Token | Dark | Light |
| --- | --- | --- |
| `--color-canvas` | `#08090d` | `#e4e3ec` |
| `--color-surface` | `#101118` | `#f7f6fa` |
| `--color-raised` | `#161821` | `#ffffff` |
| `--color-field` | `#15161f` | `#eeedf4` |
| `--color-tray` | `#12131b` | `#efeef5` |
| `--color-line` | `rgb(255 255 255 / 0.07)` | `rgb(28 30 60 / 0.09)` |
| `--color-edge` | `rgb(255 255 255 / 0.14)` | `rgb(255 255 255 / 0.9)` |
| `--color-ink-strong` | `#f3f4f9` | `#1b1c2a` |
| `--color-ink` | `#d0d2e0` | `#3e4057` |
| `--color-ink-muted` | `#b0b3c8` | `#5a5c73` |
| `--color-ink-faint` | `#8487a0` | `#6c6e86` |
| `--color-ink-disabled` | `rgb(132 135 160 / 0.6)` | `rgb(108 110 134 / 0.6)` |
| `--color-hover` | `rgb(190 184 255 / 0.07)` | `rgb(28 30 60 / 0.06)` |
| `--color-selected` | `rgb(190 184 255 / 0.11)` | `rgb(28 30 60 / 0.1)` |
| `--color-accent` | `var(--color-tint)` | same |
| `--color-servers` | `var(--tint-servers)` | same |
| `--color-talk` | `var(--tint-talk)` | same |
| `--color-events` | `var(--tint-events)` | same |
| `--color-danger` | `#ef6b6b` | `#d13438` |
| `--color-warning` | `#e2b33c` | `#9a6212` |
| `--color-scrim` | `rgb(5 6 12 / 0.6)` | `rgb(30 30 60 / 0.25)` |
| `--color-on-accent` | `#ffffff` | same |
| `--elevation-sm` | `0 10px 30px -16px rgb(6 5 24 / 0.6), inset 0 1px 0 rgb(255 255 255 / 0.04)` | `0 1px 2px rgb(30 30 70 / 0.05), 0 10px 28px -16px rgb(30 30 70 / 0.22)` |
| `--elevation-md` | `0 12px 30px -12px rgb(6 5 24 / 0.65)` | `0 10px 28px -12px rgb(30 30 70 / 0.25)` |
| `--elevation-field` | `0 12px 30px -12px rgb(6 5 24 / 0.65)` | `0 1px 2px rgb(30 30 70 / 0.06)` |
| `--elevation-lg` | `0 24px 60px -16px rgb(6 5 24 / 0.7)` | `0 24px 60px -16px rgb(30 30 70 / 0.3)` |
| `--elevation-tray` | `inset 0 2px 6px -2px rgb(0 0 0 / 0.45), inset 0 1px 0 rgb(255 255 255 / 0.07)` | `inset 0 2px 6px -2px rgb(30 30 70 / 0.12), inset 0 1px 0 rgb(28 30 60 / 0.09)` |
| `--elevation-key` | `inset 0 1px 0 rgb(255 255 255 / 0.07), inset 0 -2px 0 rgb(6 5 24 / 0.35), 0 1px 2px rgb(6 5 24 / 0.35)` | `inset 0 -2px 0 rgb(30 30 70 / 0.1), 0 1px 2px rgb(30 30 70 / 0.12)` |
| `--color-tint` | `var(--tint-servers)` | same |
| `--tint-servers` | `#8a7fdb` | same |
| `--tint-talk` | `#46b57a` | `#2fa066` |
| `--tint-events-base` | `#4a8be0` | `#2f6fd0` |
| `--tint-events` | `var(--tint-events-base)` | same |
