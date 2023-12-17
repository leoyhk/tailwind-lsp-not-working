IDE: Lazyvim

LSP Version: 0.0.14 (Installed with Mason)

Bug observed: LSP does not work when   "tailwindCSS.experimental.configFile": "./packages/config/tailwind/index.ts", is active in .vscode/setting.json

Expected behavior: LSP provides suggestions and auto completion

How to Recreate: 
1. Open the dir with nvim (i'm using the Lazyvim distribution), open any .tsx file. LSP does not provide any TailwindCSS related suggestions when typing the classnames.
2. Enter .vscode/setting.json and comment   "tailwindCSS.experimental.configFile": "./packages/config/tailwind/index.ts"
3. Restart nvim and open any .tsx file, the LSP should work normally

P.S. I'm searching for a solution / config that could make LSP work in lazyvim/nvim without changing the project settings (since it is a team project), i.e. i shall not treat commenting the line as the solution.
