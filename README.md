# TS Charts Repo

This is an example charts repository.

### How It Works

I set up GitHub Pages to point to the `docs` folder. From there, I can
create and publish docs like this:

```console
$ helm create alpine
$ helm package alpine
$ mv alpine-0.2.0.tgz docs
$ helm repo index docs --url https://technosophos.github.io/tscharts
$ git add -i
$ git commit -av
$ git push origin master
```

From there, I can do a `helm repo add tscharts
https://technosophos.github.io/tscharts`
