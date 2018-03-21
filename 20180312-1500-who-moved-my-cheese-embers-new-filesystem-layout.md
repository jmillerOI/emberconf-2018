# Who Moved My Cheese? Ember's New Filesystem Layout

- Deprecation
  - No API will be deprecated until a replacement API has landed.
  - An API to be removed will always be depricate in at least one LTS.
  
- Codemods
`ember-modules-codemod` upgrade old modules to the new standard
`ember-k-codemod`

- Optional Features
  - `@ember/optional-features`
  
- How we ship a new filesystem layout
  - RCF
  - Canary Implementation
  - Burn down a list of blockers
  - Addons will convert
  - Apps will convert
  - In the far future we can consider deprecating classic layouts
  
- New FS Basics
`/app` becomes `src/`
`/src` groups related files
  
- WHAT CAN MODULE UNIFICATION DO FOR YOU
  - CO-LOCATION FOR RELATED FILES
  - IMPROVED ISOLATION FOR SINGLE-USE COMPONENT AND HELPERS
  - IMPROVED ISOLATION OF ADDON APIS
  - THROUGH ISOLATION, OPPORTUNITIES FOR LAZY loading
  
- Real World Impact
  - travis-ci/travis-ci has 82 total helpers and components
  - of these 41 were converted to use local lookup
  
- Addon Namespaces
`addonNamespace::component`

- New module unification applications can be generated with Ember CLI canary and a feature flag.

#### Create a new layout app
`npm install ember-cli/ember-cli MODULE_UNIFICATION=true ember new my-app`

### Create a new layout addon
`npm install ember-cli/ember-cli MODULE_UNIFICATION=true ember addon my-addon`

[Slides](https://youtu.be/qfnkDyHVJzs?t=22950)

[Quest Issue, Module Unification](https://github.com/emberjs/ember.js/issues/16373)
