La web de @hablemosquechua
===============

Esta web usa [gh-pages](http://pages.github.com/) para ser hosteada, es por eso que para poder
verla de manera local, es necesario instalar [ruby](https://www.ruby-lang.org)
y [`jekyll`](http://jekyllrb.com/)

### Dependencias
Para instalar ruby en ubuntu
```
sudo apt-get install ruby
```

Luego desde el root de este proyecto se ejecuta 
```
gem install bundle
bundle install
```
para instalar todas las dependencias.

### Ejecución
Una vez instaladas todas las dependencias podemos empezar a actualizar la página, sólo tienes
que ejecutar
```
jekyll serve -w
```
Y la página correra localmente en [localhost:4000](http://localhost:4000)

El flag `-w` (watch) le dice a jekyll que actualice la página cada vez que hay un cambio.

### Deploy
Como [hablemosquechua.org](http://hablemosquechua.org) está hosteada en [github](https://github.com)
es necesario q al hacer un push con código al servidor, este también actualice el branch `gh-pages`,
para ello usamos [este truco](http://brettterpstra.com/2012/09/26/github-tip-easily-sync-your-master-to-github-pages/)
