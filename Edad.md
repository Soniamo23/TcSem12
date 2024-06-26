## EDAD

fun validateAge(age: Int): String {
    
    //  si la edad es negativa
    if (age < 0) {
        return ("REJECTED")
    }
    
    //  la persona es mayor de edad
    return if (age >= 18) {
        ("ACCEPTED")
    } else {
        ("REJECTED")
    }
}

fun main() {
    
    println(validateAge(18))
    println(validateAge(-22))
    println(validateAge(2))
    
}
