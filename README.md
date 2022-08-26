<!--suppress ALL -->

# 🤸 ஐ Stardust·星之尘埃 ஐ <img alt="GitHub followers" src="https://img.shields.io/github/followers/Stardust-minus?style=flat-square&logo=github" /> <a href="https://twitter.com/LITIANYU9"><img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/LITIANYU9?style=flat-square&logo=twitter" /></a>


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

# 📕 ❀ Languages ❀

<code><img height="30" width="30" src="rust.png"></code>
<code><img height="30" width="30" src="csharp.png"></code>
<code><img height="30" width="30" src="python.png"></code>
<code><img height="30" width="30" src="cpp.png"></code>
<code><img height="30" width="30" src="golang.png"></code>

# 📃 〄 Analysis 〄

<img width="44%" align="left" src="https://github-readme-stats.vercel.app/api?username=Stardust-minus&count_private=true&show_icons=true&theme=radical" />
<img width="44%" align ="right" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Stardust-minus&theme=radical" />
<img width="100%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Stardust-minus&theme=monokai" />

# 📞 ❅ Contact ❅

```text
Email: star_dust_chen@foxmail.com
Bilibili: @Stardust_减
Github: @Stardust-minus
```
