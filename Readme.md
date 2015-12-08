### Usage Shellout agent:

The Shellout agent allows concurrent remote execution of arbitrary shell
commands.  I hope that sounds as scary as I mean it to sound.  You need to make
sure you give due diligence to security on the clients that have access to this
agent.

Example usage 1 (outputs STDOUT):

     sudo mco rpc shellout cmd cmd='for i in $(seq 1 10);do echo $i;done'

Example usage 2 (outputs STDERR):

     sudo mco rpc shellout cmd cmd='ls -l /home/jbeiber/awesome-songs.txt'
