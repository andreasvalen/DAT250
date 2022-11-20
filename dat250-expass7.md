# Excercise 

### Report

## Experiment 1

I had to upgrade Erlang from version 24.0 to 25.0

## Experiment 2

Everything went smooth appart from the "Putting it all together" step.

I was unable to compile the classes into jar files with the RabbitMQ java client.

## Experiment 3

As I was unable to create the jar files, I just ran the classes in the IDE.

Running "NewTask" and passing arguments:
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/run-with-args.PNG?raw=true)

Had troubles with the "rabbitmqctl.bat list_queues name messages_ready messages_unacknowledged" command where rabbitmqctl.bat was not executable.
- Soultion: removed ".bat" and it worked

Workers in action:
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/worker-1.PNG?raw=true)
![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/worker-2.PNG?raw=true)

## Experiment 4

Everything went smooth.

![db screenshot](https://github.com/andreasvalen/DAT250/blob/main/resources/imgs/exchanges.PNG?raw=true)








Link to code for all experiments: https://github.com/andreasvalen/expass7
