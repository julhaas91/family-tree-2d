# Family Tree 2D
A 2D visualization of my extended family tree.

## Installation
```bash
git clone https://github.com/julhaas91/family-tree-2d.git && cd family-tree-2d
npm install
VITE_STATIC_URL='/family.ged' npm start
```

## Deployment on Firebase
To deploy the family tree as a static website on Firebase:

1. Install Firebase CLI globally if you haven't already:
```bash
npm install -g firebase-tools
```

2. Log in to Firebase:
```bash
firebase login
```

3. Create a new Firebase site (replace 'familie-site' with your desired site name):
```bash
firebase hosting:sites:create familie-site
```

4. Set up the hosting target:
```bash
firebase target:apply hosting familie-site familie-site
```

5. Build and deploy the site:
```bash
npm run build && firebase deploy --only hosting:familie-site
```

Your site will be available at: `https://familie-site.web.app` (replace 'familie-site' with your chosen site name)

## Deployment on Google Cloud
To deploy the family tree as a static website:
1. Add a GED file to `family-tree-2/public/family.ged`
2. Add a thumbnail logo to `family-tree-2d/public/logo.png`
3. Run:
```bash
./taskfile.sh create '<your-family-tree>' (e.g. 'julius-family-tree-2d')
```

## Updating the Family Tree
To update and redeploy the family tree:
1. Replace the GED file in `family-tree-2/public/family.ged`
2. Replace the thumbnail logo in `family-tree-2d/public/logo.png`
3. Run:
```bash
./taskfile.sh update '<your-family-tree>' (e.g. 'julius-family-tree-2d')
```

## Credits
This project is based on [Topola Viewer](https://pewu.github.io/topola-viewer), licensed under the [Apache 2.0 License](https://github.com/PeWu/topola-viewer/blob/master/LICENSE). Special thanks to [PeWu](https://github.com/PeWu) for the great work!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

> For inquiries, feel free to contact me via [email](mailto:juliushaas91@gmail.com) or [LinkedIn](https://www.linkedin.com/in/jh91/)
