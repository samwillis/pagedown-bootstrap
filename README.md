PageDown-bootstrap with i18n and emotion support
=======================

> This is a fork of https://github.com/samwillis/pagedown-bootstrap to add i18n and emotions support

**i18n support**

Currenly the hint and the hover tooltips are seperated from Markdown.Editor.js to i18n/Markdown.i18n.LANGUAGE.js, where translations are located. Only chinese translation is complete, but you can add pretty much any language as you like. Just make sure the format looks like the i18n/Markdown.i18n.zh-cn.js file(Your pull requests are always welcome!).

Usage:

reference the translation file in your template and pass a language preference to set the editor language when you are constructing your editor in your js code

**emotions**

You have to call Markdown.SupportEmotions(imgPath,emotions) before constructing your
editor if your want it to include emotions

The demo is viewable here: http://shellfly.org/pagedown-with-emotions/demo/browser/demo.html

New icons based on http://glyphicons.com/, http://dribbble.com/shots/365544-Mini-glyphs-12-px-Free-PSD and the origional icons.
