# Spacing

## `br`s

Some people hate `<br />`s because they're un-`[buzzword they dont know the meaning of]`, however, `br`s are useful.

When to use a br (GOOD)

```html
<!-- GOOD -->
<p>
  text text text,<br />
  text text text.
</p>
```

Also when to use a br (GOOD)

```html
<!-- GOOD -->
<button>button</button>
<br />
<br />
<p>text text text? <a ...>link</a></p>
```

VERY BAD, NEVER DO THIS (BAD)

```html
<!-- BAD -->
<div ...>
  <br />
  <!-- NEVER DO THIS -->
  <br />
  <!-- BAD -->
  <br />
  <br />
  <p>text text text.</p>
  <br />
  <!-- NEVER DO THIS -->
  <br />
  <!-- BAD -->
  <button>button</button>
  <br />
  <!-- NEVER DO THIS -->
  <br />
  <!-- BAD -->
</div>
```

Also, notice the `/`:

```html
<br />     <!-- GOOD -->

<br>       <!-- BAD -->

<br></br>  <!-- BAD -->  <!-- INVALID HTML -->
```

## Padding

> Padding handles spacing inside elements, between their border their content.

Not all elements have the same padding, however, elements of the same "type" have the same padding rules.

### `Text` elements with `background`

`Text` with `background` elements have a horizontal padding of `0.4rem` and a vertical padding of `0.2rem`.

`Text` with `background` are elements the user sees as "inline", or "part of the text", and have a distinguished background color. This includes:

- highlighted text (`<mark>...</mark>`, `<... class="mark">...</...>`)
- inline code (`<code>...</code>`, `<... class="code">...</...>`)

### `Interactive` elements with `background`

`Interactive` elements with `background` have a horizontal padding of `0.8rem` and a vertical padding of `0.4rem`.

`Interactive` elements with `background` include all user-interactable or clickable elements that have a distinguished background color. This includes:

- buttons (`<button>...</button>`, `<... class="button">...</...>`)
- inputs (`<input type="...">...</input>`)
  - textareas (`<textarea>...</textarea>`)

### `Box` elements

`Box` elements have a padding of `1rem`.

`Box` elements include:

- boxes (`<... class="box">...</...>`)
- table children (`<table>...</table>`)
  - `th`
  - `td`
- heros (`<... class="hero">...</...>`)
- footers (`<footer>...</footer>`, `<... class="footer">...</...>`)

> Note that in tables, the padding is applied to each cell (`th`, `td`).

## Margins

> Margins handle spacing between elements.

(Almost) every element has a bottom margin of `1rem`, so that the element after it is pushed down. They do not _need_ a top margin, because every element assumes the element above it is responsible for pushing the next line's element down.
