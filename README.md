# node-event-and-message-bus
The Direktspeed Event and Message Bus is a Ultra High Performance SDK for building distributed scaleable systems and software.

# Diffrent types of Events.
- Eventual Consistent
- Replicated at last X
- At last Once

# Diffrent Protocols and Message Bus Integrations
node-event-and-message-bus is able to integrate the following services
- systemd 
- docker
- syslog
- filesystem
- databases
  - mysql via diffrent implamentations
  - couchbase via diffrent implamentations
  - postgree sql
  - sqllite
  - Custom Implamentations.
  - many more .....
- Includes Healthcheck.
- Includes Polics Enforcment
- Can act as Autonom SystemAdministrator and Deployment System
- Can Manage AutoScaling 
- Can do all work that a Human needs to do on Regular Basis
- Fully AI Connected.


# Learn how to connect a PHP Application to node-event-and-message-bus
Here you learn how to integrate into a PHP Application.


## Implament a FileBased Message bus
You can Easy Implament a filebased message bus via POSIX *nix 
- Server
  - Create a RAM DISK at last 5 MB
  - write index in /mnt/ramdisk contains files in /ramdisk
  - if index gets to big reduce it via commands > concat files to persistent location
  - in index reference other files to tail 
  - expose /mnt/persistent and /mnt/ramdisk
- Client
  - tail -f index
  - tail -f every file in index (Do It Loosy if the file don't exists simply stop tailing)
  
