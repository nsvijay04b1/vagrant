# learning vagrant .....

# What is vagrant as per [wikipedia](https://en.wikipedia.org/wiki/Vagrant_(software))

Vagrant is an open-source software product for building and maintaining portable virtual development environments. The core idea behind its creation lies in the fact that the environment maintenance becomes increasingly difficult in a large project with multiple technical stacks. Vagrant manages all the necessary configurations for the developers in order to avoid the unnecessary maintenance and setup time, and increases development productivity. Vagrant is written in the Ruby language, but its ecosystem supports development in almost all major languages.

# Common Vagrant Commands

vagrant up -- starts vagrant environment (also provisions only on the FIRST vagrant up).

vagrant status -- outputs status of the vagrant machine .

vagrant halt -- stops the vagrant machine.

vagrant reload -- restarts vagrant machine, loads new Vagrantfile configuration.

vagrant provision -- forces reprovisioning of the vagrant machine.

vagrant ssh -- connects to machine via SSH.

vagrant destroy -- stops and deletes all traces of the vagrant machine.

# Tips

vagrant -v -- Get the vagrant version.

vagrant global-status -- outputs status of all vagrant machines.

vagrant global-status --prune -- same as above, but prunes invalid entries.

vagrant suspend -- Suspends a virtual machine (remembers state).

vagrant resume -- Resume a suspended machine (vagrant up works just fine for this as well).

vagrant reload --provision -- Restart the virtual machine and force provisioning.

vagrant provision --debug -- Use the debug flag to increase the verbosity of the output.

vagrant push -- Yes, vagrant can be configured to deploy code!.

vagrant up --provision | tee provision.log -- Runs vagrant up, forces provisioning and logs all output to a file


# Notes

If you are using VVV, you can enable xdebug by running vagrant ssh and then xdebug_on from the virtual 
