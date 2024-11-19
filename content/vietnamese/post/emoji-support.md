+++
author = "Tác giả Hugo"
title = "Hỗ trợ Emoji"
date = "2019-03-05"
description = "Hướng dẫn sử dụng emoji trong Hugo"
tags = [
    "emoji",
]
+++

Hugo hỗ trợ sử dụng emoji theo nhiều cách khác nhau.

<!--more-->

Hàm [`emojify`](https://gohugo.io/functions/emojify/) có thể được gọi trực tiếp trong các mẫu giao diện (templates) hoặc [Shortcode nội tuyến](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes).

Để bật emoji trên toàn bộ trang web, hãy đặt `enableEmoji` thành `true` trong [tệp cấu hình](https://gohugo.io/getting-started/configuration/) của bạn. Sau đó, bạn có thể sử dụng các mã viết tắt của emoji trực tiếp trong các tệp nội dung, ví dụ:

<p><span class="nowrap"><span class="emojify">🙈</span> <code>:see_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙉</span> <code>:hear_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙊</span> <code>:speak_no_evil:</code></span></p>
<br>

[Bảng mã Emoji](http://www.emoji-cheat-sheet.com/) là một tài liệu tham khảo hữu ích cho các mã viết tắt emoji.

---

**Lưu ý:** Các bước trên cho phép sử dụng các ký tự và chuỗi emoji theo Tiêu chuẩn Unicode trong Hugo, tuy nhiên việc hiển thị các biểu tượng này phụ thuộc vào trình duyệt và nền tảng. Để tùy chỉnh kiểu hiển thị của emoji, bạn có thể sử dụng font emoji của bên thứ ba hoặc sử dụng một bộ font kết hợp; ví dụ:

{{< highlight html >}}
.emoji {
font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji, Segoe UI Symbol, Android Emoji, EmojiSymbols;
}
{{< /highlight >}}

{{< css.inline >}}

<style>
.emojify {
	font-family: Apple Color Emoji, Segoe UI Emoji, NotoColorEmoji, Segoe UI Symbol, Android Emoji, EmojiSymbols;
	font-size: 2rem;
	vertical-align: middle;
}
@media screen and (max-width:650px) {
  .nowrap {
    display: block;
    margin: 25px 0;
  }
}
</style>

{{< /css.inline >}}
