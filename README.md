# Ex03 To-Do List using JavaScript
## Date: 12-5-26

## AIM
To create a To-do Application with all features using JavaScript.

## ALGORITHM
### STEP 1
Build the HTML structure (index.html).

### STEP 2
Style the App (style.css).

### STEP 3
Plan the features the To-Do App should have.

### STEP 4
Create a To-do application using Javascript.

### STEP 5
Add functionalities.

### STEP 6
Test the App.

### STEP 7
Open the HTML file in a browser to check layout and functionality.

### STEP 8
Fix styling issues and refine content placement.

### STEP 9
Deploy the website.

### STEP 10
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        #textbox{
            position:absolute;
            right:150px;
        }
        #add{
            position:absolute;
            right: 20px;
        }
        li{
            list-style: none;
            background-color: cyan;
            font-size: 20px;
            margin: 10px;
            border-radius: 20px;
            padding-left: 15px;
        }
        i{
            position: absolute;
            right: 30px;
        }
        .st{
            text-decoration: line-through;
        }
    </style>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
    
    <script>
      function addTask() {
    const input = document.getElementById('textbox');
    const container = document.getElementById('container');
    
    if (input.value.trim() !== "") {
        const li = document.createElement('li');
        li.innerHTML = `
            <span onclick="this.classList.toggle('st')">${input.value}</span>
            <i class="bi bi-trash" onclick="this.parentElement.remove()"></i>`;
        container.appendChild(li);
        input.value = "";
    }
}
    </script>
</head>
<body>
    <div class="card mx-auto my-3" style="width: 30rem;">
      <div class="card-header bg-danger text-white text-center" >TODO</div>
      <div class="card-body">
        ADD TASK
        <input type="text" id="textbox" class="rounded-5">
        <div class="btn btn-primary btn-sm" id="add" onclick="addTask()">ADD</div>
        <ul id="container">
            
        </ul>
      </div>
    </div>
</body>
</html>
```

## OUTPUT
<img width="1911" height="1027" alt="image" src="https://github.com/user-attachments/assets/11cfefca-f245-4129-ae67-d1d6c8487455" />


## RESULT
The program for creating To-do list using JavaScript is executed successfully.
