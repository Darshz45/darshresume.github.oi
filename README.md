<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Create your resume and share it online.">
  <title>Online Resume Builder</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>Online Resume Builder</h1>
  <form id="resumeForm">
    <label for="name">Full Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>

    <label for="phone">Phone Number:</label>
    <input type="tel" id="phone" name="phone" required>

    <label for="jobTitle">Job Title:</label>
    <input type="text" id="jobTitle" name="jobTitle" required>

    <label for="skills">Skills (comma separated):</label>
    <input type="text" id="skills" name="skills" required>

    <label for="experience">Work Experience:</label>
    <textarea id="experience" name="experience" required></textarea>

    <label for="education">Education:</label>
    <textarea id="education" name="education" required></textarea>

    <button type="submit">Generate Resume</button>
  </form>

  <div id="resumePreview" style="display:none;">
    <h2>Generated Resume</h2>
    <div id="resumeContent"></div>
    <button id="downloadBtn">Download as PDF</button>
  </div>

  <script src="script.js"></script>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 20px;
  background-color: #f4f4f4;
}

h1 {
  text-align: center;
}

form {
  max-width: 600px;
  margin: 0 auto;
  background: #fff;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

label {
  display: block;
  margin-top: 10px;
}

input, textarea {
  width: 100%;
  padding: 10px;
  margin-top: 5px;
  border-radius: 4px;
  border: 1px solid #ccc;
}

button {
  background-color: #28a745;
  color: white;
  padding: 10px 20px;
  margin-top: 20px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

button:hover {
  background-color: #218838;
}

#resumeContent {
  background-color: white;
  padding: 20px;
  margin: 20px 0;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
