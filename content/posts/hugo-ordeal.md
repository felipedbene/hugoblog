---
title: "Hugo Ordeal"
date: 2022-02-21T19:46:53-06:00
draft: false
toc: true
---


Setting this site together was a struggle, I thought that initially using hugo would make the process simplier but I've struggled with a '.
When I connected the GitHub branch to Amplify I've a json error completely undescriptive : "Invalid build file" and the only detail was that my application had no build file :-D
It turns out that Hugo's config.toml doesn't take  ' and that's the reason my site isn't called Felipe's Tech Notes.
```
baseURL = 'https://www.debene.xyz'
languageCode = 'en-us'
title = 'De Bene Tech Notes'
theme = "ananke"
```

instead of 

```
baseURL = 'https://www.debene.xyz'
languageCode = 'en-us'
title = 'De Bene's Tech Notes'
theme = "ananke"
```

In the end it was as stupid as using " instead of ' and the final code was :

```
baseURL = 'https://www.debene.xyz'
languageCode = 'en-us'
title = "De Bene's Tech Notes"
theme = "ananke"
```

Easy enough and to host it, of course AWS' Amplify: 

I've used this [tutorial](https://aws.amazon.com/es/blogs/devops/agile-website-delivery-with-hugo-and-aws-amplify/).

;-)