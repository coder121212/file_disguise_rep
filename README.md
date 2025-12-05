# file_disguise_rep
🎭 Mask a file with another file, written in Python3 🐍

🚀 HOW TO USE IT: 🗃️
Firstly, you prodive location of the "mask" file you want to use, I recommend an .jpg image or a .lnk shortcut because it would be easier to blend them in between other files on your desktop.
Secondly, you provide location of the file you want to hide, I recommend a .zip file.
And for the last, enter the name of the output file. Make sure to include the extention as well. Output file will be placed in the same directory as the executable unless you enter an absolute address.

⚠️ WARNING: ⚠️
If there is already a file at the output destination with the same name and extention, it will get overridden!
I don't take any responsibility for corrupted or lost files.

📖🔍 HOW IT WORKS: 🔎📖
Reads the input files in binary and writes them onto the same file. I recommend using .jpg as the mask file and .zip as the hidden file, but in theory you can use any file extentions. Because the jpg image is written first, your operating system sees the "jpg file starts here" header and thinks it is an ordinary image file. zip file data after "jpg file ends here" header is ignored by your photo viewer app. Instead, you can right click the file and select open with another app option and choose your prefered file compresser app -like WinRAR or 7z-. 7z works with compressed archive files so it thinks jpg file information at the start are junk data and skips reading them, starts from "zip file starts here" header.

A person who is not aware of your mischievous intentions will not think about opening that jpg image with a file compressor.

One small problem, however, is that your operating system calculates the file size correctly. An jpg file with 10GB size would raise suspicion. You should dilute your files into various images, if you are seriously considering using this app.

