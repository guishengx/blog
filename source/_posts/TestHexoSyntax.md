title: 测试英文文件名，中文标题，则可url为英文
date: 2015-03-09 16:01:41
tags:
---
# 这是一级标题


```c++
printf("FUNC:%s", __function__);
```

##二级标题

**这是粗体**

```
- (void)setMessageFrame:(MessageFrame *)messageFrame
{
    _messageFrame = messageFrame;
    Message *msg = messageFrame.message;

    //
    NSString *iconName = (msg.type == MessageTypeMe) ? @"me" : @"other";
    
    self.iconView.image = [UIImage imageNamed:iconName];
    self.iconView.frame = messageFrame.iconF;
    
    self.timeView.text = msg.time;
    self.timeView.frame = messageFrame.timeF;
    
    [self.textView setTitle:msg.text forState:UIControlStateNormal];
    
    
    self.textView.backgroundColor = [UIColor redColor];
    if (msg.type == MessageTypeMe) {
        [self.textView setBackgroundImage:[UIImage imageNamed:@"chat_send_nor"] forState:UIControlStateNormal];
    }else{
        [self.textView setBackgroundImage:[UIImage imageNamed:@"chat_recive_nor"] forState:UIControlStateNormal];
    }
    self.textView.frame = messageFrame.textF;
    
}

```