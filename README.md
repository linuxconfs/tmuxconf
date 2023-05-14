# tmuxconf

## Docs

https://tmuxcheatsheet.com/

```bash
# 清理sessions，匹配以 不是0:的sessions, kill掉。
tmux ls | grep -v $(tmux display-message -p '#S'): | cut -d: -f1 | xargs -n1 tmux kill-session -t
```

## Requirements

### [fzf](https://github.com/junegunn/fzf/) (need by tmux-fzf plugin)

`sudo apt install fzf`

## Optional 
`sudo ln -s ~/tmuxconf/clipboard-provider /usr/bin/clipboard-provider`

## Plugin list

[plugin recommendation list](https://github.com/tmux-plugins/list)

| 序号 | 插件 | 作用 | 快捷键 |
| :---: | :--- | :--- | :--- |
| 1 | resurrect | restore current workspace after system restart | <C-s>, <C-r>  |
| 2 | continuum | auto reload resurrect stored contents | - |
| 3 | [dracula/tmux](https://draculatheme.com/tmux) | a popular theme | - |
| 4 | tmux.nvim | plugin for nvim, navigator, resize, copy paste | <C-j/k/h/l>, <A-j..> |
| 5 | tmux-fzf | manager multiple sessions | <F>, <TAB>, <S-TAB>, menu |

