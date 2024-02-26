```sh
# git aliases
alias gst="git status"
alias gco="git checkout"
alias gcob="git checkout -b"
alias ga="git add"
alias gpull="git pull"
alias gpush="git push"

# --------------
# apstra aliases
# --------------
alias slicercli=""
alias slicercli_local="docker run --rm --net host -i -t -e SLICER_SERVER_URL=http://slicer-dev.dc1.apstra.com:80 -v $HOME:/root -v $PWD:/project docker-registry.dc1.apstra.com:5000/slicercli:ed_test /usr/local/bin/slicercli -it"
alias slicercli_local_prod="docker run --rm --net host -i -t -e SLICER_SERVER_URL=http://slicer.dc1.apstra.com:80 -v $HOME:/root -v $PWD:/project docker-registry.dc1.apstra.com:5000/slicercli:ed_test /usr/local/bin/slicercli -it"
# Build local slicercli
alias build_slicercli="docker build -t docker-registry.dc1.apstra.com:5000/slicercli:ed_test -f Dockerfile.slicercli --no-cache ."
alias build_slicercli_prereq6="docker pull docker pull docker-registry:5000/slicercli_base:0.6"
alias build_slicercli_prereq8="docker pull docker pull docker-registry:5000/slicercli_base:0.8"

# tox aliases
# TODO can you source a aliases file inside the container? would be real nice :)
# alias tox38="cd /home/ed/Project/systest/tox -e py38 -- "
alias tox38="tox -e py38 -- "
alias tox27="tox -e py27 -- "
alias tox="cd ~/Project/systest && bash tox_build.sh"

# EXTRA:
alias slicercli_update='docker pull docker-registry-ng.dc1.apstra.com:5000/slicercli/slicercli:latest'
alias slicercli_dev='docker run --rm --net host -i -t -e SLICER_SERVER_URL=http://slicer-dev.dc1.apstra.com:80 -v $HOME:/root -v $HOME:/project docker-registry-ng.dc1.apstra.com:5000/slicercli/slicercli /usr/local/bin/slicercli -it'
alias slicercli='docker run --rm --net host -i -t -e SLICER_SERVER_URL=http://slicer.dc1.apstra.com:80 -v $HOME:/root -v $HOME:/project docker-registry-ng.dc1.apstra.com:5000/slicercli/slicercli /usr/local/bin/slicercli -it'

alias tox_start='docker run -it --rm --net host -v /var/run/docker.sock:/var/run/docker.sock -v /home/ed/Project/systest-2272/.entrypoint.sh:/tmp/entrypoint.sh --privileged -v /home/ed/Project/systest-2272:/project -w /root --entrypoint=/tmp/entrypoint.sh docker-registry.dc1.apstra.com:5000/slicer-dev:0.3.14'

alias ssh_dev='ssh apstrktr@slicer-dev-cp.dc1.apstra.com'
alias ssh_prd='ssh apstrktr@slicer-dev.dc1.apstra.com'
```
