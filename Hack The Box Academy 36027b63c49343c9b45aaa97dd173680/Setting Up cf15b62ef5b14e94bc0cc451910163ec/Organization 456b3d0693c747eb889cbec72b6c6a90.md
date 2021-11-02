# Organization

## # Password Manager

There are only three problems with Password Manager :

- Complexity
- Re-use
- Remembering

### complexity

Nord-Pass has created the list of most commonly used passwords [common passwords](https://nordpass.com/most-common-passwords-list/). So we can guess password without any special preparation.

## #### Re-usage

Once the user has created the complex password, there are two problems generated :

- Remembering a complex and hard to guess password is still within the realm of possibility for a standard user.
- This passwo(rd is then use for all services, which allows us to work across several component of the company’s infrastructure.

**Prevention** – The user will have to create and remember complex passwords *for all* services used.

## ### Note Taking

1. **Discovering tools** – IP address, usernames, passwords, source code.
2. **Ideas for further test and processing** – Habit of Noting down everything (obsidian and xmind)
3. **Scan Results** – we use **Ghostwriter and Pwndoc.**
4. **Logging** – tools are used in **script and date**

```
`PS1="\[\033[1;32m\]\342\224\200\$([[ \$(/opt/vpnbash.sh) == *\"10.\"* ]] && echo \"[\[\033[1;34m\]\$(/opt/vpnserver.sh)\[\033[1;32m\]]\342\224\200[\[\033[1;37m\]\$(/opt/vpnbash.sh)\[\033[1;32m\]]\342\224\200\")[\[\033[1;37m\]\u\[\033[01;32m\]@\[\033[01;34m\]\h\[\033[1;32m\]]\342\224\200[\[\033[1;37m\]\w\[\033[1;32m\]]\n\[\033[1;32m\]\342\224\224\342\224\200\342\224\200\342\225\274 [\[\e[01;33m\]$(date +%D-%r)\[\e[01;32m\]]\\$ \[\e[0m\]"`
```

**script** – <date>-<start time>-<name>.log

1. **Screenshots** – for this we can use [flameshot](https://github.com/flameshot-org/flameshot) flameshot also has apt package and [Peek](https://github.com/phw/peek) for gifs.

### Container

- Docker
- Vagrant