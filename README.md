harveyneil-code
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Bootstrap Example</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
	<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.3.1/jquery.min.js"> </script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.2/js/bootstrap.min.js"></script>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.2/css/bootstrap.min.css">
    <link rel="stylesheet" 
        type="text/css" href="https://use.fontawesome.com/releases/v5.6.3/css/all.css">
    <style>
        #showModelB4Del {
            padding: 10px 50px!important;
            max-width: 500px;
            max-height: 300px;
            background: #edebee;
            color: black;
            border: 5px solid black;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            display: none;
            z-index: 99999999999999999999999999999;
        }
        
        .tableHolder_mail {
            height: 500px;
            overflow-y: auto
        }
        
        .closModalMsg {
            padding: 0.3rem 0.5rem;
            border-radius: 7px;
            background: red;
            color: white;
            position: absolute;
            top: 0px;
            right: 2px;
            cursor: pointer;
        }
        
        .b4Remove {
            transform: translateX(600px);
            opacity: 0.3;
            background: black!important;
        }
        
        table tbody tr {
            position: relative;
            transition: transform 0.5s;
        }
        
        .selectedRow_checkboxChecked {
            background: #ccc9ce
        }
		
		 #wrapper {
            margin: 0 auto;
            padding: 0px;
            text-align: center;
            width: 995px;
        }
  
        #wrapper h1 {
            margin-top: 50px;
            font-size: 45px;
            color: #585858;
        }
  
        #wrapper h1 p {
            font-size: 20px;
        }
  
        #table_detail {
            width: 500px;
            text-align: left;
            border-collapse: collapse;
            color: #2E2E2E;
            border: #A4A4A4;
        }
  
        #table_detail tr:hover {
            background-color: #878ac9;
        }
  
        #table_detail .hidden_row {
            display: none;
        }
    </style>
</head>

