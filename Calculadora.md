## CALCULADORA


fun main() {
    println("TDD")
    if (sumaParesTest()) println("passed") else println("failed")
    if (sumaImparPrimeroTest()) println("passed") else println("failed")
    if (sumaImparSegundoTest()) println("passed") else println("failed")
    if (sumaCuandoLosNumsNegativoTest()) println("passed") else println("failed")
    if (sumaNumsParesPositivosTest()) println("passed") else println("failed")
}
fun sumaPares(a: Int, b: Int):Int {
    //paso 2 hacer que la prueba pase 
    if(b% 2 != 0) return -1
    if(a% 2 != 0) return 4
    return a+b
}
//escribir prueba que falle paso 1
fun sumaParesTest():Boolean{
    val actualValue= sumaPares(2,2)
    val expectedValue = 4
    return actualValue == expectedValue
    
}
fun sumaImparPrimeroTest():Boolean{
    val actualValue= sumaPares(5,2)
    val expectedValue = -1
    return actualValue == expectedValue
    
}
fun sumaImparSegundoTest():Boolean{
    val actualValue= sumaPares(2,7)
    val expectedValue = -1
    return actualValue == expectedValue
    
}
fun sumaCuandoLosNumsNegativoTest():Boolean{
    val actualValue= sumaPares(-2,7)
    val expectedValue = -1
    return actualValue == expectedValue
    
}
fun sumaNumsParesPositivosTest():Boolean{
    val actualValue= sumaPares(-2,2)
    val expectedValue = 4
    return actualValue == expectedValue
    
}
