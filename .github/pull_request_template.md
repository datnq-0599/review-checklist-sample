## Related Tickets
- [#Ticket ID](https://dev.framgia.com/redmine/issues/???)

## WHAT
- Change number items `completed/total` in admin page.

## HOW
- I edit js file, inject not_vary_normal items in calculate function.

## WHY
- Because in previous version - number just depends on `normal` items. But in new version, we have `state` and `confirm_state` depends on both `normal` + `not_normal` items.

## Evidence (Screenshot or Video)

## Performance (Optional)
- [ ] Resolved n + 1 query

- [ ] Time run rake task : 1000 ms

- Generated SQL query

## Review Checklist

Category | View Point | Description | Expected Reviewer Answer | Reviewer1 (name) | Reviewer2 (name)
--- | --- | --- | --- | --- | ---
General | [MUST] Is the code related to only the specific issue assigned to you? | The purpose of the written code should be understood from the related issue** or the code itself. If no code belonging to the requested business rule has been written, it must be corrected. | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
General | [SHOULD] Is all the code easily understood, readable? | if the source code is difficult to understand it could be hard for maintainability | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
General | [MUST] Do the names used in the program convey intent? | variable name, method name is proper or not | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
General | [MUST] Does it follow a coding rule applied to the project | Does it conform to your agreed coding conventions? These will usually cover location of braces, variable and function names, line length, indentations, formatting, and comments. | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
General | [MUST] Does the code follow DRY?: Do not Repeat Yourself | Is there any redundant or duplicate code? DRY (Do not Repeat Yourself) principle: The same code should not be repeated more than twice. Consider reusable services, functions and components. Consider generic functions and classes. | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
General | [MUST] Do loops have a set length and correct termination conditions? | The code should be to avoid infinity loop or deadlock | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
General | [MUST] Is there any hard-coded in the code |  | NO |<li>- [ ] no</li>|<li>- [ ] no</li>
General | [MUST] is there any refactoring code that change the input or output of method and all callers of it are changed properly |  | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
General | [MUST] is there any new exception that are inserted in code, make sure it will be caught in callers  | make sure the new exception is caught and handle properly | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
Performance | [SHOULD] Are there any obvious optimizations that will improve performance? | ex make sure  N+1 query is reduced as much as possible | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
Performance | [SHOULD] Can any of the code be replaced with library or built-in functions? | Verify that existing libraries/classes are used instead of writing code from scratch | NO |<li>- [ ] no</li>|<li>- [ ] no</li>
Performance | [SHOULD] is there any debugging code | the debugging and logging code can make the performance down | NO |<li>- [ ] no</li>|<li>- [ ] no</li>
Security | [MUST] Are all data inputs validated (for the correct type, length, format, and range) | ensure that the data that require validation must be checked | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
Security | [MUST] Does the sensitive information store in the code | ensure that GCP/AWS secret key, private key don't store in code | NO |<li>- [ ] no</li>|<li>- [ ] no</li>
Security | [SHOULD] Where third-party utilities are used, are returning errors being caught? | make sure don't use black box code | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
Security | [MUST] is the password encrypted when store in database |  | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
Security | [SHOULD] Are invalid parameter values handled? |  | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
Testing | [SHOULD] Is the code testable?  | The code should be structured so that it doesn't add too many or hide dependencies, is unable to initialize objects, test frameworks can use methods etc. | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
Testing | [MUST] Do tests exist, and are they comprehensive? |  | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
Testing | [MUST] Do unit tests actually test that the code is performing the intended functionality? |  | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>
Documentation | [MUST] Is there any incomplete code? If so, should it be removed or flagged with a suitable marker like ‘TODO’? |  | YES |<li>- [ ] yes</li>|<li>- [ ] yes</li>


## Notes (Optional)
*(Impacted Areas in Application(List features, api, models or services that this PR will affect))*

*(List gem, library third party add new)*

*(Other notes)*
