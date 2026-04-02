# Welcome to My Portfolio

## Bio
Hello! I'm a Senior Full Stack Developer with over 4 years of experience in building robust and scalable web applications. I specialize in both front-end and back-end development, focusing on creating seamless user experiences and optimizing performance. My passion for coding drives me to continuously learn and adopt new technologies in this ever-evolving field.

## Tech Stack
- **Front-end:** HTML, CSS, JavaScript, React, Angular
- **Back-end:** Node.js, Express, Python, Django
- **Databases:** MongoDB, PostgreSQL, MySQL
- **Tools & Technologies:** Git, Docker, Jenkins, AWS

## Interactive JavaScript Code
Here is a snippet of code that dynamically displays my developer details:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Developer Details</title>
</head>
<body>
    <h1>Developer Details</h1>
    <div id="developer-info"></div>

    <script>
        const developer = {
            name: "Your Name",
            experience: "4+ years",
            techStack: ["JavaScript", "React", "Node.js", "MongoDB"]
        };

        const infoDiv = document.getElementById('developer-info');
        infoDiv.innerHTML = `<p>Name: ${developer.name}</p>\n                             <p>Experience: ${developer.experience}</p>\n                             <p>Tech Stack: ${developer.techStack.join(', ')}</p>`;
    </script>
</body>
</html>
```
