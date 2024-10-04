//Faraz Waqar
//251707570
//CSCS468A

//============================================================================================

//Task 1
fun main() {
    println("Task 1")
    println()
    val day = "Thursday"
    if(day=="Monday"){
        println("On $day, the opening hours are: 8 AM to 12 PM (8:00 - 12:00)")
    }
    else if(day=="Tuesday" || day=="Wednesday" || day=="Thursday"){
        println("On $day, the opening hours are: 8 AM to 6 PM (8:00 - 18:00)")
    }
    else if(day=="Friday"){
        println("On $day, the opening hours are: 8 AM to 9 PM (8:00 - 21:00)")
    }
    else if(day=="Saturday"){
        println("On $day, the opening hours are: 9 AM to 4 PM (9:00 - 16:00)")
    }
    else if(day=="Sunday"){
        println("On $day, the opening hours are: 8 AM to 4 PM (8:00 - 16:00)")
    }
    else{
        println("Invalid Day")
    }
    
    //Alternative Way using "when"
    println()
    println()
    println("===Alternatice Way===")
    println()
    when(day){
        "Monday" -> println("On $day, the opening hours are: 8 AM to 12 PM (8:00 - 12:00)")
        "Tuesday", "Wednesday", "Thursday" -> println("On $day, the opening hours are: 8 AM to 6 PM (8:00 - 18:00)")
        "Friday" -> println("On $day, the opening hours are: 8 AM to 9 PM (8:00 - 21:00)")
        "Saturday" -> println("On $day, the opening hours are: 9 AM to 4 PM (9:00 - 16:00)")
        "Sunday" -> println("On $day, the opening hours are: 8 AM to 4 PM (8:00 - 16:00)")
        else -> println("Invalid Day")
    }
}

//============================================================================================

//Task 2 (Printing triangles of "*")
fun main() {
    println("Task 2: (Printing Triangle of Stars)")
    println()
    for(n in 0..5){
        for(m in 0..n){
            print("*")
        }
        println()
    }
}

//============================================================================================

//Task 3 (Game)
fun getPoints(basePoints: Int, boost: Int): Int{
    return basePoints * boost
}

fun main() {
    println("Task 2: Game")
    println()
    var score = 0;
    println(score)
    score += getPoints(10, 1)
    println(score)
    score += getPoints(20, 2)
    println(score)
    score+= getPoints(-10, 1)
    println(score)
    score += getPoints(5,3)
    println(score)
    score += getPoints(-15, 2)
}