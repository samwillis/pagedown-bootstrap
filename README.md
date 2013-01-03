# PageDown-Bootstrap (with prototype support)


This is a fork of [pagedown-bootstrap]( https://github.com/samwillis/pagedown-bootstrap) modified for use within an application that includes the [prototype](http://prototypejs.org) javascript library. 

No demo is available for this implementation at present. From a user perspective the [demo]( http://samwillis.co.uk/pagedown-bootstrap/demo/browser/demo.html) provided by [Sam Willis](https://github.com/samwillis) gives a good overview of what to expect.

## Example

````html
<head>
  <script src="//ajax.googleapis.com/ajax/libs/prototype/1.7.1/prototype.js"></script>
  <script>window.jQuery || document.write('<script src="@{'/public/js/lib/jquery-1.7.1.min.js'}"><\/script>')</script>
  <script>
    jQuery.noConflict();
  </script>

  <script src="js/bootstrap/bootstrap-transition.js"></script>
  <script src="js/bootstrap/bootstrap-tooltip.js"></script>

  <script src="js/Markdown.Converter.js"></script>
  <script src="js/Markdown.Sanitizer.js"></script>
  <script src="js/Markdown.Editor.js"></script>
</head>

...

<div class="wmd-panel">
  <div id="wmd-button-bar"></div>
    <textarea id="wmd-input"></textarea>
  </div>
  <div class="markdown-preview" id="wmd-preview"></div>
</div>

...

<script>
  (function () {
    var converter = Markdown.getSanitizingConverter();
    var editor = new Markdown.Editor(converter);
    editor.run();
  })();

  jQuery(document).ready(function($){
    $('.btn-toolbar').tooltip()
  });
</script>
````