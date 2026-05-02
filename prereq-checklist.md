# Week 0 — Prerequisites Checklist

Half a day of setup. Do this before Week 1 starts so you're not fighting tools when the curriculum begins.

## Tools to install

- [ ] **Node.js LTS** — https://nodejs.org/ · verify: `node --version` and `npm --version`
- [ ] **Git** — https://git-scm.com/download/win · verify: `git --version`
- [ ] **GitHub account** — https://github.com (you may already have one)
- [ ] **Postman desktop** — https://www.postman.com/downloads/ · free tier
- [ ] **Docker Desktop for Windows** — https://www.docker.com/products/docker-desktop/ · needed for crAPI in Phase 2
- [ ] **VS Code** — https://code.visualstudio.com/ (you likely have this)
- [ ] **VS Code REST Client extension** — search "REST Client" by Huachao Mao in Extensions
- [ ] **Burp Suite Community Edition** — https://portswigger.net/burp/communitydownload · free, needed for Phase 2

## Accounts to create (all free)

- [ ] **freeCodeCamp** — https://www.freecodecamp.org/ · for the Back-End cert in Weeks 3-4
- [ ] **Postman** — sign in to the desktop app · for the Galaxy badges in Week 1
- [ ] **APISec University** — https://www.apisecuniversity.com/ · for Phase 2
- [ ] **PortSwigger** — https://portswigger.net/users/register · for Web Security Academy labs

## Repo to create

- [ ] Create new GitHub repo named `api-study-vault` (public)
- [ ] Clone locally: `git clone https://github.com/<your-username>/api-study-vault.git`
- [ ] Add a starter `README.md`: "8-week API study vault. Curriculum: types → build → break."
- [ ] First commit + push

## Sanity checks

- [ ] Run `docker run hello-world` — confirms Docker works
- [ ] In Postman, hit `https://jsonplaceholder.typicode.com/todos/1` with GET. Should see JSON response.
- [ ] In Burp Community, start the proxy on port 8080. Confirm browser proxy traffic flows through it.

When all boxes are checked, you're ready for **Phase 0 — Types Orientation**.
