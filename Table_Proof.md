# Table Proof

Assume ringing means timer

| number | arms_down | alarm_on | northbound_present | southbound_present | north_approach | south_approach | north_depart | south_depart | ringing | safety_hazard |
|--------|-----------|----------|--------------------|--------------------|----------------|----------------|--------------|--------------|---------|---------------|
| 0      | 0         | 0        | 0                  | 0                  | 6              | 5              | 16           | 16           |  17     |               |
| 1      | 0         | 0        | 0                  | 1                  |                |                |              |              |         |  18           |
| 2      | 0         | 0        | 1                  | 0                  |                |                |              |              |         |  18           |
| 3      | 0         | 0        | 1                  | 1                  |                |                |              |              |         |  18           |
| 4      | 0         | 1        | 0                  | 0                  | 6              | 5              | 16           | 16           | 0       |               |
| 5      | 0         | 1        | 0                  | 1                  | 7              | 19             |  16          | 20           |  13     |               |
| 6      | 0         | 1        | 1                  | 0                  | 19             | 7              |  20          | 16           |  14     |               |
| 7      | 0         | 1        | 1                  | 1                  | 19             | 19             |  20          | 20           | 15      |               |
| 8      | 1         | 0        | 0                  | 0                  |                |                |              |              |         |  21           |
| 9      | 1         | 0        | 0                  | 1                  |                |                |              |              |         |  21           |
| 10     | 1         | 0        | 1                  | 0                  |                |                |              |              |         |  21           |
| 11     | 1         | 0        | 1                  | 1                  |                |                |              |              |         |  21           |
| 12     | 1         | 1        | 0                  | 0                  |                |                |              |              |         |  22           |
| 13     | 1         | 1        | 0                  | 1                  | 15             | 19             | 16           | 4            | 23      |               |
| 14     | 1         | 1        | 1                  | 0                  | 19             | 15             | 4            | 16           | 23      |               |
| 15     | 1         | 1        | 1                  | 1                  | 19             | 19             | 13           | 14           | 23      |               |

| number | invariant |
|--------|-----------|
| 16     |  Approach signal will always proceed a depart signal | 
| 17     |  Timer never will go off in idle state | 
| 18     |  While train is is prsent, barrers will never be raised |
| 19     | Never get two approach or depart signals in a row |
| 20     | Takes longer than 10 seconds for trian to get to crossing  |
| 21     | Alarm will never be off when arm is lowered  | 
| 22     | Arms will never be down when no trains are present |
| 23     | Timer will never go of when armdown?alarm_on state |

