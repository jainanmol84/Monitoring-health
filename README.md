# Monitoring-health
Bayesian belief network classifier-based model

1. **Algorithm 1** :
  1. Inout - N number of health attribute values, prefixed the threshold value for each attribute.
  2. Output: Current state of the patient.
  3. This Output will trigger the algorithm 2

2. **Algorithm 2**:
  1.  Input: Event set = Health ∪ Behavioural ∪ Environmental
  2.  Using Algorithm 1, Determine the State of the Patient.
  3.  Generate modified early warning signal to family members.

