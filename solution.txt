import Foundation

// Complete the staircase function below.
func staircase(n: Int) -> Void {
    for i in 1...n {
        print("\(Array(repeating: " ", count: n - i).joined())\(Array(repeating: "#",count: i).joined())")
    }
}

guard let n = Int((readLine()?.trimmingCharacters(in: .whitespacesAndNewlines))!)
else { fatalError("Bad input") }

staircase(n: n)
