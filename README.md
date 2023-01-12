# yarn-workspace-bug

`pkg-a` depends on `"jest": "^26"`. `pkg-b` depends on `"jest": "^29"`.

To reproduce the bug
- clone repository & `yarn install`
- `yarn workspace pgk-a jest --version` -> outputs `26.6.3` as expected
- `yarn workspace pkg-b jest --version` -> outputs `26.6.3` as well, but exptected is `29.3.1`
