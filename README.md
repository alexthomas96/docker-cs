# docker-cs

## What is It

This container runs:

* Xvfb - X11 in a virtual framebuffer
* x11vnc - A VNC server that scrapes the above X11 server
* [noNVC](https://kanaka.github.io/noVNC/) - A HTML5 canvas vnc viewer
* Fluxbox - a small window manager
* Counter-Strike.exe - to demo that it works

<strong>WARNING</strong> : This is <strong>NOT</strong> a trusted build! Please install only at your own risk.

## Get It

Download it by clicking [here](https://github.com/alexthomas96/docker-cs/archive/master.zip).
Unzip, and navigate to that directory.

## Build It

    docker build -t cs:useless .

## Run It

    docker run -d -p 9000:8080 cs:useless
    
## Play It ####(um, not exactly)

Give it about 2 minutes to update the launcher.
Navigate to http://localhost:9000 in your browser.

## Modify It

This is a base image. God knows how long it took to create it. 
Do so with the assurance that it WILL fail.

## Issues with It

* Wine could be optimized a bit
* Fluxbox could be skinned or reduced
* Counter Strike sucks through VNC (you can only aim at the sky / ground)
