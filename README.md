# Vacuum Search

This project uses various search algorithms to intelligently search the environment for dirty rooms to clean.

The agent can be launched from command line as following:
>python vacuum_search.py -s searchType -c costFunction -r heuristic -n (corners)

USAGE:      
>python vacuum_search.py <options>  
EXAMPLES:
>python vacuum_search.py
>- starts an interactive game
>
>(2) python vacuum_search.py -s A*
>- perform A* search to clean all rooms
>
>(3)  python vacuum_search.py -s Greedy -r Manhattan
>- perform greedy algorithm search with Manhattan cost function
>
>(4) python vacuum_search.py -s UCS -c StayTop
>- perform uniform cost search while preferentially searching the top

The detailed description of each option is described in function readCommand() in script vacuum_search.py. 
searchType and costFunction options can be set using the GUI, but the last 2 options in this command can only be set using commandline launch or using the run configuration provided with the project.
