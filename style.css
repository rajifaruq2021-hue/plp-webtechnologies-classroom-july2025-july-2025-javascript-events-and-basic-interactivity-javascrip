// Wait for the entire HTML page to load before running the script
document.addEventListener('DOMContentLoaded', () => {

    // --- PART 1 & 2: Interactive Features ---

    // --- Feature 1: Light/Dark Mode Toggle ---
    const themeToggleButton = document.getElementById('theme-toggle');
    const body = document.body;

    // Listen for a click on the toggle button
    themeToggleButton.addEventListener('click', () => {
        // The 'toggle' method adds the class if it's not there, and removes it if it is.
        body.classList.toggle('dark-mode');
    });


    // --- Feature 2: Character Counter ---
    const messageInput = document.getElementById('message-input');
    const charCounter = document.getElementById('char-counter');

    // Listen for any input (typing, pasting, etc.) in the textarea
    messageInput.addEventListener('input', () => {
        const currentLength = messageInput.value.length;
        charCounter.textContent = currentLength;
    });


    // --- PART 3: Custom Form Validation ---
    const form = document.getElementById('contact-form');
    const nameInput = document.getElementById('name');
    const emailInput = document.getElementById('email');
    const passwordInput = document.getElementById('password');

    const nameError = document.getElementById('name-error');
    const emailError = document.getElementById('email-error');
    const passwordError = document.getElementById('password-error');

    // Listen for the form's 'submit' event
    form.addEventListener('submit', (event) => {
        // This is crucial: it stops the form from reloading the page
        event.preventDefault(); 
        
        let isValid = true; // Assume the form is valid initially

        // --- Validation Logic ---

        // 1. Name Validation (must not be empty)
        if (nameInput.value.trim() === '') {
            nameError.textContent = 'Name is required.';
            isValid = false;
        } else {
            nameError.textContent = '';
        }

        // 2. Email Validation (must contain '@')
        if (!emailInput.value.includes('@')) {
            emailError.textContent = 'Please enter a valid email address.';
            isValid = false;
        } else {
            emailError.textContent = '';
        }

        // 3. Password Validation (must be at least 8 characters)
        if (passwordInput.value.length < 8) {
            passwordError.textContent = 'Password must be at least 8 characters long.';
            isValid = false;
        } else {
            passwordError.textContent = '';
        }


        // --- Final Submission Check ---
        if (isValid) {
            alert('Form submitted successfully!');
            form.reset(); // Clear the form fields
        }
    });

});
