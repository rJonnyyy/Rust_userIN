

use std::io;

//Funktion der Benutzereingabe für das Programm

fn get_benutzereingabe(wasgenau: &str) -> i32 {
    let mut benutzereingabe = String::new();
    println!("Gebe ein: {}", wasgenau);                     //hier wird der Kommentar erstellt, welcher zur Benutzereingabe angezeigt wird 
    io::stdin().read_line(&mut benutzereingabe).unwrap();
    let zahl: i32 = benutzereingabe
        .trim()
        .parse()
        .expect("not a valid i32 integer!");
    zahl //Rückgabe ist eine Zahl, die dem Tag / Monat / Jahr entspricht
}


gerne erweitern!! i16 u8 einlesen etc.