{% highlight html %}
<!-- TRANSACTIONALE CODE - DO NOT EDIT! -->
<script>
    var _tr_run = (function() {
        if(window.location.search.indexOf('tr=1') < 0) return;
        var td = document.createElement('div'); td.id='transactionale';document.body.appendChild(td);
        var s = document.createElement('script');
        s.src = 'https://www.transactionale.com/embedded/popup'+window.location.search;
        document.getElementsByTagName('head')[0].appendChild(s);
        return function(d) { _tr_runTransactionale('transactionale', d.html, d.js); }
    })();
</script>
<!-- /TRANSACTIONALE CODE - DO NOT EDIT! -->
{% endhighlight %}