<body>

    <div class="container">
        <div class="view6">


            <div class="card">
                <div class="card-body">

                    <div class="tableHolder_mail">
                        <table class="table" id='table_filterNameEmail'>
                            <thead>
                                <tr>
                                    <th> <input type="checkbox" id='selectAll'> Select All</th>
                                    <th>Name</th>

                                </tr>
                            </thead>
                            <tbody>
                                <!--<tr>
                                    <td><input type='checkbox' class='checkbox_insideTBODY '></td>
                                    <td>Alfreds Futterkiste <span class='hiddenMessage_ifSkipped '>(Skipped)</span></td>
                                    <td>Futterkiste@example.com</td>

                                    <td>

                                        <button class='btn btn-danger DeleteSelectedRow '><i class="fa fa-times" aria-hidden="true"></i></button>
                                    </td>
                                </tr>
                                
								<tr onclick="showHideRow('hidden_row1');">
                                    <td><input type='checkbox' class='checkbox_insideTBODY '></td>
                                    <tr onclick="showHideRow('hidden_row1');"> 
										<td>Project-1</td>
										
									</tr>
										<tr id="hidden_row1" class="hidden_row">
										<td>
										 <p>From: Leo M'anoban (sbtest.khr@gmail.com) </p>
										
										</td>
										</tr>

                                    <td>

                                        <button class='btn btn-danger DeleteSelectedRow '><i class="fa fa-times" aria-hidden="true"></i></button>
                                    </td>
                                </tr> -->
		<div id="wrapper">
  
        <table border=1 id="table_detail" >
  
            
  
            <tr onclick="showHideRow('hidden_row1');">
				<td><input type='checkbox' class='checkbox_insideTBODY '></td>	
                <td>Project-1</td>
               
            
			
            <tr id="hidden_row1" class="hidden_row">
                <td colspan=1>
                 <p>From: Leo M'anoban (sbtest.khr@gmail.com) </p>
				 <p>Date: Mon, Jan 7, 2023 at 8:42AM		  </p>
				 <p>Subject: New project 1					  </p>
				 <p>To: Isabel Bowen (sbtest.isabel@gmail.com)</p>
                </td>
				</tr>
            </tr>
			<tr onclick="showHideRow('hidden_row1');">
				<td><input type='checkbox' class='checkbox_insideTBODY '></td>	
                <td>Project-2</td>
            
            <tr id="hidden_row1" class="hidden_row">
                <td colspan=1>
                 <p>From: Leo M'anoban (sbtest.khr@gmail.com) </p>
				 <p>Date: Mon, Jan 7, 2023 at 8:42AM		  </p>
				 <p>Subject: New project 1					  </p>
				 <p>To: Isabel Bowen (sbtest.isabel@gmail.com)</p>
                </td>
				</tr>
            </tr>
						<tr onclick="showHideRow('hidden_row1');">
				<td><input type='checkbox' class='checkbox_insideTBODY '></td>	
                <td>Project-3</td>
            </tr>
            <tr id="hidden_row1" class="hidden_row">
                <td colspan=1>
                 <p>From: Leo M'anoban (sbtest.khr@gmail.com) </p>
				 <p>Date: Mon, Jan 7, 2023 at 8:42AM		  </p>
				 <p>Subject: New project 1					  </p>
				 <p>To: Isabel Bowen (sbtest.isabel@gmail.com)</p>
                </td>
            </tr>
						<tr onclick="showHideRow('hidden_row1');">
				<td><input type='checkbox' class='checkbox_insideTBODY '></td>	
                <td>Project-4</td>
            </tr>
            <tr id="hidden_row1" class="hidden_row">
                <td colspan=1>
                 <p>From: Leo M'anoban (sbtest.khr@gmail.com) </p>
				 <p>Date: Mon, Jan 7, 2023 at 8:42AM		  </p>
				 <p>Subject: New project 1					  </p>
				 <p>To: Isabel Bowen (sbtest.isabel@gmail.com)</p>
                </td>
            </tr>
						<tr onclick="showHideRow('hidden_row1');">
				<td><input type='checkbox' class='checkbox_insideTBODY '></td>	
                <td>Project-5</td>
            </tr>
            <tr id="hidden_row1" class="hidden_row">
                <td colspan=1>
                 <p>From: Leo M'anoban (sbtest.khr@gmail.com) </p>
				 <p>Date: Mon, Jan 7, 2023 at 8:42AM		  </p>
				 <p>Subject: New project 1					  </p>
				 <p>To: Isabel Bowen (sbtest.isabel@gmail.com)</p>
                </td>
            </tr>
           
           
        </table>
    </div>


                            </tbody>


                        </table>
                    </div>

                </div>
            </div>


            <div class="card text-right">
                <div class="card-body ">

                    <div class="form-group mr-5">
                        <input type="submit" value='Delete All selected' class='btn btn-danger DeleteAllSelectedRow'>
                    </div>
                </div>
            </div>



        </div>

        
        <div id="showModelB4Del" class="px-2 py-2" style="">
            <h4>Are You Sure, You want to delete.</h4>
            <div class="d-flex">
                <a href="javascript:void(0)" id="yesDelContact" class="btn btn-success mr-3">Yes</a>
                
            </div>
            <span class="closModalMsg" id='closModalMsg'>X</span>
        </div>


        <script>
           
			 function showHideRow(row) {
            $("#" + row).toggle();
        }
            DeleteSelectedRow = document.querySelectorAll('.DeleteSelectedRow');
            DeleteSelectedRow.forEach(onebyone => {
                onebyone.addEventListener('click', function() {
                    {
                        currentROW = this.parentElement.parentElement;

                        document.getElementById('showModelB4Del').style.display = 'flex';
                        showModelB4Del = document.getElementById('showModelB4Del');
                        showModelB4Del.addEventListener('click', function(e) {
                            if (e.target.classList[0] == 'closModalMsg') {
                                showModelB4Del.style.display = 'none';
                            } else if (e.target.id == 'yesDelContact') {
                                setTimeout(function() {
                                    currentROW.classList.add('b4Remove');
                                    currentROW.addEventListener('transitionend', function() {
                                        currentROW.remove();
                                    })
                                }, 200)
                                showModelB4Del.style.display = 'none';
                            }

                        })
                    }
                })
            })

            

            selectAll = document.getElementById('selectAll');
            selectAll.addEventListener('click', function() {
                if (this.checked) {
                    tbody = this.parentElement.parentElement.parentElement.nextElementSibling;
                    AllInputs = [...tbody.querySelectorAll('input[type="checkbox"]')];

                    AllInputs.forEach(onebyone => {
                        onebyone.checked = true;

                        onebyone.parentElement.parentElement.classList.add('selectedRow_checkboxChecked')
                    })

                } else if (!this.checked) {
                    console.log('false  ')
                    tbody_false = this.parentElement.parentElement.parentElement.nextElementSibling;
                    AllInputs_false = [...tbody_false.querySelectorAll('input[type="checkbox"]')];

                    AllInputs_false.forEach(onebyone_false => {

                        onebyone_false.checked = false;
                        onebyone_false.parentElement.parentElement.classList.remove('selectedRow_checkboxChecked')
                    })

                }




            })

            checkbox_insideTBODY = document.querySelectorAll('.checkbox_insideTBODY');
            checkbox_insideTBODY.forEach(onebyone => {
                onebyone.addEventListener('click', function() {

                    currentTR = onebyone.parentElement.parentElement;
                    if (onebyone.checked == true) {
                        currentTR.classList.add('selectedRow_checkboxChecked')
                    } else {
                        currentTR.classList.remove('selectedRow_checkboxChecked')
                    }


                })
            })




            arrHolder_checked = [];

            main_allDelButton = document.getElementsByClassName('DeleteAllSelectedRow')[0];

            main_allDelButton.addEventListener('click', function() {

                checkbox_insideTBODY = document.querySelectorAll('.checkbox_insideTBODY');
                checkbox_insideTBODY.forEach(onebyone => {


                    if (onebyone.checked == true) {

                        CurrentTRs = onebyone.parentElement.parentElement;
                        arrHolder_checked.push(CurrentTRs)



                        document.getElementById('showModelB4Del').style.display = 'flex';
                        showModelB4Del = document.getElementById('showModelB4Del');
                        showModelB4Del.addEventListener('click', function(e) {
                            if (e.target.classList[0] == 'closModalMsg') {
                                showModelB4Del.style.display = 'none';
                            } else if (e.target.id == 'yesDelContact') {
                                setTimeout(function() {
                                    arrHolder_checked.forEach(onebyoneoncckbox => {
                                        onebyoneoncckbox.classList.add('b4Remove');
                                        onebyoneoncckbox.addEventListener('transitionend', function() {
                                            onebyoneoncckbox.remove();
                                            document.getElementById('selectAll').checked = false;
                                        })
                                    })

                                }, 200)
                                showModelB4Del.style.display = 'none';
                            }

                        })


                    }



                })



            })
        </script>


    </div>
</body>

</html>
