# Covid-19 Mobility-Controller

Our project discusses about a design that can smartly control overcrowding of people in popular places without prohibiting people’s mobility. Our primary responsibilities is to try “flattening the curve”.

The main project has been divided into four components - Spatial Mobility Model (SMM), Epidemiological Model (EMM), the Agent Based Modeling (ABM), the Mobility Controller (ours).

- Mobility Model - Read in mobility data and generate spatial model of NYC and simulate trips that people might take.
- Agent Based Model Simulation - Receive sample trips from mobility model and maintain state of citizens taking trips (sick, healthy, etc.) which will come from epidemiological model.
- Epidemiological Model - Models agents and movements with regards to health/sickness under variety of simulations to explore strategies of "flattening the curve".
- Mobility Controller - Receives booking requests from agent-based model simulation and ultimately decides whether or not a trip is safe to make. Confirmation/rejection is passed to agent-based model simulation. Also an alternative time will be given if that block reached maximum capacity. Also our policy should be fair to all agents - no agent should be allowed to cheat and receive consecutive booking confirmations.
