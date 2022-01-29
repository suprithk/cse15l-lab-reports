# Bug 1 - File with Image

This [failure-inducing input](https://github.com/suprithk/markdown-parse/blob/51f10558fe3f0544eab268874062085a955e7298/image.md) file had an image link along with a website link. The algorithm didn't have a mechanism to differentiate between the two as they both have very similar formats. The symptom was the output of the list `[google.com, fake.png]`. The following code change screenshot shows the changes made that detects a `!` so that an image link isn't incorrectly included in the list of links.

![Image](report-2.1.png)

# Bug 2 - File with Incorrect Format 





# Bug 3 - File with 