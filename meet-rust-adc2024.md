---
theme:
  name: tokyonight-storm
  override:
    footer:
      style: template
      center: "Meet Rust: Getting Started, What's Special, and Why You Should Care"
      right: ""
---

<!-- new_lines: 12 -->

```text +no_background
██╗    ██╗███████╗██╗      ██████╗ ██████╗ ███╗   ███╗███████╗
██║    ██║██╔════╝██║     ██╔════╝██╔═══██╗████╗ ████║██╔════╝
██║ █╗ ██║█████╗  ██║     ██║     ██║   ██║██╔████╔██║█████╗  
██║███╗██║██╔══╝  ██║     ██║     ██║   ██║██║╚██╔╝██║██╔══╝  
╚███╔███╔╝███████╗███████╗╚██████╗╚██████╔╝██║ ╚═╝ ██║███████╗
 ╚══╝╚══╝ ╚══════╝╚══════╝ ╚═════╝ ╚═════╝ ╚═╝     ╚═╝╚══════╝
```
---
```text +no_background
Christian Jansen
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖▗▄▄▖  ▗▄▖ ▗▖  ▗▖ ▗▄▄▖ ▗▄▖ ▗▄▄▖  ▗▄▄▖
▐▌   ▐▌ ▐▌▐▌ ▐▌▐▛▚▖▐▌▐▌   ▐▌ ▐▌▐▌ ▐▌▐▌   
 ▝▀▚▖▐▛▀▘ ▐▌ ▐▌▐▌ ▝▜▌ ▝▀▚▖▐▌ ▐▌▐▛▀▚▖ ▝▀▚▖
▗▄▄▞▘▐▌   ▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘▝▚▄▞▘▐▌ ▐▌▗▄▄▞▘
```

![](assets/sponsors.png)

<!-- end_slide -->

```text +no_background
▗▄▄▄ ▗▄▄▄▖ ▗▄▄▖ ▗▄▄▖▗▖    ▗▄▖ ▗▄▄▄▖▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▄▖
▐▌  █  █  ▐▌   ▐▌   ▐▌   ▐▌ ▐▌  █  ▐▛▚▞▜▌▐▌   ▐▌ ▐▌▐▌   
▐▌  █  █   ▝▀▚▖▐▌   ▐▌   ▐▛▀▜▌  █  ▐▌  ▐▌▐▛▀▀▘▐▛▀▚▖ ▝▀▚▖
▐▙▄▄▀▗▄█▄▖▗▄▄▞▘▝▚▄▄▖▐▙▄▄▖▐▌ ▐▌▗▄█▄▖▐▌  ▐▌▐▙▄▄▖▐▌ ▐▌▗▄▄▞▘
```
---

<!-- pause -->

```text +no_background
1. I am not a professional Rust developer!
```

<!-- pause -->

```text +no_background
2. This is a high-level appetizer for Rust!
```

<!-- end_slide -->

<!-- new_lines: 9 -->

```text +no_background
 ██████╗ ███████╗████████╗████████╗██╗███╗   ██╗ ██████╗ 
██╔════╝ ██╔════╝╚══██╔══╝╚══██╔══╝██║████╗  ██║██╔════╝ 
██║  ███╗█████╗     ██║      ██║   ██║██╔██╗ ██║██║  ███╗
██║   ██║██╔══╝     ██║      ██║   ██║██║╚██╗██║██║   ██║
╚██████╔╝███████╗   ██║      ██║   ██║██║ ╚████║╚██████╔╝
 ╚═════╝ ╚══════╝   ╚═╝      ╚═╝   ╚═╝╚═╝  ╚═══╝ ╚═════╝ 
```
```text +no_background
███████╗████████╗ █████╗ ██████╗ ████████╗███████╗██████╗ 
██╔════╝╚══██╔══╝██╔══██╗██╔══██╗╚══██╔══╝██╔════╝██╔══██╗
███████╗   ██║   ███████║██████╔╝   ██║   █████╗  ██║  ██║
╚════██║   ██║   ██╔══██║██╔══██╗   ██║   ██╔══╝  ██║  ██║
███████║   ██║   ██║  ██║██║  ██║   ██║   ███████╗██████╔╝
╚══════╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝   ╚══════╝╚═════╝ 
```

<!-- end_slide -->

```text +no_background
▗▖ ▗▖▗▖ ▗▖ ▗▄▖▗▄▄▄▖    ▗▄▄▄▖ ▗▄▄▖    ▗▄▄▖ ▗▖ ▗▖ ▗▄▄▖▗▄▄▄▖
▐▌ ▐▌▐▌ ▐▌▐▌ ▐▌ █        █  ▐▌       ▐▌ ▐▌▐▌ ▐▌▐▌     █  
▐▌ ▐▌▐▛▀▜▌▐▛▀▜▌ █        █   ▝▀▚▖    ▐▛▀▚▖▐▌ ▐▌ ▝▀▚▖  █  
▐▙█▟▌▐▌ ▐▌▐▌ ▐▌ █      ▗▄█▄▖▗▄▄▞▘    ▐▌ ▐▌▝▚▄▞▘▗▄▄▞▘  █  
```

---

<!-- column_layout: [1, 4] -->
<!-- column: 1 -->

<!-- pause -->
<!-- incremental_lists: true -->

* **Low-level, with zero-cost abstractions**
* **Fast, achieving similar performance as C/C++**
* **Type-safe, preventing whole classes of errors at compilation**
* **Versatile, running on everything from embedded IoT devices to web servers**

<!-- end_slide -->

```text +no_background
▗▖  ▗▖ ▗▄▖ ▗▄▄▖ ▗▄▄▄▖ ▗▄▖ ▗▄▄▖ ▗▖   ▗▄▄▄▖ ▗▄▄▖
▐▌  ▐▌▐▌ ▐▌▐▌ ▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌   ▐▌   ▐▌   
▐▌  ▐▌▐▛▀▜▌▐▛▀▚▖  █  ▐▛▀▜▌▐▛▀▚▖▐▌   ▐▛▀▀▘ ▝▀▚▖
 ▝▚▞▘ ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖▐▌ ▐▌▐▙▄▞▘▐▙▄▄▖▐▙▄▄▖▗▄▄▞▘
```

