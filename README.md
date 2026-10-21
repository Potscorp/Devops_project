# Just for You — Enhanced romantic website ♡

## Pages
- `index.html` — home page with a hero portrait and four portrait cards
- `letter.html` — romantic letter and portrait cards
- `memories.html` — portrait-focused gallery
- `reasons.html` — appreciation notes and portrait cards
- `surprise.html` — interactive gift reveal and a sweet, no-pressure date invitation
- `style.css` — shared pink theme and responsive styling

## Add your photos
Create/use the `images` folder beside the HTML files. Copy your pictures into it and name them:
- `heroine.jpeg` — main homepage portrait
- `portrait1.jpeg` through `portrait7.jpeg` — portraits used across the pages

You can use `.jpg` or `.png` too, but update the matching `src` paths in the HTML if you change the extensions. The uploaded ZIP did not contain your `images` folder or photos, so this ZIP includes beautiful pink placeholders until you add your real pictures. Your actual photos are not included or changed.

## Preview
Open `index.html` in a browser. Placeholder images need an internet connection; local photos work offline.

## Docker deployment
```bash
docker build -t her-website .
docker run -d --name her-website --restart unless-stopped -p 8081:80 her-website
```
Open `http://YOUR_DOCKER_PUBLIC_IP:8081` and allow inbound TCP 8081 in the EC2 security group.

To redeploy:
```bash
docker rm -f her-website
docker build -t her-website .
docker run -d --name her-website --restart unless-stopped -p 8081:80 her-website
```
"# Devops_project" 
