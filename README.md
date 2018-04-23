<!DOCTYPE html>
<html>
<head>
	<title>Employee Form</title>
	 <link href="https://code.jquery.com/ui/1.12.1/themes/smoothness/jquery-ui.css" rel="stylesheet">
	<link href="styles.css" rel="stylesheet">
	<link href="employee-form.css" rel="stylesheet">
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
	<script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
	<script src="https://code.jquery.com/ui/1.12.1/jquery-ui.js"></script>
	<script src="emp-form.js"></script>
</head>
<body>
	<div class="content">
		<h1>Employee Form</h1>
		<form>
			<div class="input-group">
				
				<div><label for="firstname" class="label">First Name</label></div>
				<span class="input-group-addon"><i class="glyphicon glyphicon-user"></i></span>
				<input   id="firstname" type="text" required />
				<span class="message" id="firstnamemessage">&nbsp;</span>
			</div>
			<div class="input-group">
				
				<div><label for="lastname" class="label">Last Name</label></div>
				<span class="input-group-addon"><i class="glyphicon glyphicon-user"></i></span>
				<input   id="lastname" type="text" required />
				<span class="message" id="lastnamemessage">&nbsp;</span>
			</div>
			<div class="form-group">
				<div><label for="birthdate" class="label">Birth Date</label></div>
				<!-- Prevent the user from updating the date field manually. -->
				<input id="birthdate" type="text" readonly required />
				<span class="message" id="birthdatemessage">&nbsp;</span>
			</div>
			<div class="form-group">
				<div><label for="address" class="label">Address</label></div>
				<textarea id="address" required></textarea>
				<span class="message" id="addressmessage">&nbsp;</span>
			</div>
			<div class="form-group">
				<div><label for="postalcode" class="label">Postal Code</label></div>
				<select class="postalcodeselector" id="postalcodeselector">
					<option value="411" selected>Pune</option>
					<option value="400">Mumbai</option>
					<option value="600">Chennai</option>
					<option value="110">Delhi</option>
					<option value="560">Banglore</option>
				</select>
				<input class="postalcode" id="postalcode" type="text" value="411" required />
				<span class="message" id="postalcodemessage">&nbsp;</span>
			</div>
			<div class="form-group">
				<div><label for="photo" class="label">Photo</label></div>
				<input id="photo" type="file" required />
				<span class="message" id="photomessage">&nbsp;</span>
				<img class="preview" id="preview" src=""></img>
			</div>
			<div class="form-group">
				<input type="submit" value="Submit" />
			</div>
		</form>
	</div>
</body>
</html>