```rust +line_numbers
// Declare variables with `let`
let value: i32 = 42;
```

<!-- end_slide -->

```text +no_background
▗▖  ▗▖ ▗▄▖ ▗▄▄▖ ▗▄▄▄▖ ▗▄▖ ▗▄▄▖ ▗▖   ▗▄▄▄▖ ▗▄▄▖
▐▌  ▐▌▐▌ ▐▌▐▌ ▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌   ▐▌   ▐▌   
▐▌  ▐▌▐▛▀▜▌▐▛▀▚▖  █  ▐▛▀▜▌▐▛▀▚▖▐▌   ▐▛▀▀▘ ▝▀▚▖
 ▝▚▞▘ ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖▐▌ ▐▌▐▙▄▞▘▐▙▄▄▖▐▙▄▄▖▗▄▄▞▘
```

```rust +line_numbers
// Declare variables with `let`
let value: i32 = 42;

// Type annotations are optional*
let value_two = 2024;
```

<!-- end_slide -->

```text +no_background
▗▖  ▗▖ ▗▄▖ ▗▄▄▖ ▗▄▄▄▖ ▗▄▖ ▗▄▄▖ ▗▖   ▗▄▄▄▖ ▗▄▄▖
▐▌  ▐▌▐▌ ▐▌▐▌ ▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌   ▐▌   ▐▌   
▐▌  ▐▌▐▛▀▜▌▐▛▀▚▖  █  ▐▛▀▜▌▐▛▀▚▖▐▌   ▐▛▀▀▘ ▝▀▚▖
 ▝▚▞▘ ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖▐▌ ▐▌▐▙▄▞▘▐▙▄▄▖▐▙▄▄▖▗▄▄▞▘
```

```rust +line_numbers
// Declare variables with `let`
let value: i32 = 42;

// Type annotations are optional*
let value_two = 2024;

// Error!
value = 52;
```

<!-- end_slide -->

```text +no_background
▗▖  ▗▖ ▗▄▖ ▗▄▄▖ ▗▄▄▄▖ ▗▄▖ ▗▄▄▖ ▗▖   ▗▄▄▄▖ ▗▄▄▖
▐▌  ▐▌▐▌ ▐▌▐▌ ▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌   ▐▌   ▐▌   
▐▌  ▐▌▐▛▀▜▌▐▛▀▚▖  █  ▐▛▀▜▌▐▛▀▚▖▐▌   ▐▛▀▀▘ ▝▀▚▖
 ▝▚▞▘ ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖▐▌ ▐▌▐▙▄▞▘▐▙▄▄▖▐▙▄▄▖▗▄▄▞▘
```

```rust +line_numbers
// Make variables mutable with `mut`
let mut value: i32 = 42;

// Type annotations are optional*
let value_two = 2024;

// No more error!
value = 52;
```

<!-- end_slide -->

```text +no_background
▗▖  ▗▖ ▗▄▖ ▗▄▄▖ ▗▄▄▄▖ ▗▄▖ ▗▄▄▖ ▗▖   ▗▄▄▄▖ ▗▄▄▖
▐▌  ▐▌▐▌ ▐▌▐▌ ▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌   ▐▌   ▐▌   
▐▌  ▐▌▐▛▀▜▌▐▛▀▚▖  █  ▐▛▀▜▌▐▛▀▚▖▐▌   ▐▛▀▀▘ ▝▀▚▖
 ▝▚▞▘ ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖▐▌ ▐▌▐▙▄▞▘▐▙▄▄▖▐▙▄▄▖▗▄▄▞▘
```

```rust +exec +line_numbers
# #[allow(unused)]
# fn main() {
// Make variables mutable with `mut`
let mut value: i32 = 42;

// Type annotations are optional*
let value_two = 2024;

// No more error!
value = 52;

println!("`value` is: {value}");
# }
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖ ▗▄▖ ▗▖   ▗▖   ▗▄▄▄▖ ▗▄▄▖▗▄▄▄▖▗▄▄▄▖ ▗▄▖ ▗▖  ▗▖ ▗▄▄▖
▐▌   ▐▌ ▐▌▐▌   ▐▌   ▐▌   ▐▌     █    █  ▐▌ ▐▌▐▛▚▖▐▌▐▌   
▐▌   ▐▌ ▐▌▐▌   ▐▌   ▐▛▀▀▘▐▌     █    █  ▐▌ ▐▌▐▌ ▝▜▌ ▝▀▚▖
▝▚▄▄▖▝▚▄▞▘▐▙▄▄▖▐▙▄▄▖▐▙▄▄▖▝▚▄▄▖  █  ▗▄█▄▖▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘
```
```rust +exec +line_numbers
# #[allow(unused)]
# fn main() {
// Declare an array with a list in square brackets...
let arr: [i32; 5] = [5, 10, 15, 20, 25];

// ...or fill the array with a single value
let arr_two: [f32; 3] = [3.3; 3];

println!("The first value of `arr` is {0}", arr[0]);
println!("The first value of `arr_two` is {0}", arr_two[0]);
# }
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖ ▗▄▖ ▗▖   ▗▖   ▗▄▄▄▖ ▗▄▄▖▗▄▄▄▖▗▄▄▄▖ ▗▄▖ ▗▖  ▗▖ ▗▄▄▖
▐▌   ▐▌ ▐▌▐▌   ▐▌   ▐▌   ▐▌     █    █  ▐▌ ▐▌▐▛▚▖▐▌▐▌   
▐▌   ▐▌ ▐▌▐▌   ▐▌   ▐▛▀▀▘▐▌     █    █  ▐▌ ▐▌▐▌ ▝▜▌ ▝▀▚▖
▝▚▄▄▖▝▚▄▞▘▐▙▄▄▖▐▙▄▄▖▐▙▄▄▖▝▚▄▄▖  █  ▗▄█▄▖▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘
```
```rust +exec +line_numbers
# #[allow(unused)]
# fn main() {
let tuple: (i32, f64, u8) = (500, 6.4, 1);

// Access values with a period and the index...
println!("The first value is: {0}", tuple.0);

// ...or destructure with pattern-matching
let (x, y, z) = tuple;
println!("The value of y is: {y}");
# }
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖ ▗▄▖ ▗▖   ▗▖   ▗▄▄▄▖ ▗▄▄▖▗▄▄▄▖▗▄▄▄▖ ▗▄▖ ▗▖  ▗▖ ▗▄▄▖
▐▌   ▐▌ ▐▌▐▌   ▐▌   ▐▌   ▐▌     █    █  ▐▌ ▐▌▐▛▚▖▐▌▐▌   
▐▌   ▐▌ ▐▌▐▌   ▐▌   ▐▛▀▀▘▐▌     █    █  ▐▌ ▐▌▐▌ ▝▜▌ ▝▀▚▖
▝▚▄▄▖▝▚▄▞▘▐▙▄▄▖▐▙▄▄▖▐▙▄▄▖▝▚▄▄▖  █  ▗▄█▄▖▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘
```
```rust +exec +line_numbers
# #[allow(unused)]
# fn main() {
// Declare a vector with the `vec!` macro
let mut vector: Vec<i32> = vec![5, 10, 15, 20, 25];

println!("The third value in the vector is: {0}", vector[2]);

vector.push(30);
println!("The vector's length is: {0}", vector.len());

vector.pop();
println!("And now the length is: {0}", vector.len());
# }
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖ ▗▄▖ ▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▖       ▗▄▄▄▖▗▖    ▗▄▖ ▗▖ ▗▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌       ▐▌   ▐▌   ▐▌ ▐▌▐▌ ▐▌
▐▌   ▐▌ ▐▌▐▌ ▝▜▌  █  ▐▛▀▚▖▐▌ ▐▌▐▌       ▐▛▀▀▘▐▌   ▐▌ ▐▌▐▌ ▐▌
▝▚▄▄▖▝▚▄▞▘▐▌  ▐▌  █  ▐▌ ▐▌▝▚▄▞▘▐▙▄▄▖    ▐▌   ▐▙▄▄▖▝▚▄▞▘▐▙█▟▌
```

