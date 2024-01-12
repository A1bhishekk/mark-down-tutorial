                        # Markdown Cheatsheet

<!-- heading  -->
# heading 1
I am heading 1

## heading 2
I am heading 2

### heading 3
I am heading 3


---

<!-- italic  -->

*Abhishek*

<!-- bold  -->

**Abhi**

<!-- bold and italic -->

**_bold and italic_**

<!-- quote  -->

> This is blockquote 


<!-- list -->

1. This is a **list**
   1. This is a sub list
   2. This is a sub list
   3. This is a sub list
2. This is a list 
3. This is a list 

- This is unordered list 
  - This is unordered list
  - This is unordered list
  - This is unordered list
- This is unordered list 
- This is unordered list 

<!-- code -->
`console.log("hello World)`

<!-- multi line code  -->
```javascript
export const getAnylytics = async (req, res) => {
    const shortId = req.params.shortId;

    const url = await Url.findOne({ shortId: shortId })

    if (!url) {
        return res.status(404).json({
            success: false,
            message: 'Url not found',
        })
    }

    res.status(200).json({
        success: true,
        message: 'Url analytics',
        totalClicks: url.visitHistory.length,
        redirectUrl: url.redirectUrl,
        visitHistory: url.visitHistory,
    })
};

```

<!-- link  --> 
i am link : 
[youtube](https://www.youtube.com/watch?v=ts7oLiVqwb0)

<!-- image -->

![alt text](https://cdn.hashnode.com/res/hashnode/image/upload/v1612447830875/69Dlr3tjZ.png?w=1600&h=840&fit=crop&crop=entropy&auto=compress,format&format=webp)



- [x] this is a task
- [ ] this is a task

h~2~O

<!-- table -->

| Name | Email | Mobile |
| --- | --- | --- |
| Abhishek | abhi@gmail.com | 1234567890 |
| Abhishek | abhi@gmail.com | 1234567890 |
| Abhishek | abhi@gmail.com | 1234567890 |
| Abhishek | abhi@gmail.com | 1234567890 |
| Abhishek | abhi@gmail.com | 1234567890 |


~~Strikethrough~~

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

Here's a sentence with a footnote. [^2]
[^2]: This is the footnote.

That is so funny! :joy:

I need to highlight these ==very important words==.


<!-- superscript:  -->
X^2^ + Y^2^ = Z^2^
