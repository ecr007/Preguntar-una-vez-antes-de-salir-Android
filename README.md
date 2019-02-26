# Preguntar-una-vez-antes-de-salir-Android

```java
@Override
public void onBackPressed() {
    new AlertDialog.Builder(this)
        .setTitle("Really Exit?")
        .setMessage("Are you sure you want to exit?")
        .setNegativeButton(android.R.string.no, null)
        .setPositiveButton(android.R.string.yes, new OnClickListener() {

            public void onClick(DialogInterface arg0, int arg1) {
                WelcomeActivity.super.onBackPressed();
            }
        }).create().show();
}
```
