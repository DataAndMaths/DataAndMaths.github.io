---
layout: page
title: Statistiques
subtitle: blabla
---

<!-- header KATEX -->
<!-- https://varunagrawal.github.io/2018/03/27/latex-jekyll/ -->
<!-- Load KaTeX -->
<link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/KaTeX/0.1.1/katex.min.css">
<script src="//cdnjs.cloudflare.com/ajax/libs/KaTeX/0.1.1/katex.min.js"></script>





Here, have some $$\pi$$.

The greatest equation known to man is: 

$$e^{ix} = \cos{x} + i\sin{x}$$






<!-- footer KATEX -->
<!-- Parse the Latex divs with Katex-->
<script type="text/javascript">
  $("script[type='math/tex']").replaceWith(
    function(){
      var tex = $(this).text();
      return katex.renderToString(tex, {displayMode: false});
  });
  
  $("script[type='math/tex; mode=display']").replaceWith(
    function(){
      var tex = $(this).text();
      return katex.renderToString(tex.replace(/%.*/g, ''), {displayMode: true});
  });
</script>
