
  ![on-push](../../actions/workflows/on-push.yaml/badge.svg)
  ![on-pull-request](../../actions/workflows/on-pull-request.yaml/badge.svg)
  ![on-schedule](../../actions/workflows/on-schedule.yaml/badge.svg)

  # avis-res-lab's Website

  Visit **[avis-res-lab.github.io](https://avis-res-lab.github.io)** 🚀

  _Built with [Lab Website Template](https://greene-lab.gitbook.io/lab-website-template-docs)_


---

Go ot the following link for more thorough instructions
[How to run locally](https://greene-lab.gitbook.io/lab-website-template-docs/getting-started/preview-your-site)

## How to run locally
Run this whenever you want to preview the site:
```bash
cd /c/Monaf/Codes/avis-res-lab.github.io
bash ./.docker/run.sh
```
The first time is slow because Docker builds the image. After that, it should be much faster because Docker reuses the cached build.

While that terminal is running, open:
```bash
http://localhost:4000
```

## or 
### Option 2: Create A Reusable Docker Container

If you want to start/stop it from Docker Desktop directly, do this once from Git Bash.

Go to the repo:
```bash
cd /c/Monaf/Codes/avis-res-lab.github.io
```
Fix script line endings if you have not already:
```bash
sed -i 's/\r$//' .docker/run.sh .docker/entrypoint.sh
chmod +x .docker/run.sh .docker/entrypoint.sh
```
Build the Docker image:
```bash
docker build -t avis-lab-site:local -f .docker/Dockerfile .
```
Create a reusable container:
```bash
docker create \
  --name avis-lab-site \
  --init \
  -it \
  -p 4000:4000 \
  -p 35729:35729 \
  -v "$(pwd):/usr/src/app" \
  avis-lab-site:local
```
Start it:
```bash
docker start -ai avis-lab-site
```
Then open: `http://localhost:4000`

After this, you can also open Docker Desktop, go to Containers, find avis-lab-site, and press the play/start button. To Stop It, either press `Ctrl+C` in the terminal, or stop it from Docker Desktop. Next Time, You do not need to recreate the container. Just start it:
```bash
docker start -ai avis-lab-site
```
or start avis-lab-site from Docker Desktop.
