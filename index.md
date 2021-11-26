<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Home</title>
    <link rel="stylesheet" type="text/css" href="css/style.css">
</head>
<body>
    <header>
        <div class="image_top">
            <img src="images/MicrosoftTeams-image (4).png">
        </div>
        <div class="menu">
            <a href="index.html">
                <button type="button" class="menubutt active">
                    Home
                </button>
            </a>
            <a href="Settings.html">
                <button type="button" class="menubutt">
                    Settings
                </button>
            </a>
            <a href="Report.html">
                <button type="button" class="menubutt">
                    Report
                </button>
            </a>
        </div>
    </header>
    <div class="body_container">
        <div>
            <a href="start.html">
                <button type="button" class="start">
                    START
                </button>
            </a>
        </div>
        <div>
            <a href="stop.html" >
                <button type="button" class="stop">
                    STOP
                </button>
            </a>
        </div>
    </div>
    <div class="main_container" id="front_main_container">
        <div class="color_container1">
            <img class="img_color" src="images/1.jpg">
            <div class="text_index">
                <h3>Color: Magenta</h3> <br>
                <h3>Basket: B1</h3>
            </div>
        </div>
        <div class="color_container1">
            <img class="img_color" src="images/1.jpg">
            <div class="text_index">
                <h3>Color: Magenta</h3> <br><h3>Color: Magenta</h3> <br>
                <h3>Basket: B1</h3>
            </div>
        </div>
        <div class="color_container1">
            <img class="img_color" src="images/1.jpg">
            <div class="text_index">
                <h3>Color: Magenta</h3><br>
                <h3>Basket: B1</h3>
            </div>
        </div>
        <div class="color_container1">
            <img class="img_color" src="images/1.jpg">
            <div class="text_index">
                <h3>Color: Magenta</h3> <br>
                <h3>Basket: B1</h3>
            </div>
        </div>
    </div>
</body>
<script>
    function displayfrontcards() {
        var cont_detailsf=[['1','Magenta','B1'],['1','Orange','B2'],['1','Green','B3'],['1','Yellow','B4']];
        var divvf='';
        for (let loop_cardf = 0; loop_cardf < cont_detailsf.length; loop_cardf++){
            divvf+='<div class="color_container1">';
            divvf+='<img class="img_color" src="images/'+cont_detailsf[loop_cardf][0]+'.jpg">';
            divvf+='<div class="text_index">';
            divvf+='<h3>Color: '+cont_detailsf[loop_cardf][1]+'</h3> <br>';
            divvf+='<h3>Basket: '+cont_detailsf[loop_cardf][2]+'</h3>';
            divvf+='</div>';
            divvf+='</div>';
        document.getElementById("front_main_container").innerHTML=divvf;
        }
    }
    displayfrontcards();
</script>
</html>
