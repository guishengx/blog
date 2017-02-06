title: HASH之初见
date: 2015-03-06 17:34:12
cotegories: blog
tags:
---
hash算法在高级语言中使用频繁。下面是一段最简单，但不是很好的hash算法，只是为了演示其工作原理。
<!--more-->

```c
static int hash_str(char *key)
{
	int hash = 0;
    char *cur = key;
    while(*(cur++) != '\0') {
        hash += *cur;
    }
    return hash;
}

#define HASH_INDEX(ht, key) (hash_str((key)) % (ht)->size)
```