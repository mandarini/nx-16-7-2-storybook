# Angular + Storybook + Nx

Tried to reproduce issue with Nx 16.7.2 and Angular 16.2:

1. Generated workspace with Nx 16.7.2:
   ```
   npx create-nx-workspace@16.7.2 my-wksp --preset=angular
   ```
2. Installed the `@nx/storybook` plugin
3. Generated Angular lib:
   ```
   nx g @nx/angular:lib my-lib
   ```
4. Generated component for that lib:
   ```
   nx g @nx/angular:component --project=my-lib my-comp
   ```
5. Generated Storybook configuration for that lib
   ```
   nx g @nx/angular:storybook-configuration my-lib
   ```
6. Run Storybook
   ```
   nx storybook my-lib
   ```

No error appears.
