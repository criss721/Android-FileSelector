# Android FileSelector


# How To Use : 

```java
new FileSelector(this, new String[]{FileSelector.XLS, FileSelector.XLSX}).selectFile(new FileSelector.OnSelectListener() {
      @Override
      public void onSelect(String path) {
        G.toast(path);
      }
    });

new FileSelector(this, new String[]{".jpg", ".jpeg"}).selectFile(new FileSelector.OnSelectListener() {
      @Override
      public void onSelect(String path) {
        G.toast(path);
      }
    });

findViewById(android.R.id.content).setOnClickListener(new View.OnClickListener() {
      @Override
      public void onClick(View v) {
        new FileSelector(ActivitySplash.this, new String[]{FileSelector.PNG}).selectFile(new FileSelector.OnSelectListener() {
          @Override
          public void onSelect(String path) {
            G.toast(path);
          }
        });
      }
    });
```

![intro](media.jpg)
