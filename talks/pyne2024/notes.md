



Nix nixpkgs NixOS, nix store vs FHS: 
Google IDX, Replit, GitPod, Canva, Shopify, Tumblr



Como será o próximo bilhão de programadores?

Porque software não é como LEGO?


Pessoas > Tecnologia

- https://medium.com/@sergiomarioq/pessoas-tecnologia-ca688e139e9e
- https://2024.pythonnordeste.org/



TODO get the thumbnail
https://www.youtube.com/watch?v=korOpibkm6g




The sorry state:
- xkcd,


[Replit Developer Day Keynote](https://www.youtube.com/embed/7TCqGslll-4?start=702&end=726&version=3), start=702&end=726


Docker is not enough:


- https://github.com/spatialaudio/nbsphinx/issues/182#issuecomment-430484260  
- https://github.com/PedroRegisPOAR/nbsphinx-issue-182



- https://stackoverflow.com/questions/53546775/overly-function-from-geopandas-not-working


OpenCV


- https://answers.opencv.org/question/228178/opencv-python-no-module-named-cv2/


Add slide
[Elana Hashman - The Black Magic of Python Wheels - PyCon 2019](https://www.youtube.com/watch?v=02aAZ8u3wEQ)



TODO get thumbnail
- [DeepMind’s New AI Beats Billion Dollar Systems - For Free!](https://www.youtube.com/watch?v=BufUW7h9TB8)
- https://github.com/google-deepmind/graphcast/blob/8debd7289bb2c498485f79dbd98d8b4933bfc6a7/graphcast_demo.ipynb


- Linux Torvalds: [DebConf 14: QA with Linus Torvalds](https://www.youtube.com/embed/5PmHRSeA2c8?start=1801&end=1867&version=3), start=1801&end=1867
- Andrew Stuart Tanenbaum: [MINIX 3: a Modular, Self-Healing POSIX-compatible Operating System](https://www.youtube.com/embed/bx3KuE7UjGA?start=2295&end=2376&version=3), start=2295&end=2376,
- Netflix: [Dependency Hell, Monorepos and beyond](https://www.youtube.com/embed/VNqmHJtItCs?start=649&end=858&version=3), start=649&end=858, by Mike McGarr 
- Uber: [Uber Technology Day: Monorepo to Multirepo and Back Again](https://www.youtube.com/embed/lV8-1S28ycM?start=342&end=428&version=3), start=342&end=428
- Shopify: [Shipit! Presents: How Shopify Uses Nix](https://www.youtube.com/embed/KaIRpx11qrc?start=1142&end=1151&version=3), start=1142&end=1151
- Canvas: [Supporting GPU-accelerated Machine Learning with Kubernetes and Nix](https://canvatechblog.com/supporting-gpu-accelerated-machine-learning-with-kubernetes-and-nix-7c1da8e42f61), By [Jonathon Belotti](https://github.com/thundergolfer) from [Canva Engineering](https://medium.com/@canvatechblog?source=post_page-----7c1da8e42f61--------------------------------)
- Semaphore CI: [Under the Hood of Replit with Amjad Masad](https://www.youtube.com/embed/bKhMsQTyzwY?start=164&end=206&version=3), start=164&end=206




TODO
Refs.:
- https://idx.dev/blog/article/nix-on-idx
- https://idx.dev/blog/article/insiders-look-at-gemini-in-idx
- https://youtu.be/_l-y4edAmFU?t=48
- https://youtu.be/-wlZY4tfGMY?t=636
- https://youtu.be/-wlZY4tfGMY?t=711
- https://youtu.be/UbXv-T4IUXk?t=858
- https://www.youtube.com/embed/UbXv-T4IUXk?start=838&end=877&version=3
- [Tips & tricks for using IDX: Building with Gemini in IDX](https://www.youtube.com/watch?v=-3S36NPWuQY)





Revisão:

- ELF
- file
- ldd
- pachelf
- readelf
- type
- man hier


FHS things #!/bin/sh:
- chroot
- LXC
- OCI Images 
- systemd units
- Virtual Machines
- ISOs
- ?



Alpine -> busybox -> toybox

- 1.02GB, docker run python:3.12.5-bookworm python --version
- 53.6MB, docker run python:3.12.5-alpine3.20 python --version
- 4.26MB, docker run busybox
- 854kB, docker run tianon/toybox



Primeiro os requisitos históricos sobre como o Filesystem Hierarchy Standard (FHS) se formou.

Linux Directories Explained in 100 Seconds
https://www.youtube.com/watch?v=42iQKuQodW4

Tutorial: Building the Simplest Possible Linux System - Rob Landley, se-instruments.com https://www.youtube.com/embed/Sk9TatW9ino?start=4921&end=5023&version=3
Matthew Croughan - Nix The Planet - SCaLE 21x https://www.youtube.com/embed/6iviTZfiLGU?start=448&end=489&version=3
What exactly is Nix and NixOS? (Vincent Ambo) https://www.youtube.com/watch?v=_R9ekUTOoII
Nix: What Even is it Though https://www.youtube.com/watch?v=6iVXaqUfHi4

Referências textuais sobre FHS:
- http://landley.net/writing/hackermonthly-issue022-pg33.pdf
- https://www.bell-labs.com/usr/dmr/www/notes.html




 yt-dlp \
 --write-thumbnail \
 --skip-download \
 --convert-thumbnails jpg \
 --ppa "ThumbnailsConvertor:-q:v 1" \
 https://www.youtube.com/watch\?v\=42iQKuQodW4 \
 --extractor-args "youtube:player_client=ios"

- https://github.com/ytdl-org/youtube-dl/issues/28457
- https://github.com/yt-dlp/yt-dlp/issues/7585#issuecomment-1635224154


yt-dlp \
--download-sections "*30-45" \
-v https://www.youtube.com/embed/bbmWOjuFmgA \
--force-ipv4 -S vcodec:h264 --extractor-args "youtube:player_client=ios" --force-keyframes-at-cuts

https://github.com/yt-dlp/yt-dlp/issues/7585#issuecomment-1635224154




ffmpeg -ss 0.4 -i Linux\ File\ System\ Explained\!\ \[bbmWOjuFmgA\].mp4 -frames:v 1 video-poster04.png
ffmpeg -ss 11 -i Linux\ File\ System\ Explained\!\ \[bbmWOjuFmgA\].mp4 -frames:v 1 video-poster11.png





yt-dlp -f "(bestvideo+bestaudio/best)[protocol!*=dash]" --external-downloader ffmpeg --external-downloader-args "ffmpeg_i:-ss 3263 -to 3274" "

--force-keyframes-at-cuts 

- https://www.reddit.com/r/youtubedl/wiki/howdoidownloadpartsofavideo/
- https://www.reddit.com/r/youtubedl/comments/1cs2ei6/ytdlp_any_simple_way_to_download_a_section_trim/

https://www.youtube.com/watch?v=fuWPuJZ9NcU


https://www.youtube.com/watch?v=_f5uev7UTz0



https://www.youtube.com/watch?v=oPymb2-IXbg


https://www.youtube.com/watch?v=J7Hdaqs1rjU



Linux distros
https://www.youtube.com/watch?v=korOpibkm6g
https://www.youtube.com/watch?v=ApkoY-PN0Nk








- https://www.nature.com/articles/d41586-020-02462-7
- http://rescience.github.io/ten-years/



In particular, in our own version of the system, there is a directory "/usr" which contains all user's directories, 
and which is stored on a relatively large, but slow moving head disk, while the othe files are on the 
fast but small fixed-head disk.
[...]
The reason is this: files are limited in size to 64K bytes. The reason for this is not particularly defensible, 
but it has to do with the fact that the PDP-11 word size is 16 bits.

PDP-11 can only accommodate 28K 16-bit words of core

https://www.bell-labs.com/usr/dmr/www/notes.html 15 March, 1972


> Ken and Dennis leaked their OS into the equivalent of 
> home because the root disk on the PDP-11 was too small.
Refs.:
- [Tutorial: Building the Simplest Possible Linux System - Rob Landley, se-instruments.com](https://www.youtube.com/embed/Sk9TatW9ino?start=4921&end=5023&version=3)
- https://landley.net/writing/hackermonthly-issue022-pg33.pdf
- https://yin.neocities.org/social/rob_langley_about_the_usr_split
- http://lists.busybox.net/pipermail/busybox/2010-December/074114.html
- [The Rise of Unix. The Seeds of its Fall.](https://www.youtube.com/watch?v=HADp3emVABg)


shared libraries (introduced by the Berkeley guys) prevent you from 
independently upgrading the /lib and /usr/bin parts.  They two partitions have 
to _match_ or they won't work.  This wasn't the case in 1974, back then they 
had a certain level of independence because everything was statically linked.


RK05 2.5 megabytes
PDP-7, PDP-8, PDP-11, and PDP-15

- https://en.wikipedia.org/wiki/File:RK05.jpg
- https://en.wikipedia.org/wiki/RK05
- https://en.wikipedia.org/wiki/PDP-7
- https://en.wikipedia.org/wiki/PDP-11
- https://www.bell-labs.com/usr/dmr/www/picture.html
- https://www.bell-labs.com/usr/dmr/www/ken-and-den.jpg



16 TB Persistent Disks (Big Disks) on Google Cloud 
- [Super Colliding Nix Stores: Nix Flakes for Millions of Developers](https://blog.replit.com/super-colliding-nix-stores)
- [Under the Hood of Replit with Amjad Masad](https://www.youtube.com/embed/bKhMsQTyzwY?start=1559&end=1690&version=3), start=1559&end=1690




- [The dark and murky past of NixOS (NixCon 2019)](https://www.youtube.com/embed/fsgYVi2PQr0?start=968&end=1201&version=3), start=968&end=1201



Master thesis, doctorates, PhDs:
- Armijn Hemel: [NixOS: the Nix based operating system](https://zenodo.org/records/12906987), https://doi.org/10.5281/zenodo.12906987
- Chris Burr: high energy physics at the University of Manchester, UK and a member of the LHCb, [Chris Burr - Nix for software deployment in high energy physics (NixCon 2018)](https://www.youtube.com/embed/Ee8k97Rx3DA?start=38&end=52&version=3), start=38&end=52
- Eelco Dolstra: [The Purely Functional Software Deployment Model](https://edolstra.github.io/pubs/phd-thesis.pdf), Determinate Systems, [Nix flakes (NixCon 2019)]( https://www.youtube.com/watch?v=UeBX7Ide5a0)
- Eelco Visser: [Syntax Definition for Language Prototyping](https://eelcovisser.org/publications/1997/Visser97.pdf) PhD thesis, University of Amsterdam, [scholar.google.com/citations](https://scholar.google.com/citations?user=1OA7zicAAAAJ&hl=en)
- Farid Zakaria: University of California Santa Cruz, [Java, Nix & Reproducibility](https://fzakaria.com/2021/06/27/java-nix-reproducibility.html)
- Julien Malka: PhD Student at Télécom Paris, https://github.com/JulienMalka
- Jörg Thalheim: [Jörg 'Mic92' Thalheim - About Nix sandboxes and breakpoints (NixCon 2018)](https://www.youtube.com/watch?v=ULqoCjANK-I)
- Pierre-Antoine Bouttier: [Nix as HPC package management system (NixCon 2018)](https://www.youtube.com/watch?v=s5iY3CsdSfQ)
- Sander van der Burg: [Composing FHS-compatible chroot environments with Nix (or deploying Steam in NixOS)](http://sandervanderburg.blogspot.com/2013/09/composing-fhs-compatible-chroot.html), [On Nix, NixOS and the Filesystem Hierarchy Standard (FHS)](http://sandervanderburg.blogspot.com/2011/11/on-nix-nixos-and-filesystem-hierarchy.html), [In memoriam: Eelco Visser (1966-2022)](https://sandervanderburg.blogspot.com/2022/04/in-memoriam-eelco-visser-1966-2022.html)
- Sergei Kozlukov: [Sergei Kozlukov – Deep learning and AI applications in Nixpkgs (2023 Nix Developer Dialogues)](https://www.youtube.com/embed/ZKbTpoM6KkY?start=504&end=540&version=3), start=504&end=540
- Zach Mitchell: Purdue University


Nix is the current technical solution for:
- Google IDX: https://flox.dev/blog/nitw-idx https://idx.dev/blog/article/how-we-built-project-idx-a-high-level-overview https://idx.dev/blog/tag/nix
- Google Looker (GCP): https://flox.dev/blog/nitw-looker
- AWS Cloud9: [Introduction to NixOS - Brownbag by Geoffrey Huntley](https://www.youtube.com/embed/tl9I-R83lKo?start=40&end=57) start=40&end=57, [What if the industry didn’t use Docker? - Geoffrey Huntley, GitPod](https://www.youtube.com/embed/8kZpyCeh4Z8?start=2670&end=2684&version=3), start=2670&end=2684, https://aws.amazon.com/cloud9/
- Replit: [https://blog.replit.com/super-colliding-nix-stores](https://blog.replit.com/super-colliding-nix-stores) [Everything You Need to Know About Nix on Replit in 2 Minutes](https://www.youtube.com/watch?v=gItKAtedmq4) [Replit Pro: All Things Nix](https://www.youtube.com/watch?v=q5paXmDbk7o)
- GitPod: [Workshops as code](https://www.gitpod.io/blog/workshops-as-code)
- Tumblr: [NixOS at Tumblr by Graham Christensen (NixCon 2017)](https://www.youtube.com/watch?v=6VH945-AaRY&t=66s)
- Shopify: [Shipit! Presents: How Shopify Uses Nix](https://www.youtube.com/watch?v=KaIRpx11qrc)
- Canva: [Supporting GPU-accelerated Machine Learning with Kubernetes and Nix](https://canvatechblog.com/supporting-gpu-accelerated-machine-learning-with-kubernetes-and-nix-7c1da8e42f61), By [Jonathon Belotti](https://github.com/thundergolfer) from [Canva Engineering](https://medium.com/@canvatechblog?source=post_page-----7c1da8e42f61--------------------------------)
- Supabase: [Packaging Supabase with Nix](https://www.linkedin.com/posts/supabase_packaging-supabase-with-nix-httpslnkdin-activity-7246606023845638146-Oeyx) [Packaging Supabase with Nix](https://supabase.com/blog/nix-postgres), https://github.com/supabase/nix-postgres, ´[Supabase in this year's Stack Overflow survey amongst the world's most popular Databases](https://www.linkedin.com/posts/supabase_supabase-just-appeared-in-this-years-stack-activity-7222265951780577280-FzYN)
- Obsidian Systems: [Nix Ecosystem and Infra](https://github.com/obsidiansystems/.github/blob/b39bc00072d93115c4ab87e90a226023fa07c810/profile/nix.md#-nix-ecosystem-and-infra)
- D. E. Shaw: https://flox.dev/blog/nix-pure-genius 
- ...
- List: https://github.com/ad-si/nix-companies


Open source based:
- Cachix: https://www.cachix.org/
- Determinate Systems: https://determinate.systems/posts/magic-nix-cache/
- Flox: [Flox 1.1: Time Travel Across 100k+ Nix Packages](https://flox.dev/blog/flox-1.1-blog) 25 June 2024
- Numtide: https://numtide.com/team/
- Serokell: https://serokell.io/blog/what-is-nix#fhs-is-not-suitable-for-reproducible-builds
- Tweag: https://www.tweag.io/blog/tags/nix/


bigboxSWE, [What Your Linux Distro Says About You](https://www.youtube.com/embed/korOpibkm6g?start=99&end=127)
https://youtu.be/korOpibkm6g?t=101

https://www.youtube.com/watch?v=GLp2T7PpsLo


TODO falta o meme do Elon M
No matter what we tried, it was nearly impossible to share layers between multiple builds of Polygott. 
Polygott itself is 20-30GB which adds up quickly when multiple versions are in production at the same time.
- [Will Nix Overtake Docker?](https://blog.replit.com/nix-vs-docker)
- https://github.com/replit/polygott
- https://github.com/replit/prybar
- https://blog.replit.com/nix





    

"Important/famous" people:
- Amjad Masad: [Under the Hood of Replit with Amjad Masad](https://www.youtube.com/embed/bKhMsQTyzwY?start=1527&end=1538&version=3), start=1527&end=1538, [Uber For Brains](https://www.youtube.com/embed/I2UlqaDvbS4?start=0&end=79&version=3)
- Chris Titus: [I was WRONG! This is the BEST Package Manager.](https://www.youtube.com/watch?v=Ty8C2B910EI)
- Geoffrey Huntley: GitPod [Workshops as code](https://www.gitpod.io/blog/workshops-as-code), Canvas, [What if the industry didn’t use Docker? - Geoffrey Huntley, GitPod](https://www.youtube.com/embed/8kZpyCeh4Z8?start=2670&end=2703&version=3), start=2670&end=2703
- Johannes Schickling CEO of Prisma https://flox.dev/blog/nitw-prisma [Setting up Nix on macOS from scratch (incl. dotfiles via home-manager and Nix flakes)](https://www.youtube.com/watch?v=1dzgVkgQ5mE)
- Jon Seager: Vice President of Engineering at Canonical, [Nerding out about Nix and NixOS with Jon Seager, Canonical](https://www.youtube.com/embed/9l-U2NwbKOc?start=321&end=413&version=3), start=321&end=413
- Josh Rosso: Principal Software Engineer at Reddit | Author of Production Kubernetes, [Nix Kubernetes and the Pursuit of Reproducibility](https://www.youtube.com/embed/U-mSWU4see0?start=1997&end=2004&version=3), start=1997&end=2004
- Justin Cormack: Docker CTO, [Building for Builders through Open Source | Ron Efroni & Justin Cormack](https://www.youtube.com/embed/BiF0wyclCPc?start=1493&end=1540&version=3), start=1493&end=1540
- Jérôme Petazzoni: [Jérôme Petazzoni - Creating Optimized Images for Docker and Kubernetes | #FiqueEmCasaConf ](https://www.youtube.com/embed/UbXv-T4IUXk?start=838&end=877&version=3), start=838&end=877
- Michael Brantley: [Nix Friday - [interview] floxdev](https://www.youtube.com/embed/qqzO0asKSzY?start=678&end=820&version=3), start=678&end=820
- Mitchell Hashimoto: Co-founder and CTO of HashiCorp, [NixOS VM on Mac Setup](https://www.youtube.com/embed/ubDMLoWz76U?start=502&end=543&version=3), start=502&end=543
- Ross Turk: former, SourceForge, Red Hat, npm, Talend, InkTank, [NixCon2023 Nix in the Wild](https://www.youtube.com/embed/Q4oUPmPPED0?start=144&end=160&version=3), start=144&end=160, [NixCon2023 Nix in the Wild](https://www.youtube.com/embed/Q4oUPmPPED0?start=198&end=276&version=3), start=198&end=276 
- Ryan Mulligan: [NixCon2023 Declaring an IDE with evalModules](https://www.youtube.com/embed/WsU7sQvIh0U?start=234&end=280&version=3), start=234&end=280
- Savanni D’Gerinel: Linux Desktop Technical Lead on 1Passwd, [1Password Developer Fireside Chat: An Overview of Nix & NixOS](https://www.youtube.com/watch?v=aivf96LUIdo)
- The Linux Experiment: [NIX OS: the BEST package manager on the MOST SOLID Linux distribution](https://www.youtube.com/watch?v=DMQWirkx5EY)
- Viktor Farcic: DevOps Toolkit, [Say Goodbye to Containers - Ephemeral Environments with Nix Shell](https://www.youtube.com/watch?v=0ulldVwZiKA)
- Vladimir Kryachko: Staff Software Engineer Google 8.5y, https://flox.dev/blog/nitw-idx
- Ádám Szücs-Mátyás: Principal Architect at LastPass, [short: From Kubernetes to Nix](https://www.youtube.com/shorts/CDGFY3TlAoc), [From Kubernetes to Nix](https://www.youtube.com/watch?v=cxMbpQom45I)



Nix people, experts/all in/fanatic:
- Domen Kožar: https://www.cachix.org/about
- Geoffrey Huntley: GitPod, Canvas
- Graham Christensen: Tumblr, CEO and fouder Determinate Systems 
- Jonas Chevalier: [Packaging microservices with nix - Jonas Chevalier](https://www.youtube.com/embed/wZ1PECH_cfM?start=33&end=41&version=3), start=33&end=41 
- Matthew Croughan: [Stop Using AI as a Service - (KoboldAI, InvokeAI, Nixified.AI)](https://www.youtube.com/watch?v=wJ0D7MrPNOw), [The Nix Phone and the end of Android](https://www.youtube.com/watch?v=0UIpg19KECw)
- Rok Garbas: python brasil 9, 2013, [Nix, you'll be wondering why you haven't been using it before](https://www.youtube.com/watch?v=LvjaWiL3BQA)
- Ryan Mulligan: Developer Experience Engineer at Replit: [Replit Pro: All Things Nix](https://www.youtube.com/watch?v=q5paXmDbk7o)
- Silvan Mosberger: Tweag +80 aulas [The Nix Hour](https://www.youtube.com/playlist?list=PLyzwHTVJlRc8yjlx4VR4LU5A5O44og9in)



Unique things that I have found along the years
- 


TODO
Asko Soukka - Beyond Python packaging with Nix
https://www.youtube.com/watch?v=Vnq6ngcqJAg&t=740s


Unique explanations abbout what "Nix" is:

Focused in "nix store" vs FHS:
- https://www.youtube.com/embed/IrneGNN3e6c?start=324&end=392&version=3
- https://www.youtube.com/embed/6iviTZfiLGU?start=1395&end=1406&version=3
- https://www.youtube.com/embed/6iviTZfiLGU?start=448&end=489&version=3
- [NixCon2023 Nix in Space](https://www.youtube.com/embed/GNsHIN6SYkE?start=262&end=278&version=3), start=262&end=278

Focused in Nix/nixpkgs/NixOS:
- [Robotnix - Build Android (AOSP) using Nix - Daniel Fullmer](https://www.youtube.com/watch?v=tj8t0aRaUro)
- [Bonus nix shell benefit I didn't expect](https://www.youtube.com/watch?v=QsnBpM3ZSO8)
- [Nerding out about Nix and NixOS with Jon Seager, Canonical](https://www.youtube.com/embed/9l-U2NwbKOc?start=114&end=227&version=3)



nix \
shell \
nixpkgs#auditwheel \
nixpkgs#binutils.out \
nixpkgs#glibc.bin \
nixpkgs#patchelf \
nixpkgs#poetry \
nixpkgs#python3Packages.pip \
nixpkgs#python3Packages.wheel \
nixpkgs#python3Packages.wheel-filename  \
nixpkgs#python3Packages.wheel-inspect \
nixpkgs#python3Packages.packaging \
nixpkgs#python3Packages.ffmpeg \
nixpkgs#twine \
nixpkgs#patchelf \
nixpkgs#coreutils  \
nixpkgs#glibc.bin \
nixpkgs#which \
nixpkgs#file \
nixpkgs#python3Full \
 --command \
sh -c 'ldd "$(which python3)"'



ls -alh pandas-*/pandas/_libs/*.so


wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.numpy.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.numpy.pname)-$(nix eval --raw nixpkgs#python3Packages.numpy.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'



wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.pandas.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.pandas.pname)-$(nix eval --raw nixpkgs#python3Packages.pandas.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'



wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.polars.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.polars.pname)-$(nix eval --raw nixpkgs#python3Packages.polars.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'


wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.scipy.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.scipy.pname)-$(nix eval --raw nixpkgs#python3Packages.scipy.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'



wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.sympy.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.sympy.pname)-$(nix eval --raw nixpkgs#python3Packages.sympy.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'


astropy
PNAME=psycopg2

PNAME=pytorch
wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.$PNAME.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.$PNAME.pname)-$(nix eval --raw nixpkgs#python3Packages.$PNAME.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'


PNAME=pyspark
wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.$PNAME.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.$PNAME.pname)-$(nix eval --raw nixpkgs#python3Packages.$PNAME.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'


wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.scikitlearn.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.scikitlearn.pname)-$(nix eval --raw nixpkgs#python3Packages.scikitlearn.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'



wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.cryptography.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.cryptography.pname)-$(nix eval --raw nixpkgs#python3Packages.cryptography.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'



wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.geopandas.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.geopandas.pname)-$(nix eval --raw nixpkgs#python3Packages.geopandas.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'



wheel \
unpack \
$(nix build --no-link --print-out-paths --print-build-logs nixpkgs#python3Packages.tensorflow.dist)/*

DIRETORY_NAME=$(nix eval --raw nixpkgs#python3Packages.tensorflow.pname)-$(nix eval --raw nixpkgs#python3Packages.tensorflow.version)
cd "$DIRETORY_NAME"

find . -type f -iname '*.so'




Trees vs DAGs
Boble sort vs Merg sort
Big O(n^2) vs O(n*logs(n)) 
FHS vs Nix store




- python3Packages
- python311Packages
- python312Packages
- python313Packages
- cudaPackages
- xorg
- pkgsMusl
- pkgsStatic
- pkgsCross
- glibcLocalesUtf8
- aspellWithDicts
- androidenv.composeAndroidPackages
- (nerdfonts.override { fonts = [ "FiraCode"]; })


nix build nixpkgs#pkgsCross.aarch64-multiplatform-musl.pkgsStatic.hello




Minhas contribuições ao nixpkgs:



https://github.com/NixOS/nixpkgs/pulls?q=is%3Apr+author%3APedroRegisPOAR+
https://github.com/NixOS/nixpkgs/pulls?q=is%3Apr+is%3Aissue+author%3APedroRegisPOAR+
