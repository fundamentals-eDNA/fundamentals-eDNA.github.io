---
title: Connecting RStudio and GitHub
description: Andy's reflection from overview discussion of eDNA
author: Andy Rominger
---

These are some written instructions for connecting RStudio and GitHub.  These instructions assume you've already successfully done the following:

1. made a free account with github.com
2. downloaded and installed git (or checked that it's alread availible on your computer)
3. downloaded and installed R and RStudio (or checked that they're already availible on your computer)

We will use two R packages to help us connect RStudio and GitHub: *usethis* and *gitcreds*. Let's install those packages by typing the following in the R console

```
install.packages("usethis")
install.packages("gitcreds")
```

A common problem has been that *usethis* has a dependency on the package *crayon* which is currently not playing nice.  If you have errors involving *crayon* try this:

```
install.packages("crayon", type = "source")
install.packages("usethis")
```

Now we can use functions from those packages to help us continue.  First we use *usethis* to set up a personal access tokin that will serve as our login credential with GitHub.  We do that by typing this into the R console:

```
library(usethis)
create_github_token()
```

That should open up a web broser page where you might be promted to log into your GitHub account. Do that and then on the next page scroll to the bottom and click the "Generate token" button.  You will then see on a new page a string of numbers and letters---that's the token. Copy that token and paste it somewhere temporarily, like a blank text editor document or a blank R script, it doesnt' matter you'll soon delete it.

Now come back to RStudio and run the following in the R console:

```
library(gitcreds)
gitcreds_set()
```

This will prompt you to enter a password or token; now you can paste the token you just generated here and hit enter.

You should now be good to go.  

It's possible you've already gone through this process.  If that's the case you'll see this:

```
-> Your current credentials for 'https://github.com':

  protocol: https
  host    : github.com
  username: PersonalAccessToken
  password: <-- hidden -->

-> What would you like to do? 

1: Keep these credentials
2: Replace these credentials
3: See the password / token

Selection: 
```

Enter 1 for your selection. There will be an error message but you can ignore it.

Now we should hopefully be all connected!

Now we'll double check by going to our GitHub profile 