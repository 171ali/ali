<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Discount Project</title>
</head>
<body>
    <script>
    var plan ={
        name: "Basic",
        price: 399,
        space: 100,
        transfar: 1000,
        page: 10,
        discountmonths : [6,7,8],
        callcAnnul:function(){
        var bestPrice = this.price;
        var currdate = new date();
        var thisMonth = currdate.getMonth();
        for ( var i=0; i<this.discountmonths.lenght; i++){
            if(this.discountmonths[i]=== thisMonth){
                bestPrice = this.price * discountmonths[i];
                break;
            }
        }
        return bestPrice * 12;
    }
    
    };
    // var annualprice = plan.callcAnnul(.85);
    // var anualPrice = callcAnnul();
    alert(plan.callcAnnul.bestPrice);
    </script>
</body>
</html>
