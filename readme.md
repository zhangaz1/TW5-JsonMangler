<h2 class="tc-title">
readme.md
</h2>
</a> 9th March 2019 at 11:20pm

<div class="tc-tiddler-body tc-reveal"><h1 class=""><strong>Hello There</strong></h1><p>TW5-JsonManglerPlugin by <a class="tc-tiddlylink-external" href="https://github.com/joshuafontany" rel="noopener noreferrer" target="_blank">Joshua Fontany</a>, v 2.0.6</p><p>This plugin changes the methods tiddlywiki uses to retrieve and set values in json data tiddlers. It does so in a way that aims for <em>backwards compatibility</em>.</p><p>It introduces new features, widgets, and filter operators to manage, edit, and view json tiddlers:</p><ul><li>Allows <a class="tc-tiddlylink tc-tiddlylink-missing" href="#TextReferences">TextReferences</a> to target nested values (&quot;complex json&quot;).</li><li>An automatic <strong>alert</strong> when calling actions on an invalid json data tiddler, or when plugin tiddlers have been edited.</li><li>New buttons in the <strong>editTemplate</strong> for 'application/json' data tiddlers.</li><li><strong>$jsonmangler</strong>, a widget that catches messages to edit json data tiddlers (used in the editTemplate).</li><li>A new <a class="tc-tiddlylink tc-tiddlylink-shadow" href="#%24%3A%2FControlPanel">$:/ControlPanel</a> tab, <strong>Plugin Management</strong> which allows plugin creation and editing using the new json libraries.</li><li>New filter operators:<ul><li>An updated <strong>indexes[] operator</strong> that can show all index paths. If given the argument <code>verbose</code>, it will list all paths, including the root path to nested objects and arrays.</li><li>A new <strong>hasindex[] operator</strong> that returns only those input tiddlers that have a value at the index path supplied.</li><li>A new <strong>tsort[] operator</strong> that uses a <em>tokenized sorting method</em> to resolve pesky sorting problems.</li><li>A new pair of filter operators: <strong>encodeindex[]</strong> and <strong>decodeindex[]</strong>. These are used to &quot;escape&quot; or &quot;unescape&quot; the index path separation character <code> / </code> (and the encoding character <code> ~ </code>). This can be used to build paths with literal <code>/</code>s in a key name token. This is very useful and must be studied closely.</li><li>A new <strong>encodetiddler[]</strong> operator, which returns each tiddler in the input as a full json object. Used with the previous pair of operators, this can be used to pack plugin tiddlers.</li></ul></li></ul><h1 class="">Installation</h1><p><a class="tc-tiddlylink tc-tiddlylink-resolves" href="#%24%3A%2Fplugins%2Fjoshuafontany%2Fjsonmangler">JsonMangler</a> requires the following excellent plugins:</p><ul><li><a class="tc-tiddlylink tc-tiddlylink-resolves" href="#%24%3A%2Fplugins%2Febalster%2Fmodloader">ModLoader</a> by Evan Balster</li><li><a class="tc-tiddlylink tc-tiddlylink-resolves" href="#%24%3A%2Fplugins%2Fmatabele%2Faction-maketid">Action-MakeTid</a> by Matabele.</li></ul><p>Thanks you two!</p><h2 class="">Single-file .html wikis / Node served tid files saved to wiki folder</h2><p>Drag and drop the following links to install the plugins, then restart your server and(or) refresh your wiki.</p><ul><li><a class="tc-tiddlylink tc-tiddlylink-resolves" href="#%24%3A%2Fplugins%2Febalster%2Fmodloader">$:/plugins/ebalster/modloader</a></li><li><a class="tc-tiddlylink tc-tiddlylink-resolves" href="#%24%3A%2Fplugins%2Fmatabele%2Faction-maketid">$:/plugins/matabele/action-maketid</a></li><li><a class="tc-tiddlylink tc-tiddlylink-resolves" href="#%24%3A%2Fplugins%2Fjoshuafontany%2Fjsonmangler">$:/plugins/joshuafontany/jsonmangler</a></li></ul><h2 class="">Node served from <a class="tc-tiddlylink tc-tiddlylink-missing" href="#TiddlyWiki">TiddlyWiki</a>'s plugin folder</h2><p>Use Git to clone my <code>master</code> repository into a folder in your <a class="tc-tiddlylink tc-tiddlylink-missing" href="#TiddlyWiki5">TiddlyWiki5</a> repo's plugin folder, <code>./plugins/joshuafontany/jsonmangler/</code> .</p><p>Alternately, you can use single-file <code>plugin.info</code> versions under node,js, which are found in the Releases tab.</p><p>Go to <a class="tc-tiddlylink tc-tiddlylink-shadow" href="#%24%3A%2Fplugins%2Fjoshuafontany%2Fjsonmangler%2Freadme%2FInstallation">Json Mangler Github Releases</a> and download the latest *.zip file.</p><p>Place the *.zip file in your <code>.\TiddlyWiki5</code> directory, right click and select <code>Extract Here</code> (7zip) or <code>Extract to here</code> (Winzip).</p><p>A plugin.info (json) file containing all the tiddlers for each required plugin will then be placed in the right folders within your <code>.\TiddlyWiki5\plugins</code> folder.</p><p>Edit any wiki's <code>tiddlywiki.info</code> file to include the following in the <code>plugins</code> array.</p><pre><code>&quot;joshuafontany/jsonmangler&quot;,
&quot;matabele/action-maketid&quot;,
&quot;ebalster/modloader&quot;</code></pre><p>Finally, restart your server.</p><h1 class="">Important Info</h1><p>Further documentation is available in the example wiki:</p><h2 class=""><a class="tc-tiddlylink-external" href="https://joshuafontany.github.io/TW5-JsonManglerPlugin/" rel="noopener noreferrer" target="_blank">https://joshuafontany.github.io/TW5-JsonManglerPlugin/</a></h2><p>This plugin is a work in progress; please report any issues on <a class="tc-tiddlylink tc-tiddlylink-missing" href="#GitHub">GitHub</a>: <a class="tc-tiddlylink-external" href="https://github.com/joshuafontany/TW5-JsonManglerPlugin/issues" rel="noopener noreferrer" target="_blank">https://github.com/joshuafontany/TW5-JsonManglerPlugin/issues</a></p><p>If you find this useful and would care to donate, please use my <a class="tc-tiddlylink tc-tiddlylink-missing" href="#PayPal">PayPal</a>: <a class="tc-tiddlylink-external" href="https://paypal.me/JoshuaFontany" rel="noopener noreferrer" target="_blank">https://paypal.me/JoshuaFontany</a></p></div>