# cheatsheet-tmux-A4
<a href="https://github.com/DennyZhang?tab=followers"><img align="right" width="200" height="183" src="https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/fork_github.png" /></a>

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![LinkedIn](https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/linkedin.png)](https://www.linkedin.com/in/dennyzhang001) <a href="https://www.dennyzhang.com/slack" target="_blank" rel="nofollow"><img src="http://slack.dennyzhang.com/badge.svg" alt="slack"/></a> [![Github](https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/github.png)](https://github.com/DennyZhang)

File me [tickets](https://github.com/DennyZhang/cheatsheet-tmux-A4/issues) or star [the repo](https://github.com/DennyZhang/cheatsheet-tmux-A4).

See more CheatSheets from Denny: [here](https://github.com/topics/denny-cheatsheets)

Table of Contents
=================

   * [cheatsheet-tmux-A4](#cheatsheet-tmux-a4)
      * [Tmux Basic](#tmux-basic)
      * [Tmux Layout &amp; Scroll](#tmux-layout--scroll)
      * [Tmux Console Output](#tmux-console-output)
      * [Tmate](#tmate)
   * [More links](#more-links)

<a href="https://www.dennyzhang.com"><img align="right" width="185" height="37" src="https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/dns_small.png"></a>
  
## Tmux Basic

| Name                   | Comment                                |
| :--------------------- | -------------------------------------- |
| Create new session     | `tmux new -s denny`                    |
| List all sessions      | `tmux ls`                              |
| Attach to one session  | `tmux attach -t denny`                 |
| Detach session         | `C-b d`                                |
| Kill one session       | `tmux kill-session -t denny`           |
| List all shortcut keys | `C-b :list-keys`, `C-b ?` Very useful! |
| Kill current window    | `C-b &`                                |
| Default conf file      | `~/.tmux.conf`, `~/.tmate.conf`        |

## Tmux Layout & Scroll

| Name                      | Comment                   |
| :---------------------    | ------------------------- |
| Switch to next pane       | `C-b o`                   |
| Vertically split pane     | `C-b %`                   |
| Horizontally split pane   | `C-b "`                   |
| Kill current pane         | `C-b x`                   |
| Swap two panes            | `C-b C-o`                 |
| Resize current pane right | `C-b :resize-pane -R 20`  |
| Resize current pane down  | `C-b :resize-pane -D 10`  |

## Tmux Console Output

| Name                          | Comment                                          |
| :---------------------------  | ------------------------------------------------ |
| Enter copy mode               | `C-b [`, press q/Esc to exit                     |
| Search output                 | `C-b C-s`, `C-b C-u`                             |
| Paste buffer to current panel | `C-b]`                                           |
| Page up/down                  | Enter copy mode, then use normal navigation keys |
| Show things in current buffer | `tmux show-buffer`                               |
| List all buffer               | `tmux list-buffers`                              |
| Save buffer to file           | `tmux save-buffer foo.txt`                       |

## Tmate

| Name                                           | Comment                                                                       |
| :--------------------------------------------- | ----------------------------------------------------------------------------- |
| see tmate log messages: ssh conn string        | `tmate show-messages`                                                         |
| Launch tmate in a detached state               | `tmate -S /tmp/tmate.sock new-session -d`                                     |
| Blocks until the SSH connection is established | `tmate -S /tmp/tmate.sock wait tmate-ready`                                   |
| Prints the SSH connection string               | `tmate -S /tmp/tmate.sock display -p '#{tmate_ssh}'`                          |
| Make your tmate session big by default         | [Make your default iterm window big](https://apple.stackexchange.com/a/98406) |

# More links

```
https://gist.github.com/MohamedAlaa/2961058
https://wiki.freebsdchina.org/software/t/tmux
```

- TODO: Need to automatically generate pdf

- License: Code is licensed under [MIT License](https://www.dennyzhang.com/wp-content/mit_license.txt).

<a href="https://www.dennyzhang.com"><img align="right" width="201" height="268" src="https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/denny_201706.png"></a>

<a href="https://www.dennyzhang.com"><img align="right" src="https://raw.githubusercontent.com/USDevOps/mywechat-slack-group/master/images/dns_small.png"></a>
