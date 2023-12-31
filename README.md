# Requirements:
- Golang
- Godoc
- Swaggo/swag
- Makefile
- Tailwind standalone CLI
- Node for @storybook/server-webpack5, and for webpack
- Git bash or simillar (to build, and for some other commands too)

# How to:
## First time running after clone
<ul>
  <li>make dep</li>
  <li>make storybook-dep</li>
  <li>make webpack-dep</li>
</ul>

## Run development mode
<ol type="1">
  <li>
    In one CMD do: (tailwind, with live reload)
    <ul>
      <li>make tailwind-watch</li>
    </ul>
  </li>

  <li>
    In a second CMD do: (storybook)
    <ul>
      <li>make storybook</li>
    </ul>
  </li>

  <li>
    In a third CMD do: (webpack, with live reload)
    <ul>
      <li>make webpack-watch</li>
    </ul>
  </li>

  <li>
    In a fourth CMD do: (server, with live reload)
    <ul>
      <li>air</li>
    </ul>
  </li>

  <li>
    In a fifth CMD do: (go docs)
    <ul>
      <li>make docs</li>
    </ul>
  </li>

  <li>
    In a sixth CMD do: (swagger ui)
    <ul>
      <li>make swag</li>
    </ul>
  </li>
</ol>

## Alternative for running in development mode
<ul>
  <li>
    In case you don't mind the output being all mixed, you can run all commands above at once using:
    <ul>
      <li>go run ./dev-script</li>
    </ul>
  </li>
</ul>

## Compile for production mode
<ul>
  <li>make build</li>
  <li>(copy the files needed to another directory)</li>
  <li>make clean</li>
</ul>