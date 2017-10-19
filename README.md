# Manifest for Istio repo


```bash
 
  # Download repo tool
  # See https://source.android.com/source/downloading
  mkdir ~/bin
  PATH=~/bin:$PATH
  curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
  chmod a+x ~/bin/repo
  
  # Workdir for istio  
  mkdir MY_ISTIO_SRC_DIR
  cd MY_ISTIO_SRC_DIR
  
  git config --global user.name "Your Name"
  git config --global user.email "you@example.com"
  
  repo init -u https://github.com/istio/manifest
  repo sync -c 
  
```

# Fetching a different branch

```bash


  repo init -u https://github.com/istio/manifest -b release-0.2
  repo sync -c 
```
