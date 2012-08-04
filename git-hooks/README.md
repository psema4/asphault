## Sample git hooks

1. Edit the hooks, replacing {Your-Email-Here} with your email address
1. Copy into your .git/hooks folder and make them executable:
 * `cd ~/devel/asphault`
 * `cp git-hooks/build-* ./.git/hooks/`
 * `chmod u+x .git/hooks/build-*`
1. Update them with an email address to notify.  Be sure to escape the @:
 * `perl -pi -e 's/\{Your-Email-Here\}/`username\@host.com`/g' .git/hooks/build-*

## Requires

 * mail (Ubuntu: `sudo apt-get install mailutils`)

