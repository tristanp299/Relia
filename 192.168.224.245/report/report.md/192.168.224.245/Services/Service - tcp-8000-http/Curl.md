```bash
curl -sSik http://192.168.224.245:8000/
```

[/home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_curl.html](file:///home/kali/Documents/Relia/results/192.168.224.245/scans/tcp8000/tcp_8000_http_curl.html):

```
HTTP/1.1 200 OK
Date: Wed, 03 Apr 2024 03:59:26 GMT
Server: Apache/2.4.49 (Unix) OpenSSL/1.1.1f mod_wsgi/4.9.4 Python/3.8
Last-Modified: Wed, 12 Oct 2022 08:56:01 GMT
ETag: "6ad-5ead28fdcdb81"
Accept-Ranges: bytes
Content-Length: 1709
Content-Type: text/html

<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" href="style/style.css">
    <script src="js/main.js"></script>
</head>

<body>

    <h2>DEVELOPMENT</h2>

    <button id="open_login_button" onclick="showLoginDiv()">Login</button>

    <div id="login_div" class="modal">

        <form class="modal-content animate" action="javascript:doLogin()">
            <div class="imgcontainer">
                <span onclick="hideLoginDiv()" class="close" title="Close">&times;</span>
                <img src="./img/relia.png" alt="Avatar" class="avatar">
            </div>

            <div class="container">
                <label><b>Username</b></label>
                <input id="username" type="text" placeholder="Username" name="username" required>

                <label><b>Password</b></label>
                <input id="password" type="password" placeholder="Password" name="password" required>

                <button type="submit">Login</button>
                <input type="checkbox" checked="checked"> Remember me
            </div>

            <div class="container" id="response"></div>

            <div class="container" style="background-color:#f1f1f1">
                <button type="button" onclick="hideLoginDiv()" class="cancelbtn">Cancel</button>
                <span class="psw">Forgot <a href="#">password?</a></span>
            </div>
        </form>
    </div>

    <script>
        var modal = document.getElementById('login_div');
        window.onclick = function(event) {
            if (event.target == modal) {
                modal.style.display = "none";
            }
        }
    </script>
</body>

</html>

```
