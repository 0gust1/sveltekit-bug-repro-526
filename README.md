# SvelteKit repro dev mode

Reproduction repo for https://github.com/sveltejs/kit/pull/7388#issuecomment-1308801352

**On master:**  
sveltekit v526 + byteMD + ssr=false => **NOK**, dev mode breaks the app

`git checkout master && npm ci && npm run dev -- --force`

**On feat/v525:**  
sveltekit v525 + byteMD + ssr=false => **OK**, app works

`git checkout feat/v525 && npm ci && npm run dev -- --force`

**On feat/v526_ok:**  
sveltekit v526 + byteMD + ssr=true => **OK**, app works

`git checkout feat/v526_ok && npm ci && npm run dev -- --force`

