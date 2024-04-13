# Linux Packages

---

### tldr
 Simplified, example based and community-driven man pages
https://github.com/dbrgn/tealdeer

- Installation
    
    ```bash
    $ sudo apt-get install tealdeer
    $ tldr --update
    ```
    
- How to use
    
    ```bash
    $ tldr [app]
    ```
    
    For example, if you want to search for “top” command:
    
    ```bash
    $ tldr top
    
      Display dynamic real-time information about running processes.
      More information: <https://manned.org/top>.
    
      Start `top`:
    
          top
    
      Do not show any idle or zombie processes:
    
          top -i
    
      Show only processes owned by given user:
    
          top -u username
    
      Sort processes by a field:
    
          top -o field_name
    
      Show the individual threads of a given process:
    
          top -Hp process_id
    
      Show only the processes with the given PID(s), passed as a comma-separated list. (Normally you wouldn't know PIDs off hand. This example picks the PIDs from the process name):                                                                   
    
          top -p $(pgrep -d ',' process_name)
    
      Display help about interactive commands:
    
          ?
    
    ```
    

### **fzf**
**fzf is a general-purpose command-line fuzzy finder**

https://github.com/junegunn/fzf

- Installation
    
    ```jsx
    apt install fzf
    ```
    

### bat
**A *cat* clone with syntax highlighting and Git integration**

https://github.com/sharkdp/bat

![Untitled](Linux%20Packages%207e6f0214d7514bed87aaacad585e28a2/Untitled.png)