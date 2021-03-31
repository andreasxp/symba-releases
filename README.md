# Symba
A market simulator utilizing a multi-agent reinforcement learning system.

## Installation
Symba is a closed-source application - no source code is available. You can download a pre-built binary for your system from the [releases page](https://github.com/andreasxp/symba-releases/releases). The latest version is `1.0.0`.

Consider trying out [Symba Designer](https://github.com/andreasxp/symba-gui) - a GUI companion application for Symba.

## Usage
Symba is a command-line application - you can run it from your terminal of choice. It has a command-line interface that you can use to customize your simulation:
```
$ ./symba-x64-linux --help
A market simulator built in C++.
Usage: symba [OPTIONS]

Options:
  -h,--help                   Print this help message and exit
  -o,--output-dir TEXT:DIR REQUIRED
                              Output directory for simulation results
  -I,--n-agents INT:INT in [10 - 10000]=500
                              Number of agents in the simulation
  -J,--n-stocks INT:INT in [1 - 100]=1
                              Number of stocks in the simulation
  -T,--n-steps INT:INT in [281 - 10000]=3875
                              Number of simulation time steps
  -S,--n-rounds INT:INT in [1 - 10000]=1
                              Number of simulations
  --rate FLOAT:FLOAT in [0 - 2]=0.01
                              Risk-free rate
  --plot BOOLEAN=0            Output plots
  --type-neb TEXT:{Classic,Algorithmic,Human,LossAversion,Positivity,Negativity,DelayDiscounting,Fear,Greed,LearningRate}=Classic
                              Agents' cognitive traits
  --hp-gesture FLOAT:FLOAT in [1 - 10]=1
                              Transaction gesture scalar
  --liquidation-floor INT:INT in [0 - 100]=50
                              YTD drawdown
  --leader-type TEXT:{Worst,Best,Static,Noise,NoCluster}=NoCluster
                              Type of agent leader other agents emulate
  --cluster-limit INT:INT in [0 - 100]=1
                              Percentage of agents imitating agent leader
  -v                          Level of output verbosity
```
