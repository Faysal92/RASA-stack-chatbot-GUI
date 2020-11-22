## Story 1
* greet
    - utter_greet
* position
    - utter_role
* position{"role_type": "technical"}
    - slot{"role_type": "technical"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_knowmore
* affirm
    - utter_utilities
* position
    - utter_role
* position{"role_type": "business"}
    - slot{"role_type": "business"}
    - action_check_positions
    - slot{"positions": []}
    - utter_knowmore
* deny{"deny": "nope"}
    - utter_nothanks
    - utter_goodbye

## Story 2
* greet
    - utter_greet
* position
    - utter_role
* position{"role_type": "business"}
    - slot{"role_type": "business"}
    - action_check_positions
    - slot{"positions": []}
    - utter_knowmore
* deny
    - utter_nothanks
    - utter_goodbye

## Story 3
* greet
    - utter_greet
* position
    - utter_role
* position{"role_type": "any"}
    - slot{"role_type": "any"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_knowmore

## Story 4
* greet
    - utter_greet
* position
    - utter_role
* position{"role_type": "technical"}
    - slot{"role_type": "technical"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_knowmore
* affirm
    - utter_utilities
* position
    - utter_role
* position{"role_type": "technical"}
    - slot{"role_type": "technical"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_knowmore
* affirm{"affirm": "ya"}
    - utter_utilities
* position
    - utter_role
* position{"role_type": "business"}
    - slot{"role_type": "business"}
    - action_check_positions
    - slot{"positions": []}
    - utter_knowmore
* affirm
    - utter_utilities
* position
    - utter_role
* position{"role_type": "any"}
    - slot{"role_type": "any"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_knowmore
* deny
    - utter_nothanks
    - utter_goodbye

## Story 5
* greet+position
    - utter_simple_greet
    - utter_role
* position{"role_type": "technical"}
    - slot{"role_type": "technical"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_knowmore
* affirm
    - utter_utilities
* position
    - utter_role
* position{"role_type": "business"}
    - slot{"role_type": "business"}
    - action_check_positions
    - slot{"positions": []}
    - utter_knowmore
* deny
    - utter_nothanks
    - utter_goodbye

## Generated Story 6
* greet+name+status{"PERSON": "Ali Park"}
    - slot{"PERSON": "Ali Park"}
    - utter_check
    - action_check_status
    - slot{"status": "rejected"}
    - utter_knowmore
* affirm
    - utter_utilities

## Generated Story 7
* greet+name+status{"PERSON": "jibin"}
    - slot{"PERSON": "jibin"}
    - utter_check
    - action_check_status
    - slot{"status": "unknown"}
    - utter_knowmore
* deny
    - utter_nothanks
    - utter_goodbye

## Story 8
* greet+name+status{"PERSON": "Ali Park"}
    - slot{"PERSON": "Ali Park"}
    - utter_check
    - action_check_status
    - slot{"status": "interview"}
    - utter_knowmore
* affirm{"affirm": "y"}
    - utter_utilities
* position
    - utter_role
* position{"role_type": "technical"}
    - slot{"role_type": "technical"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_knowmore
* affirm
    - utter_utilities

## Story 9
* status
    - utter_name
* name{"PERSON": "Jibin"}
    - slot{"PERSON": "Jibin"}
    - utter_check
    - action_check_status
    - slot{"status": "received"}
    - utter_knowmore
* deny{"deny": "n"}
    - utter_nothanks
    - utter_goodbye

## Story 10
* greet
    - utter_greet
* status
    - utter_name
* name{"PERSON": "Jibin"}
    - slot{"PERSON": "Jibin"}
    - utter_check
    - action_check_status
    - slot{"status": "unknown"}
    - utter_knowmore
* affirm
    - utter_utilities
* position
    - utter_role
* position{"role_type": "any"}
    - slot{"role_type": "any"}
    - action_check_positions
    - slot{"positions": ["machine learning engineer", "ML product success engineer"]}
    - utter_knowmore
* deny
    - utter_nothanks
    - utter_goodbye

## Story 11
* thanks
    - utter_nothanks

## Story 12
* status
    - utter_name
* name{"PERSON": "jibin mathew"}
    - slot{"PERSON": "jibin mathew"}
    - utter_check
    - action_check_status
    - slot{"status": "rejected"}
    - utter_knowmore
* deny
    - utter_nothanks
    - utter_goodbye

