# Filenames and LaTeX and Pandoc, Oh My!

*This [blog post][1] originally appeared on the* ProfHacker *blog at the* Chronicle of Higher Education *on November 17, 2016.*

![][image-1]

Sometimes it happens: someone sends us a document in Word format, and we’d really rather it was a PDF. The reasons can vary. Maybe we need to post it on a website, and we’d rather users be able to view it in a browser, rather than being forced to download it. Maybe it’s an essay we need to grade, and, [like Erin][2], we want to use iAnnotate or a similar application for that purpose.

When there are only a few documents involved, converting the files to PDF is simple enough; all that’s necessary is to open the file in a word processor that’s capable of reading it, then save or export it in PDF format.

That’s pretty tedious if there are a lot of files that need converting, though. A couple of years ago Natalie explained [how to batch convert documents using Google Drive][3], but as she noted, the standard version of Google Drive[^1] might not be the best solution for sensitive documents.

There *is* a way that avoids cloud-based services. The initial setup doesn’t take very long — I think I had it all done in less than half an hour, and part of that time was spent Googling how to install “rename” on the Mac. If you frequently need to convert large numbers of files from Word to PDF format, it’s well worth the time it takes, especially since it’s only necessary to do the setup once.

I stumbled across this method when, having forgotten about Natalie’s above-mentioned post, I Googled how to batch convert Word documents to PDF format on a Mac. That search led me to this very helpful post by Clark R. Donley: “Bulk convert student papers from .docx to consistently formatted .pdf files with pandoc.”[^2] (Longtime readers may well recall [Lincoln’s post about pandoc and its benefits][4].)

Using Mr. Donley’s post as a guide, I did the following on my Mac:

1. Installed [Homebrew][5]. I did this so I could easily install “rename,” which I couldn’t find on my Mac.
2. Installed “rename.” Once I’d installed Homebrew, this was easy to do: I just typed “brew install rename” at the command prompt, and hit the enter key. (The time it took to figure out how to install Homebrew and “rename” is included in my half-hour estimate.)
3. Installed [Pandoc][6].
4. Installed a LaTeX package. Since I’m on a Mac, I followed the suggestion on the Pandoc site and installed [BasicTeX][7]. (For the kind of batch conversion described here, it’s not necessary to have any familiarity with LaTeX. It just needs to be installed so that Pandoc can do its thing.)
5. Opened a terminal window, navigated to the directory where my files were, and ran “rename” to change spaces in the filenames to underscores, using a wildcard character so all .docx files in the directory would be renamed. (This step isn’t necessary if the file names don’t contain spaces.)
6. Told Pandoc to convert every .docx file it found in the directory to .pdf format. (You can see both the rename and conversion commands in the lead image. I didn’t need the formatting options that Mr. Donley did, so I eliminated parts of the conversion command that you see in his post.)

The conversion process was surprisingly quick. I also tested the process on a Linux machine (where I installed [TeX Live][8] instead of BasicTeX), and can confirm that this process works just as well in Linux. “Rename” was already present in my Linux distribution (Ubuntu 16.04), so I didn’t need to install that.

I didn’t try the process in Windows. Pandoc works in Windows, though, so I expect a similar setup is possible.

***Do you have a favorite way to batch convert files from one format to another? Or, perhaps, suggestions for improving this process? Let us know in the comments.***

*[CC-licensed image by the author.]()*

[^1]:	Google’s privacy policy for Google Apps for Education differs from its policy for the standard version.

[^2]:	Unfortunately, a check on 2/28/2021 showed that this post is no longer available on Dr. Donley’s site.

[1]:	http://www.chronicle.com/blogs/profhacker/filenames-and-latex-and-pandoc-oh-my/63169
[2]:	http://www.chronicle.com.stproxy.palni.edu/blogs/profhacker/using-iannotate-as-a-grading-tool/53981
[3]:	http://www.chronicle.com/blogs/profhacker/batch-convert-word-documents-to-pdf-in-google-drive/58491
[4]:	http://www.chronicle.com/blogs/profhacker/pandoc-converts-all-your-text-documents/38700
[5]:	http://brew.sh/
[6]:	http://pandoc.org/
[7]:	http://www.tug.org/mactex/morepackages.html
[8]:	http://www.tug.org/texlive/


[image-1]:	# "Screen shot of a terminal window"