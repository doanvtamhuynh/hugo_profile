---
author: Hugo Authors
title: Series Part 1
date: 2021-08-14
description: Hướng dẫn ngắn gọn về cách thiết lập phần 1 của series
series:
  - series-setup
---

Trong phần đầu tiên của loạt bài này, chúng tôi sẽ chỉ cho bạn cách tạo một loạt bài

<!--more-->

Bước đầu tiên, chúng ta cần thêm series dưới dạng phân loại. Chúng ta có thể thực hiện việc này bằng cách chỉnh sửa `config.toml`.
Lưu ý: Chúng ta luôn cần phải xác định các phân loại hiện có.

```toml
[taxonomies]
    category = "categories"
    series = "series"
    tag = "tags"
```

Bây giờ chúng ta đã bật chuỗi, việc tiếp theo chúng ta cần làm là thêm tên chuỗi vào FrontMatter.
Đối với ví dụ của chúng ta, chúng ta sẽ sử dụng bài đăng này và phần tiếp theo.

Như bạn có thể thấy, chúng ta đã đặt chuỗi thành `series-setup`. Chúng ta cũng làm tương tự trong các phần tiếp theo của chuỗi.
Kết quả cuối cùng này sẽ là một Front Matter trông giống như thế này:

```md
---
author: Hugo Authors
title: Series Part 1
date: 2021-08-14
description: A brief guide to how to setup series part 1
series:
  - series-setup
---
```

Mỗi bài đăng riêng lẻ giờ đây cũng sẽ hiển thị các bài đăng khác trong chuỗi dưới tiêu đề `Bài đăng trong chuỗi này`.