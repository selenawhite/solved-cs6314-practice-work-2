Download Link: https://assignmentchef.com/product/solved-cs6314-practice-work-2
<br>
Form validation is a way for you to tell the user what kind of input is required in each field and allows you to notify the user when the input is incorrect. There are many ways to do form validation, but in this assignment you will write a plugin (in Javascript) that displays information/error messages besides the input fields.

<strong><em>Requirements</em></strong>

The code files for form validation are validate.html, validate.css and validate.js. <u>You will only modify </u><u>validate.js</u><u>.</u>

The validation rules are as follows:

<ul>

 <li>The username field must contain only alphanumeric characters.</li>

 <li>The password field should be at least six characters long.</li>

 <li>The email field should be a valid email address (<a href="/cdn-cgi/l/email-protection#d9b8bbba99bdbcbff7a1a0a3"><span class="__cf_email__" data-cfemail="1677747556727370386e6f6c">[email protected]</span></a>). A valid email consists of an email prefix and an email domain. The prefix appears to the left of the @ symbol and domain appears to the right of the @ symbol.</li>

</ul>

When the page is fully loaded, you should insert a &lt;span&gt; notification element immediately after each form field. The notification elements should initially be hidden.

When the field is currently being edited, the notification element’s text should be infoMessage (i.e. password should include at least six characters), its class should be “info”, and it should be visible.

When the field is not being edited:

<ul>

 <li>If the field is empty, the notification element should be hidden.</li>

 <li>If the field is non-empty and the form field validates, the notification element’s text should be “OK”, its class should be “ok”, and it should be visible.</li>

 <li>If the field is non-empty and the form field does not validate, the notification element’s text should be “Error”, its class should be “error”, and it should be visible.</li>

</ul>

<strong><em>Solution Hint</em></strong>

You should use the <a href="https://developer.mozilla.org/en-US/docs/Web/Events">form events</a> functions to detect when a form field gains or loses focus. You should not use mouse and keyboard events such as click or keydown: there are multiple ways to give a form field focus, and it is difficult to detect all of them reliably using mouse and keyboard events. Span elements can be added using element creation and <a href="https://developer.mozilla.org/en-US/docs/Web/API/Node/appendChild">DOM insertion</a>.

For validating username and email, you will need to write <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">regular expressions</a>.