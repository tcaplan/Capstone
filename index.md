<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
			<meta name="viewport" content="width=device-width, inital-scale=1">
			<link rel="stylesheet" href='capstone.css'>
			<title>Kinematics Calculator</title>
		<style>

		</style>

	</head>
	<body background="https://user-images.githubusercontent.com/66643794/119005729-b71a8e00-b95d-11eb-86db-157a04f3cb77.png">
		<table>
			<tr>
				<td>
					<h1>Kinematics Calculator</h1>
				</td>
				<td>
					<h2>(1-Dimension)</h2>
				</td>
			</tr>
		</table>
		<p>Click on the buttons inside the tabbed menu:</p>

		<div class="tab">
		  <button class="tablinks" onclick="openTab(event, 'x0')">Find Initial Position</button>
		  <button class="tablinks" onclick="openTab(event, 'v0')">Find Initial Velocity</button>
		  <button class="tablinks" onclick="openTab(event, 'x')">Find Position</button>
		  <button class="tablinks" onclick="openTab(event, 'v')">Find Velocity</button>
		  <button class="tablinks" onclick="openTab(event, 'a')">Find Acceleration</button>
		  <button class="tablinks" onclick="openTab(event, 't')">Find Time</button>
		</div>

		<div id="x0" class="tabcontent" style="background-color:#E9E9E9">
		  <h3>Initial Position, x<sub>0</sub></h3>

		  <div id="btnx0" style="display:inline">
			Choose equation:
			<br>
			<!-- Equation 2 -->
			   <button type=button id="eq2x0" onclick="showHide(x0Eq2, btnx0)">
					<b>
						<var>x<sub>f</sub></var> = <var>x<sub>0</sub></var> +
							<var>v<sub>0</sub>t</var> +
							<var><sup>1</sup>&frasl;<sub>2</sub>at<sup>2</sup></var>
					</b>
				</button>
				<!--Equation 3-->
				<button type=button id="eq3x0" onclick="showHide(x0Eq3, btnx0)">
					<b>
						<var>v<sub>f</sub><sup>2</sup></var> =
							<var>v<sub>0</sub><sup>2</sup></var> +
							<var>2a</var>(<var>x<sub>f</sub></var> -
							<var>x<sub>0</sub></var>)
					</b>
				</button>
				<br>
			</div>

			<!--Input boxes-->
			<!--Equation 2-->
			<div id="x0Eq2" style="display:none">
				<var>x<sub>f</sub></var> = <var>x<sub>0</sub></var> +
					<var>v<sub>0</sub>t</var> +
					<var><sup>1</sup>&frasl;<sub>2</sub>at<sup>2</sup></var>

				<br>
				<label for="x0x2"><var>x</var> = </label>
				<input type="number" id=x0x2 value=null style="width:50px;"></input> <br>
				<label for="x0v02"><var>v<sub>0</sub></var> = </label>
				<input type="number" id=x0v02 value=null style="width:50px;"></input> <br>
				<label for="x0a2"><var>a</var> = </label>
				<input type="number" id=x0a2 value=null style="width:50px;"></input> <br>
				<label for="x0t2"><var>t</var> = </label>
				<input type="number" id=x0t2 value=null style="width:50px;"></input> <br>

				<br>

				<button type="button" onclick="calculate('x0', 'E2')">Calculate</button>
				<button type="button" onclick="showHide(btnx0, x0Eq2)">Back</button>
			</div>

			<div id="x0Eq3" style="display:none">
				<var>v<sub>f</sub><sup>2</sup></var> =
					<var>v<sub>0</sub><sup>2</sup></var> +
					<var>2a</var>(<var>x<sub>f</sub></var> -
					<var>x<sub>0</sub></var>)

				<br>
				<label for="x0v3"><var>v</var> = </label>
				<input type="number" id=x0v3 value=null style="width:50px;"></input> <br>
				<label for="x0v03"><var>v<sub>0</sub></var> = </label>
				<input type="number" id=x0v03 value=null style="width:50px;"></input> <br>
				<label for="x0a3"><var>a</var> = </label>
				<input type="number" id=x0a3 value=null style="width:50px;"></input> <br>
				<label for="x0x3"><var>x</var> = </label>
				<input type="number" id=x0x3 value=null style="width:50px;"></input> <br>

				<br>

				<button type="button" onclick="calculate('x0', 'E3')">Calculate</button>
				<button type="button" onclick="showHide(btnx0, x0Eq3)">Back</button>
			</div>

		  <p id="output"><var>x<sub>0</sub></var> = </p>
		</div>

		<div id="v0" class="tabcontent" style="background-color:#E9E9E9">
		  <h3>Initial Velocity, v<sub>0</sub></h3>
		  <p>Something</p>
		</div>

		<div id="x" class="tabcontent" style="background-color:#E9E9E9">
		  <h3>Position, x</h3>
		  <p>Something</p>
		</div>

		<div id="v" class="tabcontent" style="background-color:#E9E9E9">
		  <h3>Velocity, v</h3>
		  <p>Something</p>
		</div>

		<div id="a" class="tabcontent" style="background-color:#E9E9E9">
		  <h3>Acceleration, a</h3>
		  <p>Something</p>
		</div>

		<div id="t" class="tabcontent" style="background-color:#E9E9E9">
		  <h3>Time, t</h3>
		  <p>Something</p>
		</div>

		<script src="capstone.js"> </script>


	</body>
</html>