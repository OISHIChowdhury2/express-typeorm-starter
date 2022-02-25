## How to Recreate ?

### Here are the steps

1. yarn init
2. tsc --init && yarn add typescript ts-node @types/node -D
3. yarn add eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin -D
4. touch .eslintrc
5. touch .eslintignore
6. add lint script in package.json
7. yarn add prettier eslint-config-prettier -D
8. add prettier in extends array of .eslintrc
9. touch .prettierrc.js
10. npx husky-init && yarn
11. npx husky add .husky/commit-msg 'npx --no-install commitlint --edit "$1"'
12. yarn add  @commitlint/config-conventional @commitlint/cli -D
13. echo "module.exports = { extends: ['@commitlint/config-conventional'] };" > commitlint.config.js