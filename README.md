# doc-tools

Various Docker images for a better development experience.

## Node

A straightforward Node.js image with some configurations.

Use it for isolated Node.js execution. Don't forget to enable host networking in Docker Desktop.

### Usage

You can use the following aliases in your shell configuration file (e.g., `.bashrc`, `.zshrc`):

```sh
alias yarn='docker run --network host -it --rm -v $(pwd):/app --workdir /app fullpipe/node:lts yarn'
alias npm='docker run --network host -it --rm -v $(pwd):/app -v ~/.npm:/root/.npm -v ~/.npmrc:/root/.npmrc fullpipe/node:lts npm'
alias node='docker run --network host -it --rm -v $(pwd):/app --workdir /app fullpipe/node:lts node'
alias npx='docker run --network host -it --rm -v $(pwd):/app --workdir /app fullpipe/node:lts npx'
```
