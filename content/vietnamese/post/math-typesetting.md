---
author: Hugo Authors
title: Định Dạng Toán Học
date: 2019-03-08
description: Hướng dẫn ngắn gọn để thiết lập KaTeX
math: true
---

Công thức toán học trong một dự án Hugo có thể được bật lên bằng cách sử dụng các thư viện JavaScript của bên thứ ba.

<!--more-->

Trong ví dụ này, chúng ta sẽ sử dụng [KaTeX](https://katex.org/)

- Tạo một partial dưới `/layouts/partials/math.html`
- Trong partial này, tham chiếu đến [Tiện ích Tự động render](https://katex.org/docs/autorender.html) hoặc tải các tập tin script này về máy.
- Bao gồm partial trong các mẫu của bạn như sau:

```bash
{{ if or .Params.math .Site.Params.math }}
{{ partial "math.html" . }}
{{ end }}


- To enable KaTex globally set the parameter `math` to `true` in a project's configuration
- To enable KaTex on a per page basis include the parameter `math: true` in content files

**Note:** Use the online reference of [Supported TeX Functions](https://katex.org/docs/supported.html)

{{< math.inline >}}
{{ if or .Page.Params.math .Site.Params.math }}

<!-- KaTeX -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.css" integrity="sha384-zB1R0rpPzHqg7Kpt0Aljp8JPLqbXI3bhnPWROx27a9N0Ll6ZP/+DiW/UqRcLbRjq" crossorigin="anonymous">
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.js" integrity="sha384-y23I5Q6l+B6vatafAwxRu/0oK/79VlbSz7Q9aiSZUvyWYIYsd+qj+o24G5ZU2zJz" crossorigin="anonymous"></script>
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/contrib/auto-render.min.js" integrity="sha384-kWPLUVMOks5AQFrykwIup5lo0m3iMkkHrD0uJ4H5cjeGihAutqP0yW0J6dpFiVkI" crossorigin="anonymous" onload="renderMathInElement(document.body);"></script>
{{ end }}
{{</ math.inline >}}

### Examples

Inline math: \\(\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…\\)

Block math:

$$
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } }
$$
