---
title: enums / privateEnum
category: Pipe
order: 1
---

枚举转换，如果使用 `enums` 则枚举文件为 `@global/enums.ts`，如下：

{% highlight html %}
\{{val | enums: 'company'}}
{% endhighlight %}

<br>

如果使用 `privateEnum` 则可自定义枚举，如下：

{% highlight html %}
\{{emnuText | privateEnum: enums}}
{% endhighlight %}

{% highlight typescript %}
emnuText: string = 'a'

enums: object = {
  a: '1',
  b: 2
}
{% endhighlight %}
