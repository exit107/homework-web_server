# Contributing

## What you need:
* A workstation with either Docker installed
* Git
* Ansible
* [Molecule](https://molecule.readthedocs.io/en/latest/)

## What you need to know:
* All testing and development is done via Molecule
* Right now, the only OS being supported is Ubuntu 18.04

## To develop the role:
1. Clone the `homework-web_server` repo with git.
  * `git clone https://github.com/exit107/homework-web_server.git`
2. Change into the repository directory
  * `cd homework-web_server`
3. Run the command `molecule converge`. This will pull a Docker container, start it, and run the role against it.
4. Make changes to the role.
5. After making changes to the role, run `molecule converge` again to see the effect it has.

## To test the role:
1. Clone the `homework-web_server` repo with git.
  * `git clone https://github.com/exit107/homework-web_server.git`
2. Change into the repository directory
  * `cd homework-web_server`
3. Run the command `molecule test`

### Notes:
* The command `molecule login` will ssh into the running container so you can examine the environment.
* [An excellent guide to developing with Molecule](https://www.jeffgeerling.com/blog/2018/testing-your-ansible-roles-molecule) was written by Jeff Geerling. I highly recommend reading it before beginning to work on this role.

