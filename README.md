# quokkaMathjsBug
Demo of hanging bug when using mathjs inside quokka.

Shows how quokka hangs when trying to run mathjs with a certain configuration. To reproduce, 
```npm install```
then start quokka on mathJsLab.ts. It will hang.
However, if you *either* remove `ts-node` from the `devDependencies` in `package.json`, *or* if you set `allowJs: false` in `tsconfig.json`, then it will work.
