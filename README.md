Variables:
Variables allow us to store values that we can re use accross the ansible playbook
ansible by default comes with variables for the hosts that we are able to connect to, they are also called "facts"
two of those variables, are ansible_hostname and ansible_distribution among many others
You can see these variables above by using the setup module in an adhoc command > ansible node_1 -m setup -i hosts.ini


Another thing to note about playbooks are what we call conditionals:

Conditionals allow us to run specific tasks if the condition is true otherwise it will not run > when ansible_distribution == "Ubuntu" or ansible_distribution == "Debian"