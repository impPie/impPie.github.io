---
title: "Password Protected Post"
date: 2025-09-04
categories: notes
protected: true
---

<div id="password-prompt" style="text-align: center; margin: 50px 0;">
    <h3>This post is password protected</h3>
    <input type="password" id="password-input" placeholder="Enter password">
    <button onclick="checkPassword()">Submit</button>
</div>

<div id="protected-content" style="display: none;">
    <h2>Protected Content</h2>
    <p>This content is only visible after entering the correct password.</p>
    
    <!-- Your actual content goes here -->
</div>

<script>
function checkPassword() {
    const password = document.getElementById('password-input').value;
    const correctPassword = 'yourpassword123'; // Change this!
    
    if (password === correctPassword) {
        document.getElementById('password-prompt').style.display = 'none';
        document.getElementById('protected-content').style.display = 'block';
    } else {
        alert('Incorrect password');
    }
}
</script>
