# simple-log-clustering
Takes a log file as input and outputs the groups and clusters of the log statements.

## Usage
To get a json file of the output, run main.py with these parameters:

```$ python main.py <input file> <output file> <threshold 1> <threshold 2> <separator>=' '```

Threshold 1: float value 0 < x < 1 that determines the percentage of tokens in a log statement that must be the same to initially cluster them.
Threshold 2: float value 0 < x < 1 that determines the percentage of tokens that must be similar in order to merge clusters together.
Separator: character used to tokenize the log statements

## Troubleshooting
At this point in time, there may be problems with the project configuration, so if the program breaks due to unknown import, attempt the following:

```$ pip install textdistance```
