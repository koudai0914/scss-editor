Download [Sass](http://rubyforge.org/frs/?group_id=9702&release_id=46747)
and set global options.

<img src='http://scss-editor.googlecode.com/svn/images/options.png'>


If you want to override these options for a given file, you can use the new docblock format at the top of your file. For example:<br>
<br>
<pre><code><br>
/**<br>
<br>
* @outputStyle compressed<br>
* @debugInfo true<br>
* @lineComments true<br>
*/<br>
<br>
body {<br>
/* etc... */<br>
}<br>
</code></pre>

Also, you can specify the output path for the CSS, using the <code>@outputFile</code> tag:<br>
<br>
<pre><code><br>
/**<br>
<br>
* @outputFile ../www/css/stylesheet.css<br>
* @outputStyle compressed<br>
*/<br>
</code></pre>

The path can be relative to the SCSS file, or absolute to the project path. For instance, if the project path is <b>/home/user/myproject/</b> and the <code>@outputPath</code> is <b>/stylesheet.css</b>, the stylesheet will be created at <b>/home/user/myproject/stylesheet.css</b>.