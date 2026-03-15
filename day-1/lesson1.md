#6: "The server is running and the database is connected."

server - S
database - DB

S ∧ DB

#7: "If the request is valid, then the API returns 200."

Valid Request - V

Return 200 - 200

V -> 200


#8: "The user is logged in or the page is public, but not both."

Logged User - U

Public Page - P

(U ∨ P) ∧ ¬(U ∧ P)



#9: "If the cache is empty and the database is down, the app crashes."

Empty Cache - E

DB Down - D

Crashed App - C

E ∧ D -> C


#10: "The test passes if and only if all assertions are true."


Passed Test  - T

All true assersion - A

T <=> A
