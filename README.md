

# Push a image to Github Packages (GHCR)
1. Create image
2. Create PAT on Github
3. Authenticate GHCR
4. Tag and push our image to GHCR

```
export CR_PAT=<TOKEN>
echo $CR_PAT | docker login ghcr.io -u USERNAME --password-stdin
```

# Use Github Actions to Publish a Docker image to Github Packages (GHCR)


1. Create repo - and Checkin our Dockerfile
2. Build your Github action workflow
3. Trigger our workflow