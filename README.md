# SveleKitSummer

This project is the current [2025-7-5] Sveltekit demo app configured to be deployed with the node adapter to Coolify.

The build.yml tells Github Actions how to build the Dockerfile then uses Coolify's webhook (with auth) to automatically redeploy the project.

---

1. Git push 
2. Github Actions build the project to Docker Image
3. Docker image is deployed to Coolify project via webhook

---

It can be kind of a pain to set it up this way, but I promise it's worth it. Building with Coolify takes a lot of resources while also being slow, and can really easily crash the affordable tier of VPS.

Offloading the build to Actions ensure detailed deployment logs, quick builds, and instant deployment to Coolify. I can't rave enough about how much faster it is.

---