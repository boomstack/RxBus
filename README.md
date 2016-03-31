# RxBus
##Simple implementation of eventbus using RxAndroid  
example:
```
RxBus.getDefault().toObserverable(ClickEvent.class).subscribe(new Action1<ClickEvent>() {
            @Override
            public void call(ClickEvent clickEvent) {
                tv.setText("string from rxbus!  click");
            }
        });
        RxBus.getDefault().toObserverable(LongClickEvent.class).subscribe(new Action1<LongClickEvent>() {
            @Override
            public void call(LongClickEvent longClickEvent) {
                tv.setText("string from rxbus!  long click");
            }
        });
```
RxBus is a singleton.
