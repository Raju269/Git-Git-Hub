# Centralized VCS vs. Distributed VCS

## Centralized Version Control Systems (CVCS)

Repository Location: Features a single, central server where all versioned files and the entire history are stored. Clients check out files from this single source.

Network Dependency: Requires a constant network connection to perform most operations (like committing, updating, and viewing history). Working offline is severely limited or impossible.

Backup: Prone to a single point of failure. If the central server crashes and no external backups exist, all project history can be lost.

Branching: Branching and merging are generally more complex, slower, and often managed on the server, making frequent branching cumbersome for individual developers.

## Distributed Version Control Systems (DVCS) (e.g., Git)

Repository Location: Every developer maintains a full mirror of the entire repository on their local machine, including the project's complete history.
Network Dependency: Developers can work offline for long periods, committing changes locally. The network is only required for syncing (pushing or pulling) changes with remote repositories.
Backup: Provides inherent backup. If the central server fails, any developer's local repository can be used to restore the entire project history.
Branching: Branching is fast, cheap, and primarily managed locally. This encourages developers to create frequent, lightweight branches for features and experiments without impacting the remote repository until ready.
