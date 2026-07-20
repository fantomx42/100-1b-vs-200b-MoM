# Mixture of Models (MoM) Prototype

This repository contains a small, runnable prototype of the **Sociological Architecture for a Mixture of Models**.

## What it does

- Models a bounded society of agents with roles
- Runs a town-hall style deliberation process
- Lets some agents answer even when they think they should stay silent
- Forms opposing clusters for adversarial debate
- Reintroduces suppressed but high-confidence dissent when the majority looks overconfident
- Keeps an externalized institutional record of the process

## Files

- `mom.py` — core simulation engine and CLI
- `README.md` — usage notes

## Run

This project uses only the Python standard library.

```bash
python mom.py "Should we use majority consensus for model routing?"
```

## Design map

The code mirrors your architecture:

- **Society** → bounded set of agents
- **Role occupants** → expert, critic, coordinator, integrator, recorder, observer
- **Interaction order** → regulated turn-taking and staged debate
- **Institutional memory** → decision log and rationale archive
- **Constitutional governance** → configurable thresholds and rules
- **Reputation** → role-specific trust weights
- **Collective deliberation** → staged synthesis with dissent preservation
- **Town hall** → structured deliberation with adversarial challenge
- **Dunbar constraint** → active participant cap

## Notes

This is a scaffold, not a final training or inference system. It is designed to be the first working version that you can extend later with actual model backends.
