# verbose-octo-doodle

## intent
consider it as the aim or target of the user input. If a user say "i want to order a book" here intent would be ORDER BOOK  
    - good morning, hi hello there : GREET  
    - no never i don't think so no way : DENY  
    - sad, unhappy, terible, not very good : SAD / UNHAPPY  

## Entity
all nouns in dialog same to entity  
Reserve a table at Taj Hotel tomorrow night  
    - intent BOOK THE TABLE  
    - entity  
        place: Taj hotel 
        time: tomorrow night   
my saving account is 24892  
    - intent: ACCOUNT DETAILS    
    - entity  
        acc_type: saving  
        number: 24892  

## Actions
it's an opperation which can be performed by the bot 

## Stories
these are a sample interaction between the user and bot, defined in terms of intents captured

## Domain
simply it's the response by bot  

`nlu.md` - Intent and Entity  
`stories.md` - Story(Dialog management)  
`domains.yml` - actual output (hard code)[all intent, entity, action, response]  
`action.py` - custom reply  

## Rasa NLU
A library of NLU which takes the user input and try to extract the available entityes and intents and try to help to bot what user is trying to say

## Rasa Core jobs
- Dialog Engine  
- Stories  
- Domain  
- Response  
- Action  
- Slots  
- Forms  
- Knowledge Base Actions  

## RASA Architecture
steps  
1. Interpriter - this part handel by NLU
2. Tracker - this objects track of conversation state
3. Policy - receives the current state of the tracker (policy chooses which action to take next)
4. Action - action is logged by the tracker



