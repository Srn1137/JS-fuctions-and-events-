# JS-fuctions-and-events-
JS functions used in validations of html forms
<!DOCTYPE html>
<html>
    <head>
        <title>String Demo</title>
        <link rel="stylesheet" href="../node_modules/bootstrap/dist/css/bootstrap.css">
        <script>
            function ChangeTheme(){
                var themeCheckBox = document.getElementById("theme");
                var formContainer = document.getElementById("formContainer");
                if(themeCheckBox.checked) {
                    formContainer.className = "dark-theme";
                    document.querySelector("button").className="btn btn-dark w-100";
                } else {
                    formContainer.className = "light-theme";
                    document.querySelector("button").className="btn btn-primary w-100";
                }
            }
        </script>
        <style>
            .form {
                border: 2px solid black;
                padding: 20px;
                width: 250px;
                margin-top: 20px;
            }  
            .dark-theme {
                border: 2px solid black;
                padding: 20px;
                width: 250px;
                margin-top: 20px;
                background-color: black;
                color:white;
            }
            .light-theme {
                border: 2px solid black;
                padding: 20px;
                width: 250px;
                margin-top: 20px;
                background-color: white;
                color:black;
            }
        </style>
    </head>
    <body class="container-fluid">
        <div class="form" id="formContainer">
            <div class="form-switch">
                <input type="checkbox" id="theme" onchange="ChangeTheme()" class="form-check-input"> Dark Theme
            </div>
            <h2>Register User</h2>
            <dl>
                <dt>User Name</dt>
                <dd><input type="text"></dd>
                <dt>Password</dt>
                <dd><input type="password"></dd>
                <dt>Email</dt>
                <dd><input type="email"></dd>
            </dl>
            <button class="btn w-100">Login</button>
        </div>
    </body>
</html>
