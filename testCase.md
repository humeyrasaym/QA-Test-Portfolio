
## Login Test Case\
\
| Test Case ID | Scenario | Steps | Expected Result |\
|---|---|---|---|\
| TC-001 | Empty email field | 1. Go to login page<br>2. Leave email empty<br>3. Enter password<br>4. Click login | User should see an email required error |\
| TC-002 | Wrong password | 1. Go to login page<br>2. Enter valid email<br>3. Enter wrong password<br>4. Click login | User should see an invalid password error |\
| TC-003 | Valid login | 1. Go to login page<br>2. Enter valid email<br>3. Enter valid password<br>4. Click login | User should successfully log in |\
}
