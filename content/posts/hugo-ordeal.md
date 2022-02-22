---
title: "Hugo Ordeal"
date: 2022-02-21T19:46:53-06:00
draft: false
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

I couldn't find the a way of escaping the 's yet.