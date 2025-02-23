<!--suppress ALL -->

# 🤸 ஐ Stardust·星之尘埃 ஐ <img alt="GitHub followers" src="https://img.shields.io/github/followers/Stardust-minus?style=flat-square&logo=github" /> 


<img align="right" width="400" src="rain0.gif" />

```Rust
#![no_std] // Minimal kernel
#![no_main]
use core::panic::PanicInfo;
#[panic_handler]
fn panic(_info: &PanicInfo) -> ! { loop {} }
#[no_mangle]
pub extern "C" fn _start() -> ! {
    let message = "Hi, I am Stardust!"; // ☬
    let buffer = 0xb8000 as *mut u8;
    for (i, &b) in message.as_bytes().iter().enumerate() {
        unsafe { // ☈
            *buffer.offset(i as isize * 2) = b;
            *buffer.offset(i as isize * 2 + 1) = 0xb;
        }
    }
    loop {}
}
```

# 📕 ❀ Website ❀
[![Stardust Preview](https://hanabi-ai.cn/preview.png)](https://hanabi-ai.cn)

# 📃 〄 Analysis 〄

<img width="44%" align="left" src="https://github-readme-stats.vercel.app/api?username=Stardust-minus&count_private=true&show_icons=true&theme=radical" />
<img width="100%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Stardust-minus&theme=monokai" />

# 📞 ❅ Contact ❅

```text
Email: stardust@fish.audio
Bilibili: @Stardust_减
Github: @Stardust-minus
QQ:2225664821
```
