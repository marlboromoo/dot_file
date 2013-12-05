# Marlboromoo's dot files
Just marlboromoo's dot files.
```
    ___  ___           _ _                    ___  ___
    |  \/  |          | | |                   |  \/  |
    | .  . | __ _ _ __| | |__   ___  _ __ ___ | .  . | ___   ___
    | |\/| |/ _` | '__| | '_ \ / _ \| '__/ _ \| |\/| |/ _ \ / _ \
    | |  | | (_| | |  | | |_) | (_) | | | (_) | |  | | (_) | (_) |
    \_|  |_/\__,_|_|  |_|_.__/ \___/|_|  \___/\_|  |_/\___/ \___/ 's dot files

```

## Installation

### Dependency 
```
#. conky
sudo aptitude install ttf-ubuntu-font-family hddtemp curl lm-sensors conky-all

#. powerline
sudo easy_install https://github.com/Lokaltog/powerline/archive/develop.zip
find  $(echo 'import site; print site.getsitepackages()[0]' | python ) | grep -i powerline.conf$
```

### Dot files
```
cd ~
git clone https://github.com/marlboromoo/dot_file.git
for file in .conkyrc .conky .tmux.conf .tmuxline.conf; do
    mv $file{,.bak} 2>/dev/null
    ln -s dot_file/$file ./
done
```

