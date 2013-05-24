jcli
====

A Simple JIRA Command Line Interface

### Setup:
```
git clone https://github.com/dwinstanley/jcli.git   
pip install requests 
pip install jira-python
```

Edit .jcli with your JIRA setup and place it in your home directory.   

### Usage examples:

Resove an issue (with time taken and resolution):   
`devbox:~]$ jcli -k SUPPORT-123 -t Resolved -T 15m -r Fixed`

Assign an issue:   
`devbox:~]$ jcli -k SUPPORT-123 -a jira.user`

Search for an issue (using JQL):   
`devbox:~]$ jcli -s "assignee = jira.user and status = open"`

List an issue description:   
`devbox:~]$ jcli -k SUPPORT-123 -d`

### .jcli

Edit options section to your own JIRA server setup and login credentials

Add JQL favourite shortcuts to the favourites section eg:   
`mytix = assignee = some.user status = open`

Note that no quotes are needed here. Crazy.

### Finally

There will be bugs! It's very early days!
