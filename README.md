# overview
## Task 1: Secure Data Exchange 

Introduction:
Secure data exchange is essential for protecting information over networks. Encoding formats like Base64, ASCII, and URL encoding help transmit data safely while working with protocols such as HTTPS, TLS, and SMTP.

Key Points:

Encodings: Base64, ASCII, URL, Hex.

Protocols: HTTPS, TLS, SMTP, REST APIs, OAuth.

Security: Encodings prevent injection attacks but do not encrypt; risks exist if misused.

Analysis: Compare strengths/weaknesses, show data flow diagrams, and use real examples (emails, API tokens).

## Task 2: Classroom Seating Arrangement – P vs NP 

Introduction:
Arranging students for exams while following social rules is a practical example of computational complexity. This task explores why some problems are easy to verify but hard to solve.

Key Points:

Rules: Friends & same-city students cannot sit together.

P vs NP: Checking a plan is easy; finding a correct plan is hard → NP problem.

Approaches:

Brute force: Try all arrangements; impractical for large classes.

Heuristic: Seat students with many friends first or separate same-city students; faster but may not be perfect.

## Task 3: College Club Management.

Introduction:
Managing student club data efficiently requires proper database design. Normalization reduces redundancy, prevents anomalies, and allows accurate querying.

Key Points:

Problems: Redundant/duplicate data, insert/update/delete anomalies.

Normalization:

1NF: Atomic fields, primary key.

2NF: Separate Student, Club, Membership.

3NF: Remove transitive dependencies.

ER Diagram: Entities, keys, and one-to-many relationships.

SQL: Insert/display data, JOIN queries for student-club info.

Reflection: Reduces repetition, improves accuracy; JOINs reconstruct relationships.

## conclusion:
In conclusion, these tasks highlight the importance of structure, efficiency, and security in different domains. Task 1 demonstrated how encoding formats integrated with web protocols enhance secure data exchange, while Task 2 illustrated computational complexity, showing the challenges of arranging students under constraints and the usefulness of heuristic approaches. Task 3 emphasized database normalization to reduce redundancy, prevent anomalies, and enable efficient queries. Together, they show that careful design and smart strategies improve both security and operational efficiency across systems.
