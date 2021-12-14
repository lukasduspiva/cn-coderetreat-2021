# CN Coderetreat 2021 - ONLINE

## Requirements

Base requirements for participating are:

- 💻 Notebook/PC
- ⚡ Stable internet connection
- 🎥 Webcam and microphone (preferably a quite place)
- ✍️ Have prepared empty project where you can write tests rightaway

### Tools

Any participant should prepare for pairing with a developer of any platform. Therefore a couple of extra tools should be ready for use. Here is the categorized list:

**IDE Built-In Tools**

| IDE | Host Participant Requirement | Any Participant Requirements |
|:---:|:----:|:-----:|
|IntelliJ IDEA, WebStorm, AppCode & Android Studio | Installation + [Code with Me Plugin](https://plugins.jetbrains.com/plugin/14896-code-with-me) | - |
| VS Code | Installation + [Live Share Plugin](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare) | Installation + [Live Share Plugin](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare) |

**Worst-Case Scenario Tools**

- `git`

## Agenda

| Time          | What is happening? 🤔 | 
|:--------------|:----------------------|
| before 09:00  | Participants arriving to meeting |
| 09:00 - 09:30 | Welcome, introduction and overview of what is going to happen |
| 09:30 - 10:30 | **Session # 1** (_Pair Programming_ and _Game of Life_ explained) |
| 10:30 - 10:45 | Retrospective + short break |
| 10:45 - 11:45 | **Session # 2** (_Test Driven Development_ explained)|
| 11:45 - 12:00 | Retrospective |
| 12:00 - 13:15 | Lunch + socializing (big break) 🍕 |
| 13:15 - 14:15 | **Session # 3** (_4 Rules of Simple Design_ explained) |
| 14:15 - 14:30 | Retrospective + short break |
| 14:30 - 15:30 | **Session # 4** |
| 15:30 - 15:45 | Retrospective + short break |
| 15:45 - 16:45 | **Session # 5** |
| 16:45 - 17:00 | Closing circle retrospective |

## Sessions

Random and for each session unique pairs are generated based on [Stupid Sort](https://en.wikipedia.org/wiki/Stupid_sort) algorithm utilizing **Mulberry32** random number generator with seed `12`.


### Session # 1

|       #       | Participant A | Participant B | Pair Space |
| :-----------: | :-----------: |:-------------:| :---------:|
| 1 | Zdeněk B. | Róbert J. | [meeting room](https://hangouts.google.com/call/Z4bgiI56eIARj9BGypxyACEI?no_rd) + [paper](https://onthesamepage.online/CN-CODERETREAT-2021-1-0-1639469600536) |
| 2 | Martin L. | Martin K. | [meeting room](https://hangouts.google.com/call/Z7StD6iLyPMNMn3GNl24ACEI?no_rd) + [paper](https://onthesamepage.online/CN-CODERETREAT-2021-1-1-1639469600536) |
| 3 | Filip M. | Petr J. | [meeting room](https://hangouts.google.com/call/Sby41nQmIvpfRpQEektWACEI?no_rd) + [paper](https://onthesamepage.online/CN-CODERETREAT-2021-1-2-1639469600536) |
| 4 | Kateřina K. | Jiří K. | [meeting room](https://hangouts.google.com/call/O33OXx57WIobEoYi_61EACEI?no_rd) + [paper](https://onthesamepage.online/CN-CODERETREAT-2021-1-3-1639469600536) |
| 5 | Martin M. | Filip O. | [meeting room](https://hangouts.google.com/call/EEW2cquAKJMB0Jb788emACEI?no_rd) + [paper](https://onthesamepage.online/CN-CODERETREAT-2021-1-4-1639469600536) |

## Game of Life

### Rules

1. Any live cell with fewer than two live neighbors dies, as if by underpopulation.
2. Any live cell with two or three live neighbors lives on to the next generation.
3. Any live cell with more than three live neighbors dies, as if by overpopulation.
4. Any dead cell with exactly three live neighbors becomes a live cell, as if by reproduction.

For more information visit the [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life) page at Wikipedia.

#### Rule # 1

`generation x` `(n < 2)`
| ⬜ | ⬜ | ⬜ |
|:---:|:---:|:---:|
| ⬜ | 🦠 | ⬜ |
| ⬜ | ⬜ | 🦠 |

`generation x + 1`
| ❔ | ❔ | ❔ |
|:---:|:---:|:---:|
| ❔ | ⬜ | ❔ |
| ❔ | ❔ | ❔ |

#### Rule # 2

`generation x` `(n = 2,3)`
| ⬜ | ⬜ | ⬜ |
|:---:|:---:|:---:|
| 🦠 | 🦠 | ⬜ |
| ⬜ | 🦠 | 🦠 |

`generation x + 1`
| ❔ | ❔ | ❔ |
|:---:|:---:|:---:|
| ❔ | 🦠 | ❔ |
| ❔ | ❔ | ❔ |

#### Rule # 3

`generation x` `(n > 3)`
| 🦠 | 🦠 | 🦠 |
|:---:|:---:|:---:|
| 🦠 | 🦠 | 🦠 |
| 🦠 | 🦠 | 🦠 |

`generation x + 1`
| ❔ | ❔ | ❔ |
|:---:|:---:|:---:|
| ❔ | ⬜ | ❔ |
| ❔ | ❔ | ❔ |


#### Rule # 4

`generation x` `(n = 3)`
| ⬜ | ⬜ | ⬜ |
|:---:|:---:|:---:|
| 🦠 | ⬜ | ⬜ |
| ⬜ | 🦠 | 🦠 |

`generation x + 1`
| ❔ | ❔ | ❔ |
|:---:|:---:|:---:|
| ❔ | 🦠 | ❔ |
| ❔ | ❔ | ❔ |

