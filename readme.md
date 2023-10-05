HTML Tags

1. <input> Tags
<input type="checkbox" id="selectCheckBox" onchange="checkBox(this)">: This checkbox is used for selecting an option. When checked, it triggers the checkBox JavaScript function.
2. <select> and <input> Tags
<select id="selectList" name="selectList" onchange="checkSelection()">: A dropdown list used to select options. When the selection changes, it triggers the checkSelection JavaScript function.
<input type="text" id="selectListText" name="selectListText" placeholder="Other" style="display:none;">: A text input field that is displayed conditionally based on the selection in the dropdown list.
3. Form Fields and Error Messages
Various form fields, such as first name, last name, email, phone number, address, city, state, zipcode, and comments, are represented using <input> and <textarea> tags. Corresponding <span> tags with IDs (e.g., firstname_error, lastname_error) are used to display error messages.

4. Submit Button
<button type="submit" id="submitBtn" disabled>Submit</button>: The submit button that is initially disabled and enabled based on form validity.
5. Table for Displaying Data
<table id="myTable">: An HTML table element used to display form data.


JavaScript Functions

1. checkSelection()
Responsible for handling the selection of options in the dropdown list (selectList) and updating the visibility and requirements of form elements.
2. checkBox(x)
Handles the checkbox selection and the conditional display of the text input field (selectListText).
3. Validation Functions
Functions like validatefname(), validatelname(), validatemail(), validatephone(), validateAddress1(), validateCity(), validateState(), validateZipcode(), validateSelectbox(), and validatecomment() validate various form fields and display error messages accordingly.
4. submitButton()
Manages form submission by storing the form data in the sessionStorage object.
5. resetButton()
Clears any displayed error messages when the form is reset.
6. isMyFormValid()
Checks the overall validity of the form based on field-level validations. Enables/disables the submit button accordingly.
7. Event Listeners
An event listener is added to the form (myForm) to monitor changes in form fields. The submit button is enabled or disabled based on form validity.
8. showData()
Inserts form data into the HTML table for display.
9. validateForm()
Validates the form as a whole and manages the state of the submit button.