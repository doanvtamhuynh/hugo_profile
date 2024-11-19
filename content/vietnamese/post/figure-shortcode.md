---
title: 'Shortcode Figure'
date: 2021-03-13T21:47:41+00:00
draft: false
tags:
  - demo
  - shortcode
---

Hugo có sẵn shortcode `figure`, giúp bạn dễ dàng thêm chú thích hoặc thuộc tính liên kết (hyperlink rel) vào hình ảnh. Tài liệu hướng dẫn chi tiết có tại đây:

[https://gohugo.io/content-management/shortcodes/#figure](https://gohugo.io/content-management/shortcodes/#figure)

Giao diện này có 3 lớp CSS dành riêng cho các phần tử hình ảnh (figure):

- `big`: Hình ảnh sẽ vượt qua giới hạn chiều rộng của khu vực nội dung chính.
- `left`: Hình ảnh sẽ trôi về bên trái.
- `right`: Hình ảnh sẽ trôi về bên phải.

Nếu một hình ảnh không được đặt lớp CSS, nó sẽ hiển thị như hình ảnh thông thường trong Markdown: `![]()`.

Dưới đây là một số ví dụ; lưu ý rằng các kiểu này chỉ áp dụng khi chiều rộng trang lớn hơn 1300px.

{{< figure src="https://via.placeholder.com/1600x800" alt="image" caption="figure-normal (không có lớp CSS nào)" >}}

Pellentesque posuere sem nec nunc varius, id hendrerit arcu consequat. Maecenas commodo, sapien ut gravida porttitor, dolor risus facilisis enim, eget pharetra nibh nisl porttitor sapien. Proin finibus elementum ligula sit amet hendrerit. Praesent et erat sodales ante accumsan pharetra non eu nulla. Sed vehicula consequat lorem, a fermentum ante faucibus quis. Aliquam erat volutpat. In vitae tincidunt dui. Proin sit amet ligula sodales, elementum tortor et, venenatis sem. Maecenas non nisl erat. Curabitur nec velit eros. Ut cursus lacus nisi, non pretium libero euismod et. Fusce luctus in nisi quis sollicitudin. Aenean nec blandit ligula. Duis ac felis lorem. Proin tellus tellus, dictum nec tempus sit amet, venenatis ac felis. Sed in pharetra nulla, non mollis sem.

{{< figure src="https://via.placeholder.com/1600x800" alt="image" caption="figure-big" class="big" >}}

Donec nec tincidunt est. Sed id metus in erat fringilla mattis at id turpis. Aliquam tempor vehicula faucibus. Phasellus consequat aliquam odio. Morbi a ex vitae sapien porta auctor. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec sit amet nulla arcu. Praesent ut tortor purus. Praesent id eros diam. Pellentesque vitae dolor at nibh ultrices accumsan eu id urna. Aliquam finibus interdum orci in varius. Pellentesque a enim condimentum, condimentum felis id, vehicula augue. Vivamus cursus commodo eros nec lacinia.

{{< figure src="https://via.placeholder.com/1600x800" alt="image" caption="figure-medium" class="medium" >}}

In a libero varius, luctus ligula et, bibendum tortor. Sed sit amet dui malesuada, mattis justo id, ultricies enim. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Aliquam sollicitudin cursus feugiat. Vivamus suscipit ipsum eget lobortis sollicitudin. Fusce vehicula neque tellus. Integer eu posuere quam, id laoreet tortor. Mauris sit amet turpis urna. Donec venenatis tempor dolor, nec laoreet orci aliquet et. Sed condimentum elit eu tristique aliquam. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Nunc luctus ipsum sit amet nisl maximus pellentesque.

{{< figure src="https://via.placeholder.com/1600x800" alt="image" caption="figure-small" class="small" >}}

Pellentesque posuere sem nec nunc varius, id hendrerit arcu consequat. Maecenas commodo, sapien ut gravida porttitor, dolor risus facilisis enim, eget pharetra nibh nisl porttitor sapien. Proin finibus elementum ligula sit amet hendrerit. Praesent et erat sodales ante accumsan pharetra non eu nulla. Sed vehicula consequat lorem, a fermentum ante faucibus quis. Aliquam erat volutpat. In vitae tincidunt dui. Proin sit amet ligula sodales, elementum tortor et, venenatis sem. Maecenas non nisl erat. Curabitur nec velit eros. Ut cursus lacus nisi, non pretium libero euismod et. Fusce luctus in nisi quis sollicitudin. Aenean nec blandit ligula. Duis ac felis lorem. Proin tellus tellus, dictum nec tempus sit amet, venenatis ac felis. Sed in pharetra nulla, non mollis sem.

{{< figure src="https://via.placeholder.com/1600x800" alt="image" caption="figure-tiny" class="tiny" >}}

Suspendisse fringilla malesuada massa, in malesuada orci lacinia a. Praesent dapibus faucibus nisl, id volutpat elit bibendum eu. Nulla vitae laoreet nibh, eu hendrerit lacus. Donec lacinia auctor ligula, vel interdum ipsum malesuada vitae. Donec placerat a justo eu gravida. Aenean ultricies imperdiet convallis. Pellentesque accumsan non ex sed euismod. Proin bibendum lectus nec enim faucibus feugiat. Donec hendrerit nisi viverra ornare luctus. Nullam non viverra nisl. Nam vel tellus et tortor elementum volutpat sit amet et erat. Aliquam a libero quis libero porta consectetur. Etiam aliquam felis vel nulla mattis finibus. Mauris laoreet lacus arcu, sed rhoncus odio condimentum sed. Aenean in dui rutrum elit faucibus faucibus nec fringilla augue. Fusce non ornare mauris.

{{< figure src="https://via.placeholder.com/400x280" alt="image" caption="figure-left" class="left" >}}

Trong chế độ hiển thị nhỏ, hình ảnh sẽ tự động căn chỉnh phù hợp. Với nội dung trôi trái và phải, hãy sử dụng các lớp `left` hoặc `right`. 

---

Nếu bạn cần thêm các điều chỉnh khác hoặc nội dung dịch cụ thể hơn, cứ yêu cầu nhé! 😊
