# EKI RESEARCH & DEVELOPMENT

"OK"


update note : 
- CODE SERVER [VISUAL STUDIO CODE - BROWSER]
- FILE BROWSER [FILE SHARING - BROWSER]
- WETTY [TERMINAL SSH - BROWSER]



# documentation code server

```ts

  docker run -it --name code-server -p 127.0.0.1:8080:8080 \
  -v "$HOME/.config:/home/coder/.config" \
  -v "$PWD:/home/coder/project" \
  -u "$(id -u):$(id -g)" \
  -e "DOCKER_USER=$USER" \
  codercom/code-server:latest
  
```


# documentation file browser

```ts

docker run \
    -v /path/to/root:/srv \
    -v /path/filebrowser.db:/database.db \
    -v /path/.filebrowser.json:/.filebrowser.json \
    --user $(id -u):$(id -g)
    -p 80:80 \
    filebrowser/filebrowser

```



# documentation wetty

```ts

docker run --rm -p 3000:3000 wettyoss/wetty --ssh-host=<YOUR-IP>

```


for best config see : EKI_BEST_CONFIG.txt


![EXAMPLE](https://github.com/EKI-INDRADI/eki-latihan-docker-code-server--file-browser--wetty/raw/master/hasil/eki.png)


# Regards,

# Eki Indradi
"TIME > KNOWLEDGE > MONEY".





