# formaction
<?php
if(isset($_POST['Submit'])){
    $first_name = $_POST['first_name'];
    $Last_name = $_POST['last_name'];
    $DOB = $_POST['DOB'];
    $phone = $_POST['phone'];
    $Gender = $_POST['gender'];
    $username = $_POST['username'];
    $create_password = $_POST['create_password'];
    $confirm_password = $_POST['confirm_password'];

    $array_data = [
        'first_name' => $first_name,
        'last_name' => $last_name,
        'DOB' => $DOB,
        'phone' => $phone,
        'gender' => $gender,
        'username' => $username,
        'create_password' => $create_password,
        'confirm_password' => $confirm_password,
    ];

    echo $first_name . $Last_name . $DOB . $Phone . $Gender . $username . $Create_password . $Confirm_password;
    file_put_contents(files/ . $array_data['first_name'] . ".txt", $array_data);
}

?>
