# fsjetpacktypings
fs-jetpack typings problem.

## Steps to reproduce.
```sh
npm install 
npm run build
```

Error: 
> error TS6307: File 'c:/gitroot/fsjetpacktypings/node_modules/fs-jetpack/types.ts' is not in project file list. Projects must list all files or use an 'include' pattern.

## Fix
In the node_modules/fs-jetpack folder, rename types.ts to types.d.ts.

Then
```sh
npm run build
```
This time build was successful.