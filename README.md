
<div dir="rtl">
 
# تمارين  - رقم 3


</div>

import UIKit

//function

func printMe(){
    print ("hello i'm noura")
    print ("i am 13 years old")
    print ("i like the color purple")
}

printMe()



var number1 = 5
var number2 = 3
func number (N:Int, B:Int) -> Int {
 
    return (N + B)/2
}



//password

import Foundation
func isValidPassword(password:String?) -> Bool {
    guard password != nil else { return false }
 
    // at least one uppercase,
    // at least one digit
    // at least one lowercase
    // 8 characters total
    let passwordTest = NSPredicate(format: "SELF MATCHES %@", "(?=.*[A-Z])(?=.*[0-9])(?=.*[a-z]).{8,}")
    return passwordTest.evaluate(with: password)
}

isValidPassword(password: "Abcd1234")
isValidPassword(password: "abcd1234")


func checkPassword(password:String) -> String {
    if password.count <= 8 {
      return "passwordIstValid"
    } else {
        return "passwordIsNotValid"
    }
    
}


checkPassword(password: "abc")
