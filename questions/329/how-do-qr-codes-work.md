## How do QR codes work?

- posted by: [Moshe](https://stackexchange.com/users/-1/165-moshe) on 2011-04-21
- tagged: `encoding`, `barcode`
- score: 5

I understand the basics of how barcodes work, but what is the layout and format of a QR code, and how do QR code readers understand the data? (Compared to the liner, binary format of a bar code.)


## Answer 332

- posted by: [Pearsonartphoto](https://stackexchange.com/users/-1/67-pearsonartphoto) on 2011-04-22
- score: 7

<p>QR codes are organized as follows:</p>

<p><img src="http://i.imgur.com/oGI5I.png" alt="QR code explanation, is licensed under Creative Common"> (<a href="http://en.wikipedia.org/wiki/File%3aQR_Code_Structure_Example.svg" rel="nofollow">Original image from Wikipedia</a>)</p>

<p>Note that the main boxes help with the alignment, as well as one smaller box contained in the image. Bar codes contain similar mechanisms to help with alignment. The smaller box helps to know the orientation. Similarly, there are two additional lines within the image which will guide one to each line of data.</p>

<p>So, a scanner application will simply use the alignment guides to realize the size and orientation of the code, and will proceed to read the data, one byte at a time. </p>




---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
