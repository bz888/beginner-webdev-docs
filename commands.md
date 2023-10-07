### Useful commands

#### notes: A list of helpful commands

#### Terminal:

- `ls` List all contents in a directory (folder) if you wish to list all contents including hidden contents `ls -a`
- `mkdir` Create directory e.g. (`mkdir myFolder`), creates a folder named `myFolder`
- `touch` Create a file e.g. (`touch index.ts`), creates a file `index.ts`
- `rm -rf` Deletes the desired file/directory (`rm -rf node_modules`) !!! Use with care
- You can also find more commands online that would help you, but these are the main ones you can use

#### Docker commands

- Inside the directory with a `docker-compose.yml` file you can run `docker-compose pull && docker-compose up` to start your docker image
- `docker-compose down` to stop your docker service

### Git

- `git clone <repo>` repo can either be SSH or HTTPs e.g. `git clone git@todo-list`
- `git pull` pulling from branch
- `git rebase <branch>` I doubt this will be used, Chat GPT for its purpose
- `git checkout -b <branch-name>` creating a new branch on the branch you are currently on
- `git add -a` or `gaa` adds all files to be committed
- `git commit -m '<message>'` commit all added files
- `git push` pushing your commits to the branch

#### Node js package.json commands

#### npm:

- `npm install <package-name>` Installing new packages if you wish to add it as a dev dependency add the flag `-D` e.g. `npm install --dev types/node`
- `npm install` or `npm i` installs all packages stated in your `package.json`

### yarn:

- `yarn install` or `yarn` installs all packages
- `yarn add <package-name>` if you wish to add it as a dev dependency add the flag `-D` e.g. `yarn add -D types/node`
