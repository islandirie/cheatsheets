# Colorizing ls Output
alias ls='ls -G'  # Enable colorized output for ls
alias ll='ls -alF'  # List all files with color coding and additional details

# Customizing Prompt
export PS1="\[\e[36m\]\u@\h \[\e[32m\]\w\[\e[0m\]\$ "  # Custom prompt with username, hostname, and current directory

# Aliases for Navigation
alias c='cd'  # Shortcut for 'cd'
alias ..='cd ..'  # Go up one directory
alias ...='cd ../..'  # Go up two directories

# Alias for Clearing the Screen
alias cls='clear'  # Clear the screen

# Alias for Opening Files or Directories
alias o='open'  # Open file or directory with default application

# Colorizing grep Output
alias grep='grep --color=auto'  # Enable colorized output for grep

