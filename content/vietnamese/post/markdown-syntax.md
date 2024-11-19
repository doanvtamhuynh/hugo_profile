+++
author = "Hugo Authors"
title = "Hướng Dẫn Cú Pháp Markdown"
date = "2019-03-11"
description = "Bài viết mẫu giới thiệu cú pháp Markdown cơ bản và định dạng cho các phần tử HTML."
tags = [
    "markdown",
    "css",
    "html",
]
categories = [
    "themes",
    "syntax",
]
series = ["Themes Guide"]
aliases = ["migrate-from-jekyl"]
+++

Bài viết này cung cấp một ví dụ về cú pháp Markdown cơ bản có thể sử dụng trong các tệp nội dung Hugo, cũng như cho thấy liệu các phần tử HTML cơ bản có được trang trí bằng CSS trong một chủ đề Hugo hay không.

<!--more-->

## Đầu Mục (Headings)

Các phần tử HTML `<h1>`—`<h6>` đại diện cho sáu cấp độ tiêu đề. `<h1>` là cấp tiêu đề cao nhất trong khi `<h6>` là cấp thấp nhất.

# H1

## H2

### H3

#### H4

##### H5

###### H6

## Đoạn Văn

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Trích Dẫn (Blockquotes)

Phần tử trích dẫn đại diện cho nội dung được trích dẫn từ nguồn khác, có thể có hoặc không có nguồn trích dẫn (citation) và có thể có thay đổi nội dung như chú thích và viết tắt.

#### Trích dẫn không có nguồn

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Lưu ý** rằng bạn có thể sử dụng _cú pháp Markdown_ trong một trích dẫn.

#### Trích dẫn có nguồn

> Đừng giao tiếp bằng cách chia sẻ bộ nhớ, hãy chia sẻ bộ nhớ bằng cách giao tiếp.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: Câu trên được trích từ [bài nói chuyện](https://www.youtube.com/watch?v=PAAkCSZUG1c) của Rob Pike trong Gopherfest, ngày 18 tháng 11 năm 2015.

## Bảng (Tables)

Bảng không phải là một phần của đặc tả Markdown cơ bản, nhưng Hugo hỗ trợ chúng ngay ngoài hộp.

| Tên    | Tuổi |
| ------ | ---- |
| Bob    | 27   |
| Alice  | 23   |

#### Markdown trong bảng

| In nghiêng   | In đậm   | Mã lệnh  |
| ------------ | -------- | -------- |
| _in nghiêng_ | **in đậm** | `mã lệnh` |

## Khối Mã (Code Blocks)

#### Khối mã với dấu nháy đơn

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
#### Khối mã với shortcode highlight nội bộ của Hugo

{{< highlight html >}}

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <title>Example HTML5 Document</title>
  </head>
  <body>
    <p>Test</p>
  </body>
</html>

{{< /highlight >}}

## Các loại danh sách

#### Danh sách có thứ tự

1. Mục đầu tiên
2. Mục thứ hai
3. Mục thứ ba

#### Danh sách không có thứ tự

- Mục trong danh sách
- Mục khác trong danh sách
- Và một mục khác nữa

#### Danh sách lồng nhau

- Trái cây
  - Táo
  - Cam
  - Chuối
- Sữa phẩm
  - Sữa
  - Phô mai

## Các phần tử khác — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> là một định dạng hình ảnh bitmap.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Nhấn <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> để kết thúc phiên.

Hầu hết <mark>con kỳ nhông</mark> là động vật hoạt động về đêm và săn tìm côn trùng, giun, và các sinh vật nhỏ khác.
