# BigMac2
import 

var snake_array;  
function create_snake(){
    var length = 5;   
    snake_array = [] 
    for (var i = 0; i < length; i++) {
        snake_array.push({x:i,y:0});
    }
}

create_snake() // invoking the method

//painting the snake
function paint(){


    var nx = snake_array[0].x;
    var ny = snake_array[0].y;
    if(d == "right") nx++;    
    else if(d == "left") nx--;
    if(d == "up") ny--;
    if(d == "down") ny++;

    var tail = snake_array.pop(); // pops out the last cell
    tail.x = nx;
    tail.y = ny;
    snake_array.unshift(tail)

    

    }
}

paint() // invoking the method
