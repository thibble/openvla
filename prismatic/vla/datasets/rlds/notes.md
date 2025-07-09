notes for antonio:
- after restructure i don't havea state obs, just action. here are the keys of transformed ds:
el['observation'].keys()
dict_keys(['image_primary', 'timestep'])
el.keys()
dict_keys(['observation', 'task', 'action', 'dataset_name', 'absolute_action_mask'])

So depending on your transform function you might have been taking EEF (not deltas) or joint positions as rel_actions_world

next question: how are those used for supervision? 