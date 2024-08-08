```bash
curl -sSik http://192.168.224.246:80/
```

[/home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_curl.html](file:///home/kali/Documents/Relia/results/192.168.224.246/scans/tcp80/tcp_80_http_curl.html):

```
HTTP/1.1 200 OK
Date: Wed, 03 Apr 2024 03:57:13 GMT
Server: Apache/2.4.52 (Ubuntu)
Vary: Accept-Encoding
Content-Length: 1516
Content-Type: text/html; charset=UTF-8



<!DOCTYPE html>
<html >
<head>
	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<title>Code Validation</title>
	<base target="_self">

	<script src="js/jquery-1.12.4.min.js"></script>
	<script src="js/scripts.js"></script>
	<link rel="stylesheet" href="css/bootstrap.min.css" />
	<!-- <link rel="stylesheet" href="css/styles.css" /> -->
</head>
<body>
<hr>
	<div class="container">
		<div class="row">
			<div class="col-md-4 col-md-offset-4">
				<div class="panel panel-default">
					<div class="panel-body">
						<div class="text-center">
							<h3><i class="glyphicon glyphicon-globe gi-4x"></i></h3>
							<h2 class="text-center">Code Validation</h2>
							<p>Provide your entry code here.</p>
							<div class="panel-body">
								<form class="form">
								<fieldset>
									<div class="input-group">
										<span class="input-group-addon">
											<i class="glyphicon glyphicon-lock color-blue"></i>
										</span>
										<input id="code_input" placeholder="Enter code here" class="form-control" required="">
										<input id="hidden_nonce" type="hidden" value="jE1h3xOI1k2bUP4ASYWf">
									</div>
									</div>
									<input class="btn btn-lg btn-primary btn-block" value="Submit Code" type="button" onclick="javascript:sendCode()">
								</div>
								</fieldset>
								</form>
								<div id="response"></div>

							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</body>
</html>

```
