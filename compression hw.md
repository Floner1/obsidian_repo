**WHY COMPRESS DATA (syllabus 1.3)**

- Reduces file size for storage and for transmission
- Matters most where storage space or bandwidth is limited
- Real uses: sending multiple files by email, uploading and downloading to servers, streaming video and audio, getting past file-type blocks on email attachments

**WHAT A COMPRESSION ALGORITHM IS**  
A compression technique is an algorithm, a defined sequence of steps, that reduces the number of bits needed to represent a file.

- Compression: original file in, compressed file out
- Decompression: compressed file in, usable file out, identical to the original only if the method is lossless
- Compression changes the data but not the file's core properties, a compressed 10 minute song is still 10 minutes long, a compressed bitmap keeps its resolution
- Compression is usually automatic, you don't choose it, your phone just saves photos as JPEG

**LOSSY VS LOSSLESS (syllabus 1.3, core requirement)**

Lossy

- Data is permanently removed during compression
- Decompressed file is an approximation, not identical to the original
- Works because the human eye or ear can't detect the missing detail
- Called a destructive process, the original data can never be fully recovered
- Used for: MP3 (audio), JPEG (photographs), MPEG-1 (small low-res video), MPEG-2 (full-screen high-res video)
- Risk: repeated rounds of lossy compression stack up loss, the file can become unrecognisable
- Never use on text or numeric data, you can't approximate a word or a number, "fos" could decompress as floss, frogs, or fools (fifteen possible words fit)

Lossless

- No data lost, decompressed file is identical to the original
- Used for: PNG (high quality images), GIF (images and short animations), ZIP (bundling and compressing files)
- Required wherever exact accuracy matters, documents, code, assignments, numeric data

Justifying a choice in an exam answer

- Pick lossy when the file is image, audio, or video, minor quality loss is acceptable, and small size matters more (streaming, web, email)
- Pick lossless when the file is text or numeric, exact accuracy is required, or the file will be edited and recompressed repeatedly (avoids generation loss)

**RUN-LENGTH ENCODING, RLE (syllabus 1.3, named technique, know this in detail)**

- Lossless
- Finds runs of repeated values and replaces each run with one instance of the value plus a count
- Data is stored as pairs: pattern, then count
- Well suited to images with small colour palettes and blocks of solid colour, cartoons, line art, logos
- Badly suited to photographs, continuous colour variation means few repeated runs, RLE can make the file bigger, not smaller
- Rule: the number of bits used for the count must be large enough to hold the biggest possible run

Worked example, from your source, 28x28 image, 5 colours

- 5 colours needs a 3-bit colour code (2^3 = 8, covers it)
- Uncompressed row of 28 pixels: 28 x 3 = 84 bits
- Compressed row uses colour+count pairs, 48 bits total, well under 84
- Row breakdown: white x4, blue x2, white x4, pink x7, blue x2, white x9, six runs total, each pair is 3-bit colour + 5-bit count = 8 bits, 6 x 8 = 48 bits, confirmed

Practice example, 4x4 black/white image, 1-bit colour code, 3-bit count

- Last row given as answer: 1 1 1 1, RLE is "1 100" (colour 1 = white, count 100 binary = 4)
- First row is 0 0 0 1, that's a run of 3 blacks then 1 white
- Answer: 0 011 1 001 (colour 0, count 011 = 3, then colour 1, count 001 = 1)

**DICTIONARY-BASED COMPRESSION (syllabus 1.3, text file example)**

- Lossless
- Finds repeated patterns, usually words, patterns don't need to be adjacent, unlike RLE
- Each unique word gets a short code, the code is stored instead of the full word
- A dictionary (code list) is stored too, so decompression can substitute codes back for words
- Number of code bits depends on the number of unique words, worked example: 36 unique words needs 6 bits (2^6 = 64 is enough, 2^5 = 32 is not)
- Big savings on long or frequently repeated words, an 8-letter word at 128 bits in Unicode (8 characters x 16 bits) can become a single 6-bit code
- Fully lossless, original text is recreated exactly

**JPEG (syllabus 1.3, bitmap image example, lossy)**

- Discards imperceptible colour detail per pixel block

**MP3 (syllabus 1.3, sound file example, lossy)**

- Discards inaudible frequencies

**ZIP (syllabus 1.3, general file compression, lossless)**

- Bundles one or more files or folders into a single compressed file
- Sends multiple files in one email
- Gets around email providers blocking certain file types, like .exe, as harmful content, since zipping changes the apparent file type
- Useful for uploading and downloading to servers, especially ones that auto-unzip on receipt

**MEASURING COMPRESSION (syllabus 1.3, evaluating a method)**

Compression ratio

- Ratio of original size to compressed size
- Written as whole numbers, colon or fraction form, eg 1:5
- Example: 8GB original, 2GB compressed, expressed as 2:8, simplified to 1:4

Saving percentage

- Percentage of space saved
- Example: 25GB original, 16.25GB compressed, compressed file is 65% of the original, saving percentage is 35%

**CHOOSING A COMPRESSION METHOD (syllabus 1.3, justification skill)**

- Balance space saved against time taken to compress and decompress
- Storage or bandwidth-limited systems prioritise smaller size
- Performance-critical systems, video streaming for example, sometimes need specialist hardware to decompress fast enough, or you get lag
- Lag might be tolerable watching something at home, not acceptable in a commercial setting