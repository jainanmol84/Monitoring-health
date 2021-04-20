# Monitoring-health
Bayesian belief network classifier-based model

Algorithm 1 :
Input: N number of health attribute values, prefixed the
threshold value for each attribute.
Output: Current state of the patient.
Step 1: Determine attributes for the current context.
Step 2: Calculate Degree of Impact (DOI).
Step 2.1 : If ( DOI value in Abnormal Range)
Then Patient_State = Unsafe. Goto Step 4
Step 2.2: Else Paitent_State = Safe
Step 3: Return Paitent_State.
Step 4: Trigger the Event_Occurrence = True
Step 4.1: Generate early warning signal to responder.
Step 4.2: Send vital data to the Cloud storage
repository for analysis.
Step 5: Exit

Algorithm 2:
Input: Event set = Health ∪ Behavioural ∪ Environmental
Step 1: Using Algorithm 1, Determine the State of the
Patient.
Step 2: Determine current time stamp.
Step 3: If (Paitent_State = Unsafe and Any
Event_Occurrence =True), goto Step 4 else goto Step
8 // Any_Event Occurrence is a variable used for managing
an event. //
Step 4: Do
Step 4.1: Create a checkpoint. // Check-point is a
save point in time space. //
Step 4.2: Empty Log // Record of events //
Step 4.3: Start new session. // Granule formation for
events.//
Step 5: Add Event attributes to the Log for granulation
based temporal information generation.
Step 6: After t time , Determine Temporal Health Index
(THI) of the patient.
Step 7: If (THI (TGS(I), t) > α)
Step 7.1: Transfer log and health attribute
information to the responder for emergency
handling as shown in Fig. 5.
Step 7.2: Generate modified early warning signal to
family members.
Step 8: Repeat Step 1 after a definite time interval.
Step 9: Exit
