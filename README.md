# Karabiner Config

Shared [Karabiner-Elements](https://karabiner-elements.pqrs.org/) configuration synced across Macs via Git.

## Setup on a new Mac

```bash
git clone https://github.com/andriibuda/karabiner-config.git ~/dotfiles/karabiner-config
mv ~/.config/karabiner ~/.config/karabiner.bak
ln -s ~/dotfiles/karabiner-config ~/.config/karabiner
```

Karabiner-Elements will pick up the symlinked config automatically.

## Syncing changes

After editing your config (via Karabiner UI or manually):

```bash
cd ~/dotfiles/karabiner-config
git add -A && git commit -m "Update config" && git push
```

On the other Mac:

```bash
cd ~/dotfiles/karabiner-config && git pull
```
