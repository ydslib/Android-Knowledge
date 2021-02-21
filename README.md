# Android-Knowledge
Android知识梳理，知识问答

# [消息](https://github.com/ydslib/Android-Knowledge/wiki#%E6%B6%88%E6%81%AF)
>- [消息机制](https://github.com/ydslib/Android-Knowledge/wiki#1-%E6%B6%88%E6%81%AF%E6%9C%BA%E5%88%B6)
> 
>- [sendMessage和post(Runnable)的区别？](https://github.com/ydslib/Android-Knowledge/wiki#2-sendmessage%E5%92%8Cpostrunnable%E7%9A%84%E5%8C%BA%E5%88%AB)
> 
>- [子线程中维护的looper，消息队列无消息时候的处理节省性能的处理方案](https://github.com/ydslib/Android-Knowledge/wiki#3-%E5%AD%90%E7%BA%BF%E7%A8%8B%E4%B8%AD%E7%BB%B4%E6%8A%A4%E7%9A%84looper%E6%B6%88%E6%81%AF%E9%98%9F%E5%88%97%E6%97%A0%E6%B6%88%E6%81%AF%E6%97%B6%E5%80%99%E7%9A%84%E5%A4%84%E7%90%86%E8%8A%82%E7%9C%81%E6%80%A7%E8%83%BD%E7%9A%84%E5%A4%84%E7%90%86%E6%96%B9%E6%A1%88)
>
>- [Handler中的loop方法为什么不会导致线程卡死？](https://github.com/ydslib/Android-Knowledge/wiki#4-handler%E4%B8%AD%E7%9A%84loop%E6%96%B9%E6%B3%95%E4%B8%BA%E4%BB%80%E4%B9%88%E4%B8%8D%E4%BC%9A%E5%AF%BC%E8%87%B4%E7%BA%BF%E7%A8%8B%E5%8D%A1%E6%AD%BB)

# [渲染](https://github.com/ydslib/Android-Knowledge/wiki#%E6%B8%B2%E6%9F%93)
>
>- [渲染机制](https://github.com/ydslib/Android-Knowledge/wiki#1-%E6%B8%B2%E6%9F%93%E6%9C%BA%E5%88%B6)
# [屏幕刷新](https://github.com/ydslib/Android-Knowledge/wiki#2-%E5%B1%8F%E5%B9%95%E5%88%B7%E6%96%B0)
>- [16.6ms刷新一次屏幕是什么意思？是指没隔16.6ms调用一次onDraw么？](https://github.com/ydslib/Android-Knowledge/wiki#21-166ms%E5%88%B7%E6%96%B0%E4%B8%80%E6%AC%A1%E5%B1%8F%E5%B9%95%E6%98%AF%E4%BB%80%E4%B9%88%E6%84%8F%E6%80%9D%E6%98%AF%E6%8C%87%E6%B2%A1%E9%9A%94166ms%E8%B0%83%E7%94%A8%E4%B8%80%E6%AC%A1ondraw%E4%B9%88)
>
>- [如果界面一直保持不变的话，那么还会没隔16.6ms刷新一次屏幕么？](https://github.com/ydslib/Android-Knowledge/wiki#22-%E5%A6%82%E6%9E%9C%E7%95%8C%E9%9D%A2%E4%B8%80%E7%9B%B4%E4%BF%9D%E6%8C%81%E4%B8%8D%E5%8F%98%E7%9A%84%E8%AF%9D%E9%82%A3%E4%B9%88%E8%BF%98%E4%BC%9A%E6%B2%A1%E9%9A%94166ms%E5%88%B7%E6%96%B0%E4%B8%80%E6%AC%A1%E5%B1%8F%E5%B9%95%E4%B9%88)
>
>- [界面的显示其实就是一个Activity的View树里所有的View都进行测量、布局、绘制操作之后的结果呈现，那么如果这部分工作都完成后，屏幕会马上就刷新么？](https://github.com/ydslib/Android-Knowledge/wiki#23-%E7%95%8C%E9%9D%A2%E7%9A%84%E6%98%BE%E7%A4%BA%E5%85%B6%E5%AE%9E%E5%B0%B1%E6%98%AF%E4%B8%80%E4%B8%AAactivity%E7%9A%84view%E6%A0%91%E9%87%8C%E6%89%80%E6%9C%89%E7%9A%84view%E9%83%BD%E8%BF%9B%E8%A1%8C%E6%B5%8B%E9%87%8F%E5%B8%83%E5%B1%80%E7%BB%98%E5%88%B6%E6%93%8D%E4%BD%9C%E4%B9%8B%E5%90%8E%E7%9A%84%E7%BB%93%E6%9E%9C%E5%91%88%E7%8E%B0%E9%82%A3%E4%B9%88%E5%A6%82%E6%9E%9C%E8%BF%99%E9%83%A8%E5%88%86%E5%B7%A5%E4%BD%9C%E9%83%BD%E5%AE%8C%E6%88%90%E5%90%8E%E5%B1%8F%E5%B9%95%E4%BC%9A%E9%A9%AC%E4%B8%8A%E5%B0%B1%E5%88%B7%E6%96%B0%E4%B9%88)
>
>- [主线程耗时的操作会导致丢帧，那么耗时操作为什么会导致丢帧？它是如果导致丢帧的？](https://github.com/ydslib/Android-Knowledge/wiki#24-%E4%B8%BB%E7%BA%BF%E7%A8%8B%E8%80%97%E6%97%B6%E7%9A%84%E6%93%8D%E4%BD%9C%E4%BC%9A%E5%AF%BC%E8%87%B4%E4%B8%A2%E5%B8%A7%E9%82%A3%E4%B9%88%E8%80%97%E6%97%B6%E6%93%8D%E4%BD%9C%E4%B8%BA%E4%BB%80%E4%B9%88%E4%BC%9A%E5%AF%BC%E8%87%B4%E4%B8%A2%E5%B8%A7%E5%AE%83%E6%98%AF%E5%A6%82%E6%9E%9C%E5%AF%BC%E8%87%B4%E4%B8%A2%E5%B8%A7%E7%9A%84)
>
>- [DecorView与ViewRootImpl什么时候关联在一起的？](https://github.com/ydslib/Android-Knowledge/wiki#25-decorview%E4%B8%8Eviewrootimpl%E4%BB%80%E4%B9%88%E6%97%B6%E5%80%99%E5%85%B3%E8%81%94%E5%9C%A8%E4%B8%80%E8%B5%B7%E7%9A%84)
>
>- [为什么在Activity到onCreate，onStart，onResume里获取不到View到宽高？](https://github.com/ydslib/Android-Knowledge/wiki#26-%E4%B8%BA%E4%BB%80%E4%B9%88%E5%9C%A8activity%E5%88%B0oncreateonstartonresume%E9%87%8C%E8%8E%B7%E5%8F%96%E4%B8%8D%E5%88%B0view%E5%88%B0%E5%AE%BD%E9%AB%98)

# [优化](https://github.com/ydslib/Android-Knowledge/wiki#%E4%BC%98%E5%8C%96)
>- [卡顿原理](https://github.com/ydslib/Android-Knowledge/wiki#1-%E5%8D%A1%E9%A1%BF%E5%8E%9F%E7%90%86)
>
>- [OOM](https://github.com/ydslib/Android-Knowledge/wiki#3-oom)
>
>- [内存泄漏](https://github.com/ydslib/Android-Knowledge/wiki#4-%E5%86%85%E5%AD%98%E6%B3%84%E6%BC%8F)
>
>- [ANR](https://github.com/ydslib/Android-Knowledge/wiki#5-anr)
# [GC](https://github.com/ydslib/Android-Knowledge/wiki#2-gc)
>- [GC原理](https://github.com/ydslib/Android-Knowledge/wiki#1-gc%E5%8E%9F%E7%90%86)
>
>- [对象存活判断](https://github.com/ydslib/Android-Knowledge/wiki#2-%E5%AF%B9%E8%B1%A1%E5%AD%98%E6%B4%BB%E5%88%A4%E6%96%AD)
>
>- [GC root包括哪些？](https://github.com/ydslib/Android-Knowledge/wiki#3-gc-root%E5%8C%85%E6%8B%AC%E5%93%AA%E4%BA%9B)
>
>- 
>- [垃圾回收算法有哪些？](https://github.com/ydslib/Android-Knowledge/wiki#4-%E5%9E%83%E5%9C%BE%E5%9B%9E%E6%94%B6%E7%AE%97%E6%B3%95%E6%9C%89%E5%93%AA%E4%BA%9B)
>
# [View的绘制](https://github.com/ydslib/Android-Knowledge/wiki#view%E7%9A%84%E7%BB%98%E5%88%B6)
>- [View的绘制从哪里开始的，以及过程？](https://github.com/ydslib/Android-Knowledge/wiki#1-view%E7%9A%84%E7%BB%98%E5%88%B6%E4%BB%8E%E5%93%AA%E9%87%8C%E5%BC%80%E5%A7%8B%E7%9A%84%E4%BB%A5%E5%8F%8A%E8%BF%87%E7%A8%8B)
>
>- [自定义控件有哪几种方式？](https://github.com/ydslib/Android-Knowledge/wiki#2-%E8%87%AA%E5%AE%9A%E4%B9%89%E6%8E%A7%E4%BB%B6%E6%9C%89%E5%93%AA%E5%87%A0%E7%A7%8D%E6%96%B9%E5%BC%8F)
>
# [事件](https://github.com/ydslib/Android-Knowledge/wiki#%E4%BA%8B%E4%BB%B6)
>- 
>
#[Binder](https://github.com/ydslib/Android-Knowledge/wiki#binder)
>- [Binder跨进程通信原理](https://github.com/ydslib/Android-Knowledge/wiki#1-binder%E8%B7%A8%E8%BF%9B%E7%A8%8B%E9%80%9A%E4%BF%A1%E5%8E%9F%E7%90%86)
>
>- [AIDL生成的java类的类结构是怎么样的？](https://github.com/ydslib/Android-Knowledge/wiki#2-aidl%E7%94%9F%E6%88%90%E7%9A%84java%E7%B1%BB%E7%9A%84%E7%B1%BB%E7%BB%93%E6%9E%84%E6%98%AF%E6%80%8E%E4%B9%88%E6%A0%B7%E7%9A%84)
>
>- [Binder的优势是什么？](https://github.com/ydslib/Android-Knowledge/wiki#3-binder%E7%9A%84%E4%BC%98%E5%8A%BF%E6%98%AF%E4%BB%80%E4%B9%88)
>
# [并发](https://github.com/ydslib/Android-Knowledge/wiki#%E5%B9%B6%E5%8F%91)

