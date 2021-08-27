<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>空白</title>
</head>
<body>
404
</body>
</html>

<?php

include("flag.php");

class G2mtu{
    private $key = '100';
    private $secret = 'abc';

    public function __construct($key,$file){
        $this->key = $key;
        $this->file = $file;
    }

    function __wakeup(){
        $this->key = '520';
    }

    function __destruct(){
        if ($this->key != 100) {
            echo "</br>gun~hacker!!!</br>";
            die();
        }
        if ($this->secret === 'abc') {
            global $flag;
            echo $flag;
        }else{
            echo "</br>hello my friend~~</br>sorry i can't give you the flag!";
            die();        
        }

    }
}
function is_valid($s) {
    for($i = 0; $i < strlen($s); $i++)
        if(!(ord($s[$i]) >= 32 && ord($s[$i]) <= 125))
            return false;
    return true;
}

if(isset($_GET{'a'})) {
    $a = (string)$_GET['a'];
    if(is_valid($a)) {
        @unserialize($a);
    }
}