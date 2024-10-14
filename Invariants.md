# Invariants
- An approach signal will always procede a depart signal
- Power will never be interrupted 
- While train is at crossing, barrier will never be raised
- Alarm will never be off when it is lowered
- Assume sensers are never broken or delayed

# Varying Invariants

## Does There Exist a Sequence of Events, Such that an Invariant is No Longer True?

- Analyzing the example fsm, counter examples that prove the invariants false are:
  - State: idle --> nb_approach signal received --> state: ringing, arms up -> sb_approach signal received -> timer elapses -> state: ringing, ars down -> nb_depart signal recieved -> state: ringing, arms up
 -> timer elapses -> state: idle
  In the above sequence of events, the south bound train is still on the tracks, but the FSM has reached the "idle" state, violating the third invariant.