```rust +exec +line_numbers
# fn main() {
let number = 3;

if number < 5 {
    println!("The condition was true!");
} else {
    println!("The condition was false!");
}
# }
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖ ▗▄▖ ▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▖       ▗▄▄▄▖▗▖    ▗▄▖ ▗▖ ▗▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌       ▐▌   ▐▌   ▐▌ ▐▌▐▌ ▐▌
▐▌   ▐▌ ▐▌▐▌ ▝▜▌  █  ▐▛▀▚▖▐▌ ▐▌▐▌       ▐▛▀▀▘▐▌   ▐▌ ▐▌▐▌ ▐▌
▝▚▄▄▖▝▚▄▞▘▐▌  ▐▌  █  ▐▌ ▐▌▝▚▄▞▘▐▙▄▄▖    ▐▌   ▐▙▄▄▖▝▚▄▞▘▐▙█▟▌
```

```rust +exec +line_numbers
# fn main() {
let flag: bool = true;

let result: i32 = if flag { 50 } else { -50 };

println!("`result` is: {result}");
# }
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖ ▗▄▖ ▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▖       ▗▄▄▄▖▗▖    ▗▄▖ ▗▖ ▗▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌       ▐▌   ▐▌   ▐▌ ▐▌▐▌ ▐▌
▐▌   ▐▌ ▐▌▐▌ ▝▜▌  █  ▐▛▀▚▖▐▌ ▐▌▐▌       ▐▛▀▀▘▐▌   ▐▌ ▐▌▐▌ ▐▌
▝▚▄▄▖▝▚▄▞▘▐▌  ▐▌  █  ▐▌ ▐▌▝▚▄▞▘▐▙▄▄▖    ▐▌   ▐▙▄▄▖▝▚▄▞▘▐▙█▟▌
```

```rust +exec +line_numbers
# fn main() {
let flag: bool = false;

let result: i32 = if flag { 50 } else { -50 };

println!("`result` is: {result}");
# }
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖ ▗▄▖ ▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▖       ▗▄▄▄▖▗▖    ▗▄▖ ▗▖ ▗▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌       ▐▌   ▐▌   ▐▌ ▐▌▐▌ ▐▌
▐▌   ▐▌ ▐▌▐▌ ▝▜▌  █  ▐▛▀▚▖▐▌ ▐▌▐▌       ▐▛▀▀▘▐▌   ▐▌ ▐▌▐▌ ▐▌
▝▚▄▄▖▝▚▄▞▘▐▌  ▐▌  █  ▐▌ ▐▌▝▚▄▞▘▐▙▄▄▖    ▐▌   ▐▙▄▄▖▝▚▄▞▘▐▙█▟▌
```

```rust +exec +line_numbers
# fn main() {
let mut count = 0;

// `loop` goes forever, or until a `break`
loop {
    count += 1;

    if count >= 10 {
        break;
    }
}

println!("Count: {count}");
# }
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖ ▗▄▖ ▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▖       ▗▄▄▄▖▗▖    ▗▄▖ ▗▖ ▗▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌       ▐▌   ▐▌   ▐▌ ▐▌▐▌ ▐▌
▐▌   ▐▌ ▐▌▐▌ ▝▜▌  █  ▐▛▀▚▖▐▌ ▐▌▐▌       ▐▛▀▀▘▐▌   ▐▌ ▐▌▐▌ ▐▌
▝▚▄▄▖▝▚▄▞▘▐▌  ▐▌  █  ▐▌ ▐▌▝▚▄▞▘▐▙▄▄▖    ▐▌   ▐▙▄▄▖▝▚▄▞▘▐▙█▟▌
```

```rust +exec +line_numbers
# fn main() {
let mut count = 0;

// `while` loops as long as the condition is true
while count < 15 {
    count += 1;
}

println!("Count: {count}");
# }
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖ ▗▄▖ ▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▖       ▗▄▄▄▖▗▖    ▗▄▖ ▗▖ ▗▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌  █  ▐▌ ▐▌▐▌ ▐▌▐▌       ▐▌   ▐▌   ▐▌ ▐▌▐▌ ▐▌
▐▌   ▐▌ ▐▌▐▌ ▝▜▌  █  ▐▛▀▚▖▐▌ ▐▌▐▌       ▐▛▀▀▘▐▌   ▐▌ ▐▌▐▌ ▐▌
▝▚▄▄▖▝▚▄▞▘▐▌  ▐▌  █  ▐▌ ▐▌▝▚▄▞▘▐▙▄▄▖    ▐▌   ▐▙▄▄▖▝▚▄▞▘▐▙█▟▌
```

