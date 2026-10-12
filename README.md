# Branches

Мой учебный проект на Rust, в котором я практикуюсь в программировании и изучаю основные конструкции языка.

## О проекте

Проект создан в процессе изучения Rust. Здесь я сохраняю результаты практических заданий и закрепляю изученную теорию на практике.

## Код

```rust
fn main() {
    let mut count = 0;
    'counting_up: loop {
        println!("count = {count}");
        let mut remaining = 10;

        loop {
            println!("remaining = {remaining}");
            if remaining == 9 {
                break;
            }
            if count == 2 {
                break 'counting_up;
            }
            remaining -= 1;
        }

        count += 1;
    }
    println!("End count = {count}");
}

```
