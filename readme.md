## 一、添加滚动试图和活动Web链接

### 1.1为活动网页链接添加自动链接属性

将属性添加到 .此的 XML 代码现在如下所示：`android:autoLink="web"`

```xml
<TextView
    android:id="@+id/article"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:autoLink="web"
    android:lineSpacingExtra="5sp"
    android:padding="@dimen/padding_regular"
    android:text="@string/article_text" />
```
### 1.2向布局添加滚动视图
若要使用滚动视图，则需要使用ScrollView，如下所示：
```xml
<ScrollView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:layout_below="@id/article_heading">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical">

        <TextView
            android:id="@+id/article_subheading"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:padding="@dimen/padding_regular"
            android:text="I am the article subtitle"
            android:textAppearance=
                "@android:style/TextAppearance.DeviceDefault" />

        <TextView
            android:id="@+id/article"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:autoLink="web"
            android:lineSpacingExtra="5sp"
            android:padding="@dimen/padding_regular"
            android:text="@string/article_text" />
    </LinearLayout>

</ScrollView>
```

