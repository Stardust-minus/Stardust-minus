<!--suppress ALL -->

# 🤸 ஐ Stacker ஐ <img alt="GitHub followers" src="https://img.shields.io/github/followers/StackerDesu?style=flat-square&logo=github" /> <a href="https://twitter.com/StackerDesu"><img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/StackerDesu?style=flat-square&logo=twitter" /></a>


<img align="right" width="400" src="rain0.gif" />

```Rust
#![no_std] // Minimal kernel
#![no_main]
use core::panic::PanicInfo;
#[panic_handler]
fn panic(_info: &PanicInfo) -> ! { loop {} }
#[no_mangle]
pub extern "C" fn _start() -> ! {
    let message = "Hi, I am Stacker!"; // ☬
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
<code><img height="30" width="30" src="dotnet.png"></code>
<code><img height="30" width="30" src="csharp.png"></code>
<code><img height="30" width="30" src="python.png"></code>
<code><img height="30" width="30" src="cpp.png"></code>
<code><img height="30" width="30" src="golang.png"></code>

# 📃 〄 Analysis 〄

<img width="44%" align="left" src="https://github-readme-stats.vercel.app/api?username=StackerDesu&count_private=true&show_icons=true&theme=radical" />
<img width="44%" align ="right" src="https://github-readme-stats.vercel.app/api/top-langs/?username=StackerDesu&theme=radical" />
<img width="100%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=StackerDesu&theme=monokai" />

# 📞 ❅ Contact ❅

```text
Email: mistyraincloudservice@gmail.com
Twitter: @StackerDesu
Github: @StackerDesu
```

[![☬](https://img.shields.io/badge/-@StackerDesu-%23181717?style=flat-square&logo=github)](https://github.com/StackerDesu)
