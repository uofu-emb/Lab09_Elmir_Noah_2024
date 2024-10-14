# Elmir's FSM
- Counter_Examples:
  - In Elmir's, from idle, if northbound_approach signal is recieved, we enter the second state, from the second state, there is no logic to check for southbound_approach, so we can recive that signal during state 2. In state 3 we can recieve either northbound_depart or southbound_depart, and after 10 seconds, the other train might still be on the tracks, which is not safe.

# Noah's FSM
- Counter_Examples:
  - Assuming two tracks, if two trains coming northbound, and southboud at the same time come, the state will be stuck in ide since the transition will not be able to choose to go into northbound state or southbound state unless stated othereise
