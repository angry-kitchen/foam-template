# Arn

systrace

```
/Users/admin/Library/Android/sdk/platform-tools/systrace

python /Users/admin/Library/Android/sdk/platform-tools/systrace/systrace.py -o mynewtrace.html -a com.hunantv.imgo.activity sched

/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome mynewtrace.html
```

TraceView

```
Debug.startMethodTracing("trace_card_fragment");

Debug.stopMethodTracing();
```

Android 函数耗时统计工具之Hugo