```rust +exec +line_numbers
# #[allow(unused)]
# fn main() {
let mut count = 0;

// `for` iterates through a range
for i in 0..20 {
    count += 1;
}

println!("Count: {count}");
# }
```

<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▖ ▗▖▗▖  ▗▖ ▗▄▄▖▗▄▄▄▖▗▄▄▄▖ ▗▄▖ ▗▖  ▗▖ ▗▄▄▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌▐▌     █    █  ▐▌ ▐▌▐▛▚▖▐▌▐▌   
▐▛▀▀▘▐▌ ▐▌▐▌ ▝▜▌▐▌     █    █  ▐▌ ▐▌▐▌ ▝▜▌ ▝▀▚▖
▐▌   ▝▚▄▞▘▐▌  ▐▌▝▚▄▄▖  █  ▗▄█▄▖▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘
```

```rust +line_numbers
# #[allow(unused)]
// Declare functions with `fn`
fn main() {
    println!("Hello, world!");
}
```

<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▖ ▗▖▗▖  ▗▖ ▗▄▄▖▗▄▄▄▖▗▄▄▄▖ ▗▄▖ ▗▖  ▗▖ ▗▄▄▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌▐▌     █    █  ▐▌ ▐▌▐▛▚▖▐▌▐▌   
▐▛▀▀▘▐▌ ▐▌▐▌ ▝▜▌▐▌     █    █  ▐▌ ▐▌▐▌ ▝▜▌ ▝▀▚▖
▐▌   ▝▚▄▞▘▐▌  ▐▌▝▚▄▄▖  █  ▗▄█▄▖▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘
```

```rust +line_numbers
# #[allow(unused)]
// Declare functions with `fn`
fn main() {
    println!("Hello, world!");
}

// Parameters must be type-annotated
fn print_num(num: i32) {
    println!("The number is: {num}");
}
```

<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▖ ▗▖▗▖  ▗▖ ▗▄▄▖▗▄▄▄▖▗▄▄▄▖ ▗▄▖ ▗▖  ▗▖ ▗▄▄▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌▐▌     █    █  ▐▌ ▐▌▐▛▚▖▐▌▐▌   
▐▛▀▀▘▐▌ ▐▌▐▌ ▝▜▌▐▌     █    █  ▐▌ ▐▌▐▌ ▝▜▌ ▝▀▚▖
▐▌   ▝▚▄▞▘▐▌  ▐▌▝▚▄▄▖  █  ▗▄█▄▖▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘
```

```rust +line_numbers
# #[allow(unused)]
// Declare functions with `fn`
fn main() {
    println!("Hello, world!");
}

// Parameters must be type-annotated
fn print_num(num: i32) {
    println!("The number is: {num}");
}

// To declare a return type, use an arrow
fn double_num(num: i32) -> i32 {
    return num * 2;
}
```

<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▖ ▗▖▗▖  ▗▖ ▗▄▄▖▗▄▄▄▖▗▄▄▄▖ ▗▄▖ ▗▖  ▗▖ ▗▄▄▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌▐▌     █    █  ▐▌ ▐▌▐▛▚▖▐▌▐▌   
▐▛▀▀▘▐▌ ▐▌▐▌ ▝▜▌▐▌     █    █  ▐▌ ▐▌▐▌ ▝▜▌ ▝▀▚▖
▐▌   ▝▚▄▞▘▐▌  ▐▌▝▚▄▄▖  █  ▗▄█▄▖▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘
```

```rust +line_numbers
# #[allow(unused)]
// Declare functions with `fn`
fn main() {
    println!("Hello, world!");
}

// Parameters must be type-annotated
fn print_num(num: i32) {
    println!("The number is: {num}");
}

// To declare a return type, use an arrow
fn double_num(num: i32) -> i32 {
    return num * 2;
}

// Implicit return statement
fn product(num: i32, num_two: i32) -> i32 {
    num * num_two
}
```

<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▖ ▗▖▗▖  ▗▖ ▗▄▄▖▗▄▄▄▖▗▄▄▄▖ ▗▄▖ ▗▖  ▗▖ ▗▄▄▖
▐▌   ▐▌ ▐▌▐▛▚▖▐▌▐▌     █    █  ▐▌ ▐▌▐▛▚▖▐▌▐▌   
▐▛▀▀▘▐▌ ▐▌▐▌ ▝▜▌▐▌     █    █  ▐▌ ▐▌▐▌ ▝▜▌ ▝▀▚▖
▐▌   ▝▚▄▞▘▐▌  ▐▌▝▚▄▄▖  █  ▗▄█▄▖▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘
```

```rust +line_numbers
# #[allow(unused)]
// Declare functions with `fn`
fn main() {
    println!("Hello, world!");
}

// Parameters must be type-annotated
fn print_num(num: i32) {
    println!("The number is: {num}");
}

// To declare a return type, use an arrow
fn double_num(num: i32) -> i32 {
    return num * 2;
}

// Implicit return statement
fn product(num: i32, num_two: i32) -> i32 {
    num * num_two
}

// Multiple return values
fn multiple(num: i32) -> (i32, i32, i32) {
    (num * 2, num * 3, num * 4)
}
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖▗▄▄▄▖▗▄▄▖ ▗▖ ▗▖ ▗▄▄▖▗▄▄▄▖▗▄▄▖
▐▌     █  ▐▌ ▐▌▐▌ ▐▌▐▌     █ ▐▌   
 ▝▀▚▖  █  ▐▛▀▚▖▐▌ ▐▌▐▌     █  ▝▀▚▖
▗▄▄▞▘  █  ▐▌ ▐▌▝▚▄▞▘▝▚▄▄▖  █ ▗▄▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

```rust +line_numbers
// Declare a struct with `struct`...
struct Attendees {
    // ...and then any member variables with type annotations
    total_num: u64,
    attendee_id: Vec<u32>,
    attendee_age: Vec<u32>,
}
```

