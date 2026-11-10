# WorldMonitor: View the Latest Changes

## Steps to See the Changes Again

1.  Open a terminal and navigate to your cloned repository (for example,
    `D:\Dev\worldmonitor-git`):

    ``` cmd
    cd /d D:\Dev\worldmonitor-git
    ```

2.  Fetch the latest updates from GitHub:

    ``` cmd
    git fetch origin
    ```

3.  Switch to the required branch:

    ``` cmd
    git checkout claude/compassionate-volta-8p8m73
    ```

4.  Pull any newer commits from that branch:

    ``` cmd
    git pull
    ```

5.  Start the application. Run `npm install` first only if
    `package.json` has changed since your last installation:

    ``` cmd
    npm run dev
    ```

6.  Open the app in your browser:

    <http://localhost:3000>

## Things to Know

### Check Which Branch You Are On

Run:

``` cmd
git branch
```

The current branch is marked with an asterisk (`*`). If the current
branch is `main`, you will not see the changes from
`claude/compassionate-volta-8p8m73`.

### If the Red Banner Is Hidden

If the red banner does not appear, clear the following key from your
browser's local storage:

``` text
wm-pro-banner-launched-dismissed
```

A previous dismissal hides the banner for one week.

### Save and Push Your Local Edits

Only commits pushed to GitHub are safely stored in the remote
repository. If you make changes on your PC, run:

``` cmd
git add -A
git commit -m "Describe your changes"
git push
```

Do this before closing your work session if you want your edits
available on GitHub.

### Switch Back to the Original Code

To return to the original `main` branch:

``` cmd
git checkout main
```

You can switch between `main` and the feature branch whenever needed:

``` cmd
git checkout claude/compassionate-volta-8p8m73
```
