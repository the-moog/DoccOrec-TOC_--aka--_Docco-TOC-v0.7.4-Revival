<!DOCTYPE html><html><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1"/><link rel="stylesheet" href="https://themes.runkitcdn.com/runkit-light.css"/><link rel="stylesheet" type="text/css" href="https://runkit-packages-static.com/text-sha512-hMXVzQAm7WMNCxFLorSUo1dfndC_ejjrhL2K9jnPmmgj+uuhgPbFv7FjyklBmCF4WipTv9GxC90scnXU3LZT2A==.css" integrity="sha512-hMXVzQAm7WMNCxFLorSUo1dfndC/ejjrhL2K9jnPmmgj+uuhgPbFv7FjyklBmCF4WipTv9GxC90scnXU3LZT2A==" crossorigin="anonymous"/><style id="visible-range"></style><script id="built-in-modules" type="uri-encoded-json">%5B%22assert%22%2C%22buffer%22%2C%22child_process%22%2C%22cluster%22%2C%22console%22%2C%22crypto%22%2C%22dgram%22%2C%22dns%22%2C%22domain%22%2C%22events%22%2C%22fs%22%2C%22http%22%2C%22https%22%2C%22net%22%2C%22os%22%2C%22path%22%2C%22punycode%22%2C%22querystring%22%2C%22readline%22%2C%22stream%22%2C%22string_decoder%22%2C%22timers%22%2C%22tls%22%2C%22tty%22%2C%22url%22%2C%22util%22%2C%22v8%22%2C%22vm%22%2C%22zlib%22%2C%22module%22%5D</script><script type="text/javascript" src="https://runkit-packages-static-executables.com/update-parent-sha512-IW8D09RhHoOi4m85d15vQKOab6FetQJ4Vn0nAtmQxQnIENcBFYhoHxoNc3Go1OPT8a91_d7LcoDQq1iaV0CsKA==.bundle.js" integrity="sha512-IW8D09RhHoOi4m85d15vQKOab6FetQJ4Vn0nAtmQxQnIENcBFYhoHxoNc3Go1OPT8a91/d7LcoDQq1iaV0CsKA==" crossorigin="anonymous"></script><script type="text/javascript" src="https://runkit-packages-static-executables.com/update-from-url-sha512-F0P_ugFZRRhhiow+Gu5TSY7zBkXhfyeCCb1vmXAg4N2GoFypqRBBPdhqrSRMxcd3v5Gd0JlTdmrGdkS4++fwGw==.bundle.js" integrity="sha512-F0P/ugFZRRhhiow+Gu5TSY7zBkXhfyeCCb1vmXAg4N2GoFypqRBBPdhqrSRMxcd3v5Gd0JlTdmrGdkS4++fwGw==" crossorigin="anonymous"></script></head><body data-media-type="text/x-markdown"><div id="scroll-container" class="cm-s-runkit-light"><ol><li>This is a simple plain-markdown template.</li><li>
</li><li>It can be used to convert your docco output even further,</li><li>for example to output to PDF via <span class = "cm-comment">`</span><span class = "cm-comment">LaTeX</span><span class = "cm-comment">`</span> with <span class = "cm-link">[</span><span class = "cm-link cm-comment">`</span><span class = "cm-link cm-comment">pandoc</span><span class = "cm-link cm-comment">`</span><span class = "cm-link">]</span><span class = "cm-string cm-url">[</span><span class = "cm-string cm-url">pandoc</span><span class = "cm-string cm-url">]</span>.</li><li>
</li><li>The resulting markdown uses code fences (<span class = "cm-tag cm-bracket">&lt;</span><span class = "cm-tag">code</span><span class = "cm-tag cm-bracket">&gt;</span>```<span class = "cm-tag cm-bracket">&lt;&#x2F;</span><span class = "cm-tag">code</span><span class = "cm-tag cm-bracket">&gt;</span>), </li><li>which is compatible with Github- and pandoc-flavoured markdown.</li><li>
</li><li>Example PDF output:</li><li>
</li><li>    <span class = "cm-comment"># fetch some annotated source code</span></li><li>    <span class = "cm-comment">cd &#x2F;tmp</span></li><li>    <span class = "cm-comment">wget https:&#x2F;&#x2F;raw.github.com&#x2F;documentcloud&#x2F;underscore&#x2F;master&#x2F;underscore.js </span></li><li>    <span class = "cm-comment"># make plain with docco</span></li><li>    <span class = "cm-comment">docco -l plain-markdown underscore.js</span></li><li>    <span class = "cm-comment">cd .&#x2F;docs</span></li><li>    <span class = "cm-comment"># make PDF from plaintext with pandoc</span></li><li>    <span class = "cm-comment">pandoc -f markdown docs&#x2F;underscore.html -o underscore.pdf</span></li><li>
</li><li>
</li><li><span class = "cm-comment">`</span><span class = "cm-comment">pandoc</span><span class = "cm-comment">`</span> has a ton of options and output formats, you could also export to ePub, iBook- and Kindle-eBooks, Mediawiki markup, etc. <span class = "cm-link">[</span><span class = "cm-link">RTFM</span><span class = "cm-link">]</span><span class = "cm-string cm-url">[</span><span class = "cm-string cm-url">pandoc-man</span><span class = "cm-string cm-url">]</span>!</li><li>
</li><li>An full-fledged scientific-looking PDF could use these options:</li><li>
</li><li>    <span class = "cm-comment">pandoc -f markdown \</span></li><li>      <span class = "cm-comment">--table-of-contents \</span></li><li>      <span class = "cm-comment">--highlight-style=pygments \</span></li><li>      <span class = "cm-comment">-V title=&quot;Underscore.js&quot; \</span></li><li>      <span class = "cm-comment">-V author=&quot;Prof. Dr. J. Ashkenas&quot; \</span></li><li>      <span class = "cm-comment">-V date=&quot;$(date +%d-%m-%Y)&quot; \</span></li><li>      <span class = "cm-comment">-V documentclass=&quot;book&quot; \</span></li><li>      <span class = "cm-comment">--chapters \</span></li><li>      <span class = "cm-comment">-o docs&#x2F;underscore.pdf \</span></li><li>      <span class = "cm-comment">docs&#x2F;underscore.html</span></li><li>
</li><li>
</li><li>This is as quick-and-dirty as the original docco,</li><li>so there are some <span class = "cm-strong">**</span><span class = "cm-strong">bugs</span><span class = "cm-strong">**</span>:</li><li>
</li><li><span class = "cm-variable-2">- </span><span class = "cm-variable-2">The</span><span class = "cm-variable-2"></span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">code</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">blocks</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">don</span><span class = "cm-variable-2">&#039;</span><span class = "cm-variable-2">t</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">always</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">fit</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">on</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">paper</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">(</span><span class = "cm-variable-2">if</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">the</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">lines</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">are</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">too</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">long).</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">This</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">is</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">a</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">serious</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">issue,</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">but</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">could</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">be</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">fixed</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">&quot;</span><span class = "cm-variable-2">easily</span><span class = "cm-variable-2">&quot;</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">in</span><span class = "cm-variable-2"> </span><span class = "cm-link cm-variable-2">[</span><span class = "cm-link cm-variable-2">pandoc</span><span class = "cm-link cm-variable-2">&#039;</span><span class = "cm-link cm-variable-2">s</span><span class = "cm-link cm-variable-2"> </span><span class = "cm-link cm-variable-2">LaTeX</span><span class = "cm-link cm-variable-2"> </span><span class = "cm-link cm-variable-2">template</span><span class = "cm-link cm-variable-2">]</span><span class = "cm-string cm-url cm-variable-2">[</span><span class = "cm-string cm-url cm-variable-2">]</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">(</span><span class = "cm-variable-2">where</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">&quot;</span><span class = "cm-variable-2">easy</span><span class = "cm-variable-2">&quot;</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">is</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">relative,</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">as</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">always</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">when</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">dealing</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">with</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">LaTeX)</span></li><li>
</li><li><span class = "cm-variable-2">- </span><span class = "cm-variable-2">No</span><span class = "cm-variable-2"></span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">syntax</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">higlighting.</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">Could</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">maybe</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">built</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">into</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">the</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">template</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">--</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">it</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">would</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">be</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">just</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">a</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">matter</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">of</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">printing</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">something</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">like</span><span class = "cm-variable-2"> </span><span class = "cm-tag cm-bracket">&lt;</span><span class = "cm-tag">code</span><span class = "cm-tag cm-bracket">&gt;</span>```javascript<span class = "cm-tag cm-bracket">&lt;&#x2F;</span><span class = "cm-tag">code</span><span class = "cm-tag cm-bracket">&gt;</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">as</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">the</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">start</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">of</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">each</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">code</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">fence.</span></li><li>
</li><li><span class = "cm-variable-2">- </span><span class = "cm-variable-2">The</span><span class = "cm-variable-2"></span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">plaintext</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">output</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">file</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">is</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">markdown,</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">but</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">the</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">filename</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">has</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">.html</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">(</span><span class = "cm-variable-2">not</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">really</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">important</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">since</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">it</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">is</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">just</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">an</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">intermediary</span><span class = "cm-variable-2"> </span><span class = "cm-variable-2">file)</span></li><li>
</li><li>
</li><li>
</li><li><span class = "cm-link">[</span><span class = "cm-link">pandoc</span><span class = "cm-link">]:</span> <span class = "cm-string cm-url">http:&#x2F;&#x2F;johnmacfarlane.net&#x2F;pandoc&#x2F;index.html</span></li><li><span class = "cm-link">[</span><span class = "cm-link">pandoc-man</span><span class = "cm-link">]:</span> <span class = "cm-string cm-url">http:&#x2F;&#x2F;johnmacfarlane.net&#x2F;pandoc&#x2F;README.html</span></li><li><span class = "cm-link">[</span><span class = "cm-link">pandoc&#039;s LaTeX template</span><span class = "cm-link">]:</span> <span class = "cm-string cm-url">https:&#x2F;&#x2F;github.com&#x2F;jgm&#x2F;pandoc-templates&#x2F;blob&#x2F;master&#x2F;default.latex</span></li><li></li></ol></div><a class="unfold top" href="#"></a><a class="unfold bottom" href="#"></a></body></html>