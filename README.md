# practice-html-<!DOCTYPE html>
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
        <title></title>
        <meta name="description" content="">
        <meta name="viewport" content="width=device-width">
		    <style>
      table {
        width: 100%;
      }
      table, th, td {
        border: 1px solid #bcbcbc;
      }
    </style>
 
    </head>
	
	<script src="http://code.jquery.com/jquery-latest.min.js"></script>
	
	<script>
		$(document).ready(function() {			
			
			$('#send_button').click(function() {
					
				var input_val = $('#receiver_select').val();
				
				$('#value_input').val(input_val);
				
				console.log(input_val);
				
			})
			
		})
	</script>
    
	<body>
        <!-- Add your site or application content here -->
		<table>
			<thead>
				<tr>
					<td colspan=2>
						<div id="mywallet_div" style="text-align:center"><h1>My Wallet</h1></div>
					</td>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>
						<h2> ACCOUNT 
							<select id="account_select">
									<option>1</option>
									<option>2</option>
									<option>3</option>
							</select> 
						</h2>
					</td>
					<td>
						<h2>BALANCE <input id="balance_input" type="number" value=""></h2>
					</td>
				</tr>
				<tr>
					<td>
						<h2> RECEIVE <input id="receiver_select"></input>  <h2/>
					</td>
					<td>
						<h2> VALUE <input id="value_input" type="text" value=""><br/></h2>
					</td>
				</tr>
					<td colspan=2>
						<h2> PASSWORD<input id="password_input" type="PASSWORD" value=""><br/><h2/>
								<button id="send_button">
								send
								</button>
							<div style="text-align:center">
								<button id="process_button" style="color: white; background:black; font-size:1em; border-radius:0.5em; padding:5px 20px;">
								Process payment
								</button>
							</div>
					</td>
			</tbody>
			
		</table>
    </body>
</html>
