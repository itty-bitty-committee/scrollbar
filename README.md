# The _itty bitty_ Committee

#### Style modifications that improve accessibility

## Scrollbar

The Committee has denied your _itty bitty_ scrollbar!

### Requirements

Install the [stylus](https://add0n.com/stylus.html) browser extension.

[Chrome](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
| [Firefox](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)

### Installation

[Open the scrollbar style page](https://userstyles.world/style/9192/twitch-scrollbar)
and use the `install` button to add it to the stylus extension.

Alternatively, install the
[itty-bitty](https://github.com/itty-bitty-committee/itty-bitty) bundle which
includes all accessibility improvements so far.

### Customize

Use the style settings via the stylus extension to input custom modification
values

## Contributing

The Committee has invited you to submit an _itty bitty_ scrollbar violation
report.

Submit a pull request per domain with style modifications in the following
syntax using customizable variables whenever possible:

```css
/* ==UserStyle==
@var [type] [name] [label] [value]
==/UserStyle== */
@-moz-document domain("[domain]") {
  .[class] {
    [property]: [name] !important;
  }
}
```

| Input    | Description                        |
| -------- | ---------------------------------- |
| type     | Variable type (text, number, etc.) |
| name     | Variable name to reference         |
| label    | Customization menu title           |
| value    | Default value                      |
| domain   | Domain name                        |
| class    | CSS class to modify                |
| property | CSS property to modify             |

### Example

```css
/* ==UserStyle==
@var text twitch.tv "Scrollbar Width" 13px
==/UserStyle== */
@-moz-document domain("twitch.tv") {
  .simplebar-scrollbar {
    width: twitch.tv !important;
  }
}
```
