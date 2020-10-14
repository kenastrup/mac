# Ken sin mac
Denne er opprettet for å kunne restore macen raskere

Består av Brewfile og Keyboard Layouts.

Brewfile er manuelt kopiert hit. Er det mulig å symlinke den, tro?


## Pimpe opp zsh

Jeg bruker [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh) for å pimpe shellet.

### Install oh-my-zsh 
```shell script
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Endre theme
Når `oh-my-zsh` er installert, endre dette i `$HOME/.zshrc`

```shell script
# For å fjerne user@host fra prompt
export DEFAULT_USER=$USER
prompt_context(){} 

# Velge theme
ZSH_THEME="agnoster"

# Velge plugins
plugins=(git 
  direnv 
  docker 
  docker-compose 
  extract 
  httpie 
  iterm2
  jira
  thefuck
  z
)
```

### Endre font til en theme vennlig font

#### installere powerline fonts
Themet trenger powerline fonts

```
git clone https://github.com/powerline/fonts
cd fonts
./install.sh
```

#### Endre fonten i terminal/iterm2 
Her bruker jeg `Meslo LG L DZ for powerline` regular 14pt
