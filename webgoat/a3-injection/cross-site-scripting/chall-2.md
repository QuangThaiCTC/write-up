# Challenge name: Try It! Reflected XSS

### Challenge Description
The assignment’s goal is to identify which field is susceptible to XSS.

It is always a good practice to validate all input on the server side. XSS can occur when unvalidated user input gets used in an HTTP response. In a reflected XSS attack, an attacker can craft a URL with the attack script and post it to another website, email it, or otherwise get a victim to click on it.

An easy way to find out if a field is vulnerable to an XSS attack is to use the `alert()` or `console.log()` methods. Use one of them to find out which field is vulnerable.

### My solution
- If you click `Purchase`, your credit card number will printing below.
![img](chall-attached/img-1.png)
- This is location where we XSS attack.
- Insert this payload to input of credit card number
`<script>alert('XSS Attack')</script>`