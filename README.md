# romainfavier.github.io

atc123@Linux-Fav:/home$ mkdir sites <-- création du fichier sites dans home

atc123@Linux-Fav:/home$ sudo chmod 777 sites <-- changement des droits d'accès sur sites

atc123@Linux-Fav:/home$ cd sites <-- positionnement dans sites

atc123@Linux-Fav:/home/sites$ pwd
/home/sites

atc123@Linux-Fav:/home/sites$ sudo apt-get install Jekyll <-- Téléchargement de Jekyll en root
[sudo] password for atc123: 

After this operation, 52,5 MB of additional disk space will be used.
Do you want to continue? [Y/n] y <-- Comfirmer pour installer

Processing triggers for libc-bin (2.21-0ubuntu4) ... <-- installation réussite.

atc123@Linux-Fav:/home/sites$ jekyll new blog <-- Création d'un blog dans sites
New jekyll site installed in /home/sites/blog. 
atc123@Linux-Fav:/home/sites$ cd blog 
atc123@Linux-Fav:/home/sites/blog$ jekyll serve <-- lancement du serveur
Configuration file: /home/sites/blog/_config.yml
            Source: /home/sites/blog
       Destination: /home/sites/blog/_site
      Generating... 
                    done.
Configuration file: /home/sites/blog/_config.yml
    Server address: http://0.0.0.0:4000/
  Server running... press ctrl-c to stop.

atc123@Linux-Fav:/home/sites/blog$ sudo apt-get install ruby-full <-- installation Ruby (debian/Ubuntu)
 
atc123@Linux-Fav:/home/sites/blog$ sudo apt-get install rubygems <-- installation de ruby gems pour effetuer l'update de jekyll
atc123@Linux-Fav:/home/sites/blog$ sudo gem update --system <-- mise à jour de rubygems
RubyGems system software updated

atc123@Linux-Fav:/home/sites/blog$ sudo gem install rubygems-update
atc123@Linux-Fav:/home/sites/blog$ update_rubygems <-- Update Rubygems

atc123@Linux-Fav:/home/sites/blog$ sudo apt-get install ruby2.0.0-dev

atc123@Linux-Fav: sudo gem update jekyll 2.4.0