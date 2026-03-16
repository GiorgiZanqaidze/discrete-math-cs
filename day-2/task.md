
## Exercises — Set A (Direct Translation)

Define your variables and write the formula.

| # | English Statement | Variables | My Formula | Correct? |
|---|-------------------|-----------|------------|----------|
| 1 | "The API returns an error unless the token is valid." | | | |
| 2 | "You can deploy only if all tests pass." | | | |
| 3 | "The page loads if and only if the CDN is reachable and the server is up." | | | |
| 4 | "The notification is sent if the user is online or if the priority is high." | | | |
| 5 | "The build fails unless the config exists and the dependencies are installed." | | | |

1. 
The API returns an error unless the token is valid

if not Valid -> error

¬V -> E


2. 
"You can deploy only if all tests pass."

Deploy -> All tests


3.
"The page loads if and only if the CDN is reachable and the server is up."


Load 

CDN_REACH

ServerUp

Load -> (CDN_REACH ∧ ServerUp) 

4. 
"The notification is sent if the user is online or if the priority is high."

SEND_NOTI

ONLINE_USER

HIGH_PRIOR


(ONLINE_USER ∨ HIGH_PRIOR ) -> SEND_NOTI

5.

"The build fails unless the config exists and the dependencies are installed."

FAILS

CONF_EXIST

DEP_INSTALLED

¬(CONF_EXIST ∨ DEP_INSTALLED) -> FAILS





## Exercises — Set B (Bug Hunting)

Each formula has a mistake. Find it and fix it.

### #6
**English:** "Access is granted if the user is an admin or the request is internal."  
**Given formula:** a ∧ r → g  
**What's wrong?**  
My answer:  


**My corrected formula:**  


### #7
**English:** "The email is sent only if the user has opted in and the address is verified."  
**Given formula:** (o ∧ v) → e  
**What's wrong?**  
My answer:  


**My corrected formula:**  


### #8
**English:** "The cache is cleared unless it was updated in the last hour."  
**Given formula:** u → ¬c  
**What's wrong?**  
My answer:  


**My corrected formula:**  

