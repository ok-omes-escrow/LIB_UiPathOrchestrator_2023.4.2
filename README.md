# LIB_UiPathOrchestrator_2023.4.2

## Description
The Holiday Calendar UiPath Library Project provides calendar related functionalities.  
Some important details to consider before to use it are:

  - UiPath Orchestrator Version: 2023.4.2
  - Uipath Studio Version : 2023.4.5 
 

## Features
- [Activity-1](#activity-1-get-previous-working-day)
- [Activity-2](#activity-2-get-next-working-day)



## Activity 1: Get Previous Working Day  
 
### Details:
  - Business requirement is to get current working day and its previous working day from Calendar. The current date must be a working day, it should not be weekend or non-working day.  Also check its previous date, if it is weekend or non-working day then Consider its previous date. 
Note: Calendar functionality in UiPath Orchestrator allows Bot controller to define non-working days. Non-working days can be festivals or public holidays. This functionality offers Bot Controller to Schedule/Trigger UiPath Bots only on working days. 

    | Command | Description |
    | --- | --- |
    | Input | in_strInputDate : string; in_strCalendarName : string; in_intMaxLoopCounter : int; in_excMsgMaxLoopCounter : string; in_excMsgInvalidCalendarName : string |
    | Output | out_strCurrentWorkingDay : string ; out_strPreviousWorkingDay : string |
    | Input/Output | |
    | Requirements | NA |
    | App Version | NA |



  - Additional Details:
  - Examples: input: 2023-12-12 ( 12th December is already declared as non-working day in calendar)    
    Output: Current date: 2023-12-11  &  Previous date: 2023-12-08

    Screenshot :
    ![image](https://github.com/ok-omes-escrow/LIB_UiPathOrchestrator_2023.4.2/assets/146367950/de7937c6-75c2-4f8c-bb74-481ede777b98)

 

- [Back to menu](#features)


## Activity 2: Get Next Working Day  

### Details:
  - Business requirement is to get next working day from Calendar based on Input day. Input day must be dynamic.
Note: Calendar functionality in UiPath Orchestrator allows Bot controller to define non-working days. Non-working days can be festivals or public holidays. This functionality offers Bot Controller to Schedule/Trigger UiPath Bots only on working days. 

    | Command | Description |
    | --- | --- |
    | Input | in_strInputDate : string; in_strRequiredInputDay : string;  in_strCalendarName : string; in_excMsgInvalidCalendarName : string; in_intMaxLoopCounter : int; in_excMsgMaxLoopCounter : string; in_excMsgCalenDaysNotFound : string; |
    | Output | out_strOutDate : string ; |
    | Input/Output | |
    | Requirements | NA |
    | App Version | NA |



  - Additional Details:
  - Examples: in_strInputDate : 2024-01-15 ( 24th  is already declared as non-working day in calendar)
    in_strRequiredInputDay : Wednesday 
    Output: 2024-01-17

  - Examples: input: 2024-01-17 ( 24th  is already declared as non-working day in calendar)
    in_strRequiredInputDay : Wednesday   
    Output: 2024-01-31 

    Screenshot :
![image](https://github.com/ok-omes-escrow/LIB_UiPathOrchestrator_2023.4.2/assets/146367950/edbb5784-d301-43a9-9201-11f5a270a1bd)






 

- [Back to menu](#features)
