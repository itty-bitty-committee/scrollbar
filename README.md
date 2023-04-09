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

Submit separate pull requests per domain with style modifications in the
following syntax using customizable variables whenever possible:

```css
/* ==UserStyle==
@preprocessor [processor]
@var [type] [name] [label] [value]
==/UserStyle== */
@-moz-document domain("[domain]") {
  /* [affects] */
  [selector][identifier] {
    [property]: [name] !important;
  }
}
```

| Input      | Description                                                                                                                          |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| processor  | Compatible style preprocessor ([default, uso, less, stylus](https://github.com/openstyles/stylus/wiki/Writing-UserCSS#preprocessor)) |
| type       | Value type ([text, color, checkbox, select, range, number](https://github.com/openstyles/stylus/wiki/Writing-UserCSS#type))          |
| name       | Name to reference formatted as `[domain name]_[component]_[css property]`                                                            |
| label      | Settings menu title formatted as `"[Component]: [CSS Property]"`                                                                     |
| value      | Default improvement value                                                                                                            |
| domain     | Domain name to apply styles                                                                                                          |
| affects    | Describes what the block changes                                                                                                     |
| selector   | CSS selector (., #, etc.)                                                                                                            |
| identifier | CSS selector name to modify                                                                                                          |
| property   | CSS property to modify                                                                                                               |

#### Example

```css
/* ==UserStyle==
@preprocessor stylus
@var text twitch_scrollbar_width "Scrollbar: Width" 13px
==/UserStyle== */
@-moz-document domain("twitch.tv") {
  /* width */
  .simplebar-scrollbar {
    width: twitch_scrollbar_width !important;
  }
}
```

### Compatibility

If running into issues with variable usage due to preprocessor compatibility,
hardcoded values may be used.

#### Example

```css
/* ==UserStyle==
@preprocessor default
==/UserStyle== */
@-moz-document domain("discord.com") {
  /* width */
  .messagesWrapper-RpOMA3 ::-webkit-scrollbar {
    width: 19px !important;
  }
  /* color */
  #app-mount {
    --scrollbar-auto-thumb: #b5bac1 !important;
  }
}
```

### Resources

[Writing UserCSS](https://github.com/openstyles/stylus/wiki/Writing-UserCSS#type)