<!-- reset_layout -->
<!-- end_slide -->

```text +no_background
 ▗▄▄▖▗▄▄▄▖▗▄▄▖ ▗▖ ▗▖ ▗▄▄▖▗▄▄▄▖▗▄▄▖
▐▌     █  ▐▌ ▐▌▐▌ ▐▌▐▌     █ ▐▌   
 ▝▀▚▖  █  ▐▛▀▚▖▐▌ ▐▌▐▌     █  ▝▀▚▖
▗▄▄▞▘  █  ▐▌ ▐▌▝▚▄▞▘▝▚▄▄▖  █ ▗▄▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

```rust +line_numbers
// Declare a struct with `struct`...
struct Attendees {
    // ...and then any member variables with type annotations
    total_num: u64,
    attendee_id: Vec<u32>,
    attendee_age: Vec<u32>,
}

// Define functions in an `impl` block
impl Attendees {
    // "Associated functions" don't use `&self`
    // and are called with the double-colon (::)
    fn new() -> Self {
        Self {
            total_num: 0,
            attendee_id: vec![],
            attendee_age: vec![],
        }
    }

// Continued on second column...
```

<!-- column: 1 -->

```rust +line_numbers
// ...continued from first column

    // "Methods" use `&self`
    // and are called with a period (.)
    fn number_of_attendees(&self) -> u64 {
        self.total_num
    }

    // Methods can have other parameters too
    fn add_person(&mut self, id: u32, age: u32) {
        self.attendee_id.push(id);
        self.attendee_age.push(age);
        self.total_num += 1;
    }
}
```

<!-- reset_layout -->
<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▄▄▄▖▗▄▄▄▖▗▄▄▖
  █  ▐▌ ▐▌▐▌ ▐▌  █    █ ▐▌   
  █  ▐▛▀▚▖▐▛▀▜▌  █    █  ▝▀▚▖
  █  ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖  █ ▗▄▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

```rust +line_numbers
struct Attendees {
    total_num: u64,
    // ...
}

impl Attendees {
    fn new() -> Self {
    // ...
}
```

<!-- reset_layout -->
<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▄▄▄▖▗▄▄▄▖▗▄▄▖
  █  ▐▌ ▐▌▐▌ ▐▌  █    █ ▐▌   
  █  ▐▛▀▚▖▐▛▀▜▌  █    █  ▝▀▚▖
  █  ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖  █ ▗▄▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

```rust +line_numbers
struct Attendees {
    total_num: u64,
    // ...
}

impl Attendees {
    fn new() -> Self {
    // ...
}
```

<!-- column: 1 -->

```rust +line_numbers
// Define traits with `trait`
trait PartialEq {
    // ...
}
```

<!-- reset_layout -->
<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▄▄▄▖▗▄▄▄▖▗▄▄▖
  █  ▐▌ ▐▌▐▌ ▐▌  █    █ ▐▌   
  █  ▐▛▀▚▖▐▛▀▜▌  █    █  ▝▀▚▖
  █  ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖  █ ▗▄▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

```rust +line_numbers
struct Attendees {
    total_num: u64,
    // ...
}

impl Attendees {
    fn new() -> Self {
    // ...
}
```

<!-- column: 1 -->

```rust +line_numbers
// Define traits with `trait`
trait PartialEq {
    // No default implementation
    fn eq(&self, other: &Self) -> bool;

    // Default implementation provided
    fn ne(&self, other: &Self) -> bool {
        // ...
    }
}
```

<!-- reset_layout -->
<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▄▄▄▖▗▄▄▄▖▗▄▄▖
  █  ▐▌ ▐▌▐▌ ▐▌  █    █ ▐▌   
  █  ▐▛▀▚▖▐▛▀▜▌  █    █  ▝▀▚▖
  █  ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖  █ ▗▄▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

```rust +line_numbers
struct Attendees {
    total_num: u64,
    // ...
}

impl Attendees {
    fn new() -> Self {
    // ...
}
```

<!-- column: 1 -->

```rust +line_numbers
// Define traits with `trait`
trait PartialEq {
    // No default implementation
    fn eq(&self, other: &Self) -> bool;

    // Default implementation provided
    fn ne(&self, other: &Self) -> bool {
        // ...
    }
}

impl PartialEq for Attendees {
    // ...
}
```

<!-- reset_layout -->
<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▄▄▄▖▗▄▄▄▖▗▄▄▖
  █  ▐▌ ▐▌▐▌ ▐▌  █    █ ▐▌   
  █  ▐▛▀▚▖▐▛▀▜▌  █    █  ▝▀▚▖
  █  ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖  █ ▗▄▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

```rust +line_numbers
struct Attendees {
    total_num: u64,
    // ...
}

impl Attendees {
    fn new() -> Self {
    // ...
}
```

<!-- column: 1 -->

```rust +line_numbers
// Define traits with `trait`
trait PartialEq {
    // No default implementation
    fn eq(&self, other: &Self) -> bool;

    // Default implementation provided
    fn ne(&self, other: &Self) -> bool {
        // ...
    }
}

impl PartialEq for Attendees {
    fn eq(&self, other: &Self) -> bool {
        // Some custom implementation...
    }

    // No need to implement `ne`
}
```

<!-- reset_layout -->
<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▄▄▖  ▗▄▖ ▗▄▄▄▖▗▄▄▄▖▗▄▄▖
  █  ▐▌ ▐▌▐▌ ▐▌  █    █ ▐▌   
  █  ▐▛▀▚▖▐▛▀▜▌  █    █  ▝▀▚▖
  █  ▐▌ ▐▌▐▌ ▐▌▗▄█▄▖  █ ▗▄▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

```rust +line_numbers
struct Attendees {
    total_num: u64,
    // ...
}

impl Attendees {
    fn new() -> Self {
    // ...
}
```

<!-- column: 1 -->

```rust +line_numbers
// Define traits with `trait`
trait PartialEq {
    // No default implementation
    fn eq(&self, other: &Self) -> bool;

    // Default implementation provided
    fn ne(&self, other: &Self) -> bool {
        // ...
    }
}

impl PartialEq for Attendees {
    fn eq(&self, other: &Self) -> bool {
        // Some custom implementation...
    }

