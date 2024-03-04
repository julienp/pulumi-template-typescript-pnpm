A pulumi template that uses pnpm to manage node dependencies.

Note that the presence of `pnpm-lock.yaml` is what makes `pulumi install` opt in to using pnpm over npm.

```
% pulumi new --stack dev \
    --name "pnpm-example" \
    --description "project using pnpm" \
    https://github.com/julienp/pulumi-template-typescript-pnpm
Created project 'pnpm-example'

Created stack 'dev'

Installing dependencies...

Lockfile is up to date, resolution step is skipped
Packages: +285

Progress: resolved 285, reused 285, downloaded 0, added 285, done

dependencies:
+ @pulumi/pulumi 3.108.1

devDependencies:
+ @types/node 18.19.21

Done in 798ms
Finished installing dependencies

Your new project is ready to go! ✨

To perform an initial deployment, run `pulumi up`

```
