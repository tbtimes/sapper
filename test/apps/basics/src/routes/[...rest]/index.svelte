<script context="module">
  export function preload({ query, params }) {
    const { rest } = params;
    return { rest };
  }
</script>

<script>
  export let rest;
</script>

<h1>{rest.join(',')}</h1>
<h2>Great success!</h2>
<a href="a">a</a>
<a href="ambiguous/ok.json">ok</a>
<a href="echo-query?message">ok</a>
<a href="echo-query?p=one&p=two">ok</a>
<a href="xyz/abc/deep">deep</a>
<a href="xyz/abc">deep</a>
<a href="xyz/abc/def">deep</a>
<a href="xyz/abc/def/ghi">deep</a>
<a href="234">regexp route</a>

<div class="hydrate-test" />
