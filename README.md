# workflow_automation

## Run

- python workflow_dispatcher.py

## ToDo
- sample.csv overwrites itself if more than one job at a time is executed
- Add logger
- Instructions how to add pipeline
- Instructions ho to run pipeline in container?
- Add clean up
- Add env.yml
- Add test

## TBD
- Shall a new sample.csv sheet be created for every run? -> Can we just overwrite sample.csv?
- config.yaml run_date: "" has to be overwritten as well. Is it the exactly the same everywhere?
- Is it sufficient to have only one active container per workflow? (Serial instead of parallel processing)
- Base sm environment to start the container
- The containers use the unpacked DBs on ds/groups -> Whats the maximum size here?
- What happens if the same workflow starts for two different sequencer outputs? Will that happen? One Workflow container per sequencer?
- Can multiple users controll one cron job? Automation user that can be used from different people?
- Clean up -> move results to "output" folder and delete everything else?
