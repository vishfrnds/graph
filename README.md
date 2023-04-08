# Aim

## LLM
* graph based llm
* context is stored in nodes of graph and maintained forever
* weights are in edges of graph

## Copying capability
* build interfaces between existing models, to copy them.
* same model has non context based transformers to communicate with other models.

## Hierarchy of time prediction
* Remember immediate past
* Remember past in logarithmic decreasing order (same space is representing more information in time) as summary at different levels.
* Predict immediate future.
* Predict future in logarithmic decreasing order as summary at different levels.
