# workflow_automation

## Run

- python workflow_dispatcher.py

## ToDo
- Add logger
- Add workflow description
- Instructions how to add pipeline
- Instructions ho to run pipeline in container?
- Add env.yml
- Add test

## TBD
- Shall a new sample.csv sheet be created for every run? -> Can we just overwrite sample.csv? -> Yes
- config.yaml run_date: "" has to be overwritten as well. Is it the exactly the same everywhere? -> Shall be overwritten every time
- Is it sufficient to have only one active container per workflow? (Serial instead of parallel processing) -> Yes
- Base sm environment to start the container -> See shared user
- The containers use the unpacked DBs on ds/groups -> Whats the maximum size here? -> 140 GB
- What happens if the same workflow starts for two different sequencer outputs? Will that happen? One Workflow container per sequencer? -> One container is sufficient
- Can multiple users controll one cron job? Automation user that can be used from different people? -> Ask Marcel
- Clean up -> move results to "output" folder and delete everything else? -> Not needed
