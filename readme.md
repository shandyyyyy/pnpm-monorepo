 # Running tasks with pnpm

`pnpm --filter my-remix-app dev/build` // dev/build my-remix-app

`pnpm add shared-ui --filter my-remix-app --workspace`   //add share-ui package to my-remix-app
`pnpm add react --filter my-remix-app`  //add package to my-remix-app

`pnpm run -r build`  // build all application
`pnpm run --parallel -r build` //

# Running tasks with Nx
`npx nx build my-remix-app`
`npx nx dev my-remix-app`
`npx nx graph`
`npx nx affected:graph`
`npx nx affected:build`
`npx nx run-many --target=build --all`  //We can also run commands in parallel across the projects
`npx nx run-many --target=build --projects=my-remix-app` selectively specify projects with

```
 function test(){
  console.log('test')
 }
```