    // No need to implement `ne`
}
```
<!-- reset_layout -->

---
```text +no_background
COMPOSITION OVER INHERITANCE
```
---

<!-- end_slide -->

<!-- new_lines: 14 -->

```text +no_background
██╗    ██╗██╗  ██╗ █████╗ ████████╗███████╗    ███████╗██████╗ ███████╗ ██████╗██╗ █████╗ ██╗     
██║    ██║██║  ██║██╔══██╗╚══██╔══╝██╔════╝    ██╔════╝██╔══██╗██╔════╝██╔════╝██║██╔══██╗██║     
██║ █╗ ██║███████║███████║   ██║   ███████╗    ███████╗██████╔╝█████╗  ██║     ██║███████║██║     
██║███╗██║██╔══██║██╔══██║   ██║   ╚════██║    ╚════██║██╔═══╝ ██╔══╝  ██║     ██║██╔══██║██║     
╚███╔███╔╝██║  ██║██║  ██║   ██║   ███████║    ███████║██║     ███████╗╚██████╗██║██║  ██║███████╗
 ╚══╝╚══╝ ╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝   ╚══════╝    ╚══════╝╚═╝     ╚══════╝ ╚═════╝╚═╝╚═╝  ╚═╝╚══════╝
```

<!-- end_slide -->

```text +no_background
▗▄▄▄▖▗▄▖  ▗▄▖ ▗▖   ▗▄▄▄▖▗▖  ▗▖ ▗▄▄▖
  █ ▐▌ ▐▌▐▌ ▐▌▐▌     █  ▐▛▚▖▐▌▐▌   
  █ ▐▌ ▐▌▐▌ ▐▌▐▌     █  ▐▌ ▝▜▌▐▌▝▜▌
  █ ▝▚▄▞▘▝▚▄▞▘▐▙▄▄▖▗▄█▄▖▐▌  ▐▌▝▚▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

<!-- pause -->
## Cargo
<!-- pause -->
* Build management
```shell
% cargo build
% cargo run
```
<!-- pause -->
* Per-project dependency management
```shell
% cargo add some_package
    Updating crates.io index
    Adding some_package v4.5.18 to dependencies
    ...
```
<!-- pause -->
* Command-line tool installation
```shell
% cargo install cool-cli
    Updating crates.io index
    Installing cool-cli v0.8.0
    ...
% cool-cli
```

<!-- pause -->

<!-- column: 1 -->

## Rustfmt

* The official Rust code formatting tool
```shell
% rustfmt main.rs
```

<!-- pause -->

## Clippy

* A tool for more idiomatic Rust code
```shell
% cargo clippy
    Checking my_rust_project v0.1.0
    warning: unused variable: `var`
        ...
    warning: empty string literal in `println!`
        ...
```

<!-- pause -->

## Rustdoc

* Generates web-ready documentation from code comments

<!-- end_slide -->

```text +no_background
 ▗▄▖ ▗▖ ▗▖▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▄▖▗▖ ▗▖▗▄▄▄▖▗▄▄▖ 
▐▌ ▐▌▐▌ ▐▌▐▛▚▖▐▌▐▌   ▐▌ ▐▌▐▌   ▐▌ ▐▌  █  ▐▌ ▐▌
▐▌ ▐▌▐▌ ▐▌▐▌ ▝▜▌▐▛▀▀▘▐▛▀▚▖ ▝▀▚▖▐▛▀▜▌  █  ▐▛▀▘ 
▝▚▄▞▘▐▙█▟▌▐▌  ▐▌▐▙▄▄▖▐▌ ▐▌▗▄▄▞▘▐▌ ▐▌▗▄█▄▖▐▌   
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->
<!-- pause -->

```rust +exec +line_numbers
fn main() {
    let value = 42;
    println!("`value` is: {value}");

    borrow_int(&value);
    take_int(value);

    println!("`value` is still: {value}");
}

fn borrow_int(num: &i32) {
    let new_num = num / 2;
    println!("The borrowed number is: {new_num}")
}

fn take_int(mut num: i32) {
    num *= 2;
    println!("The taken number is: {num}");
}
```

<!-- pause -->
<!-- column: 1 -->

```rust +exec +line_numbers
fn main() {
    let value = vec![1, 2, 3, 4];
    println!("`value` is: {value:?}");

    borrow_vec(&value);
    take_vec(value);

    println!("`value` is still: {value:?}");
}

fn borrow_vec(vector: &Vec<i32>) {
    let length = vector.len();
    println!("The length is: {length}")
}

fn take_vec(mut vector: Vec<i32>) {
    let _ = vector.split_off(2);
    println!("The taken vector is: {vector:?}");
}
```

<!-- reset_layout -->
<!-- end_slide -->

```text +no_background
 ▗▄▖ ▗▖ ▗▖▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▄▖▗▖ ▗▖▗▄▄▄▖▗▄▄▖ 
▐▌ ▐▌▐▌ ▐▌▐▛▚▖▐▌▐▌   ▐▌ ▐▌▐▌   ▐▌ ▐▌  █  ▐▌ ▐▌
▐▌ ▐▌▐▌ ▐▌▐▌ ▝▜▌▐▛▀▀▘▐▛▀▚▖ ▝▀▚▖▐▛▀▜▌  █  ▐▛▀▘ 
▝▚▄▞▘▐▙█▟▌▐▌  ▐▌▐▙▄▄▖▐▌ ▐▌▗▄▄▞▘▐▌ ▐▌▗▄█▄▖▐▌   
```

## The Borrow-Checker strikes!

```shell
error[E0382]: borrow of moved value: `value`
  --> src/main.rs:8:33
   |
2  |     let value = vec![1, 2, 3, 4];
   |         ----- move occurs because `value` has type `Vec<i32>`, which does not implement the `Copy` trait
...
6  |     take_vec(value);
   |              ----- value moved here
7  |
8  |     println!("`value` is still: {value:?}");
   |                                 ^^^^^^^^^ value borrowed here after move
   |
note: consider changing this parameter type in function `take_vec` to borrow instead if owning the value isn't necessary
```

<!-- end_slide -->

```text +no_background
 ▗▄▖ ▗▖ ▗▖▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▄▖▗▖ ▗▖▗▄▄▄▖▗▄▄▖ 
▐▌ ▐▌▐▌ ▐▌▐▛▚▖▐▌▐▌   ▐▌ ▐▌▐▌   ▐▌ ▐▌  █  ▐▌ ▐▌
▐▌ ▐▌▐▌ ▐▌▐▌ ▝▜▌▐▛▀▀▘▐▛▀▚▖ ▝▀▚▖▐▛▀▜▌  █  ▐▛▀▘ 
▝▚▄▞▘▐▙█▟▌▐▌  ▐▌▐▙▄▄▖▐▌ ▐▌▗▄▄▞▘▐▌ ▐▌▗▄█▄▖▐▌   
```

```rust +line_numbers
fn main() {
    let value = vec![1, 2, 3, 4];
    println!("`value` is: {value:?}");

    borrow_vec(&value);
    take_vec(value);

    println!("`value` is still: {value:?}");
}

fn borrow_vec(vector: &Vec<i32>) {
    let length = vector.len();
    println!("The length is: {length}")
}

fn take_vec(mut vector: Vec<i32>) {
    let _ = vector.split_off(2);
    println!("The taken vector is: {vector:?}");
}
```

<!-- end_slide -->

```text +no_background
 ▗▄▖ ▗▖ ▗▖▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▄▖▗▖ ▗▖▗▄▄▄▖▗▄▄▖ 
▐▌ ▐▌▐▌ ▐▌▐▛▚▖▐▌▐▌   ▐▌ ▐▌▐▌   ▐▌ ▐▌  █  ▐▌ ▐▌
▐▌ ▐▌▐▌ ▐▌▐▌ ▝▜▌▐▛▀▀▘▐▛▀▚▖ ▝▀▚▖▐▛▀▜▌  █  ▐▛▀▘ 
▝▚▄▞▘▐▙█▟▌▐▌  ▐▌▐▙▄▄▖▐▌ ▐▌▗▄▄▞▘▐▌ ▐▌▗▄█▄▖▐▌   
```

```rust {1-20|6|1-20} +line_numbers
fn main() {
    let value = vec![1, 2, 3, 4];
    println!("`value` is: {value:?}");

    borrow_vec(&value);
    take_vec(value.clone());

    println!("`value` is still: {value:?}");
}

fn borrow_vec(vector: &Vec<i32>) {
    let length = vector.len();
    println!("The length is: {length}")
}

fn take_vec(mut vector: Vec<i32>) {
    let _ = vector.split_off(2);
    println!("The taken vector is: {vector:?}");
}
```

<!-- end_slide -->

```text +no_background
 ▗▄▖ ▗▖ ▗▖▗▖  ▗▖▗▄▄▄▖▗▄▄▖  ▗▄▄▖▗▖ ▗▖▗▄▄▄▖▗▄▄▖ 
▐▌ ▐▌▐▌ ▐▌▐▛▚▖▐▌▐▌   ▐▌ ▐▌▐▌   ▐▌ ▐▌  █  ▐▌ ▐▌
▐▌ ▐▌▐▌ ▐▌▐▌ ▝▜▌▐▛▀▀▘▐▛▀▚▖ ▝▀▚▖▐▛▀▜▌  █  ▐▛▀▘ 
▝▚▄▞▘▐▙█▟▌▐▌  ▐▌▐▙▄▄▖▐▌ ▐▌▗▄▄▞▘▐▌ ▐▌▗▄█▄▖▐▌   
```

```rust +exec +line_numbers
fn main() {
    let value = vec![1, 2, 3, 4];
    println!("`value` is: {value:?}");

    borrow_vec(&value);
    take_vec(value.clone());

    println!("`value` is still: {value:?}");
}

fn borrow_vec(vector: &Vec<i32>) {
    let length = vector.len();
    println!("The length is: {length}")
}

fn take_vec(mut vector: Vec<i32>) {
    let _ = vector.split_off(2);
    println!("The taken vector is: {vector:?}");
}
```

<!-- end_slide -->

```text +no_background
 ▗▄▄▖▗▄▄▖ ▗▄▄▄▖ ▗▄▄▖▗▄▄▄▖ ▗▄▖ ▗▖       ▗▄▄▄▖▗▖  ▗▖▗▖ ▗▖▗▖  ▗▖ ▗▄▄▖
▐▌   ▐▌ ▐▌▐▌   ▐▌     █  ▐▌ ▐▌▐▌       ▐▌   ▐▛▚▖▐▌▐▌ ▐▌▐▛▚▞▜▌▐▌   
 ▝▀▚▖▐▛▀▘ ▐▛▀▀▘▐▌     █  ▐▛▀▜▌▐▌       ▐▛▀▀▘▐▌ ▝▜▌▐▌ ▐▌▐▌  ▐▌ ▝▀▚▖
▗▄▄▞▘▐▌   ▐▙▄▄▖▝▚▄▄▖▗▄█▄▖▐▌ ▐▌▐▙▄▄▖    ▐▙▄▄▖▐▌  ▐▌▝▚▄▞▘▐▌  ▐▌▗▄▄▞▘
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->
<!-- pause -->

# Result

<!-- pause -->

```rust +line_numbers
enum Result<T, E> {
   Ok(T),
   Err(E),
}
```

<!-- pause -->

```rust +line_numbers
fn get_ip_addr() -> Result<u16, ()> {
    // Code that gets the IP address...

    if ip_addr != 0 {
        return Ok(ip_addr);
    } else {
        return Err(());
    }
}
```

<!-- column: 1 -->
<!-- pause -->

# Option

<!-- pause -->

```rust +line_numbers
enum Option<T> {
    None,
    Some(T),
}
```

<!-- pause -->

```rust +line_numbers
fn get_connected_devices() -> Option<Vec<u16>> {
    // Code to find all the connected devices...

    if device_vec.is_empty() {
        return None;
    } else {
        return Some(device_vec);
    }
}
```

<!-- reset_layout -->
<!-- pause -->

```rust +line_numbers
// Explicitly get the value from wrapper
result.unwrap();
```

<!-- end_slide -->

<!-- new_lines: 9 -->

```text +no_background
██╗    ██╗██╗  ██╗██╗   ██╗    ██╗   ██╗ ██████╗ ██╗   ██╗
██║    ██║██║  ██║╚██╗ ██╔╝    ╚██╗ ██╔╝██╔═══██╗██║   ██║
██║ █╗ ██║███████║ ╚████╔╝      ╚████╔╝ ██║   ██║██║   ██║
██║███╗██║██╔══██║  ╚██╔╝        ╚██╔╝  ██║   ██║██║   ██║
╚███╔███╔╝██║  ██║   ██║          ██║   ╚██████╔╝╚██████╔╝
 ╚══╝╚══╝ ╚═╝  ╚═╝   ╚═╝          ╚═╝    ╚═════╝  ╚═════╝ 
```
```text +no_background
███████╗██╗  ██╗ ██████╗ ██╗   ██╗██╗     ██████╗      ██████╗ █████╗ ██████╗ ███████╗
██╔════╝██║  ██║██╔═══██╗██║   ██║██║     ██╔══██╗    ██╔════╝██╔══██╗██╔══██╗██╔════╝
███████╗███████║██║   ██║██║   ██║██║     ██║  ██║    ██║     ███████║██████╔╝█████╗  
╚════██║██╔══██║██║   ██║██║   ██║██║     ██║  ██║    ██║     ██╔══██║██╔══██╗██╔══╝  
███████║██║  ██║╚██████╔╝╚██████╔╝███████╗██████╔╝    ╚██████╗██║  ██║██║  ██║███████╗
╚══════╝╚═╝  ╚═╝ ╚═════╝  ╚═════╝ ╚══════╝╚═════╝      ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝
```

<!-- end_slide -->

```text +no_background
▗▖ ▗▖▗▖ ▗▖▗▖  ▗▖    ▗▖  ▗▖▗▄▖ ▗▖ ▗▖     ▗▄▄▖▗▖ ▗▖ ▗▄▖ ▗▖ ▗▖▗▖   ▗▄▄▄      ▗▄▄▖ ▗▄▖ ▗▄▄▖ ▗▄▄▄▖
▐▌ ▐▌▐▌ ▐▌ ▝▚▞▘      ▝▚▞▘▐▌ ▐▌▐▌ ▐▌    ▐▌   ▐▌ ▐▌▐▌ ▐▌▐▌ ▐▌▐▌   ▐▌  █    ▐▌   ▐▌ ▐▌▐▌ ▐▌▐▌   
▐▌ ▐▌▐▛▀▜▌  ▐▌        ▐▌ ▐▌ ▐▌▐▌ ▐▌     ▝▀▚▖▐▛▀▜▌▐▌ ▐▌▐▌ ▐▌▐▌   ▐▌  █    ▐▌   ▐▛▀▜▌▐▛▀▚▖▐▛▀▀▘
▐▙█▟▌▐▌ ▐▌  ▐▌        ▐▌ ▝▚▄▞▘▝▚▄▞▘    ▗▄▄▞▘▐▌ ▐▌▝▚▄▞▘▝▚▄▞▘▐▙▄▄▖▐▙▄▄▀    ▝▚▄▄▖▐▌ ▐▌▐▌ ▐▌▐▙▄▄▖
```

---

<!-- pause -->

```text +no_background
Rust's focus on clarity results in code that is readable and maintainable
```

<!-- pause -->

```text +no_background
Rust's emphasis on explicit error-checking results in code that is robust and fault-tolerant
```

<!-- pause -->

```text +no_background
Rust's incredible performance and lack of garbage-collection make it a contender for almost every situation
```

<!-- pause -->

```text +no_background
Rust makes it easy to write good code
```

<!-- end_slide -->

```text +no_background
▗▖   ▗▄▄▄▖ ▗▄▖ ▗▄▄▖ ▗▖  ▗▖    ▗▖  ▗▖ ▗▄▖ ▗▄▄▖ ▗▄▄▄▖
▐▌   ▐▌   ▐▌ ▐▌▐▌ ▐▌▐▛▚▖▐▌    ▐▛▚▞▜▌▐▌ ▐▌▐▌ ▐▌▐▌   
▐▌   ▐▛▀▀▘▐▛▀▜▌▐▛▀▚▖▐▌ ▝▜▌    ▐▌  ▐▌▐▌ ▐▌▐▛▀▚▖▐▛▀▀▘
▐▙▄▄▖▐▙▄▄▖▐▌ ▐▌▐▌ ▐▌▐▌  ▐▌    ▐▌  ▐▌▝▚▄▞▘▐▌ ▐▌▐▙▄▄▖
```

<!-- column_layout: [1, 1] -->
<!-- column: 0 -->

<!-- pause -->

## Install Rust for yourself!
```
rust-lang.org/tools/install
```

<!-- pause -->

```text +no_background
----- OR -----
```

<!-- pause -->

## Try it in your browser!
```
play.rust-lang.org
```

<!-- column: 1 -->
<!-- pause -->

## Read *The Book*!
* "The Rust Programming Language"
```
doc.rust-lang.org/book
```

<!-- pause -->

```text +no_background
----- OR -----
```

<!-- pause -->

## Learn by example!
* "Rust by Example"
```
doc.rust-lang.org/rust-by-example
```

<!-- end_slide -->

<!-- new_lines: 12 -->

```text +no_background
████████╗██╗  ██╗ █████╗ ███╗   ██╗██╗  ██╗    ██╗   ██╗ ██████╗ ██╗   ██╗
╚══██╔══╝██║  ██║██╔══██╗████╗  ██║██║ ██╔╝    ╚██╗ ██╔╝██╔═══██╗██║   ██║
   ██║   ███████║███████║██╔██╗ ██║█████╔╝      ╚████╔╝ ██║   ██║██║   ██║
   ██║   ██╔══██║██╔══██║██║╚██╗██║██╔═██╗       ╚██╔╝  ██║   ██║██║   ██║
   ██║   ██║  ██║██║  ██║██║ ╚████║██║  ██╗       ██║   ╚██████╔╝╚██████╔╝
   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝╚═╝  ╚═╝       ╚═╝    ╚═════╝  ╚═════╝ 
```

---

```text +no_background
Have a great day!
```