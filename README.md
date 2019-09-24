# jekyll-includes
Test case for indented includes tag issue.

`index.md` after include tags are parsed:

```md
- list
- list
  <strong>strong tag</strong>
<a href="https://github.com">github</a>
- list
  <ul>
  <li>nested list</li>
</ul>
- list
  <div>div in a list, line break below</div>

<button>button</button>
- list
```

The markdown list breaks because of the line breaks/injected HTML.
