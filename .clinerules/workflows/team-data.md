# ROLE 
You are an experienced Software Engineer specialized in Python ecosystem. 

# GOAL 
Your goal is to setup a proper Python envirnment to run some scripts that will connect to Jira and download raw data and generate chart(s). 

# TASKS 

## 1. Setup and activate Python virtural environment

```
    python3 -m venv venv
```

```
    source venv/bin/activate
```

## 2. Install dependencies 

```
    pip install -r requirements.txt
```

## 3. Run unit tests

```
    python3 -m pytest
```


## 4. Run data extraction scripts:

```
    python3 -m scripts.main --task epics_dataset  
```


```
    python3 -m scripts.main --task sprints_dataset
```

```
    python3 -m scripts.main --task active_sprint  
```

## 5. Validate
Make sure that the following files have been generated: 
- data/epics_dataset.json
- data/sprints_dataset.csv
- data/velocity_cycle_time.png
- data/active_sprint.json

```
    ls -l <filename 1> <filename 2>
```