
WHY COMPRESS DATA (syllabus 1.3)

- Reduces file size for storage and for transmission
- Matters most where storage space or bandwidth is limited
- Real uses: sending multiple files by email, uploading/downloading to servers, streaming video and audio, getting past file-type blocks on email attachments

WHAT A COMPRESSION ALGORITHM IS  
A compression technique is an algorithm, a defined sequence of steps, that reduces the number of bits needed to represent a file.

- Compression: original file in, compressed file out
- Decompression: compressed file in, usable file out (identical to original only if the method is lossless)
- Compression changes the data but not the file's core properties, a compressed 10 minute song is still 10 minutes long, a compressed bitmap keeps its resolution
- Compression is usually automatic, you don't choose it, your phone just saves photos as JPEG

LOSSY VS LOSSLESS (syllabus 1.3, core requirement)

Lossy

- Data is permanently removed during compression
- Decompressed file is an approximation, not identical to the original
- Works because the human eye or ear can't detect the missing detail
- Used for: JPEG (photos), MP3 (audio), MPEG-1 (small low-res video), MPEG-2 (full-screen high-res video)
- Risk: repeated rounds of lossy compression stack up loss, file can become unrecognisable
- Never use on text or numeric data, you can't approximate a word or a number, "fos" could decompress as floss, frogs, or fools

Lossless

- No data lost, decompressed file is identical to the original
- Used for: PNG (high quality images), GIF (images and short animations), ZIP (bundling and compressing files)
- Required wherever exact accuracy matters, documents, code, assignments, numeric data

Justifying a choice in an exam answer

- Pick lossy when the file is image/audio/video, minor quality loss is acceptable, and small size matters more (streaming, web, email)
- Pick lossless when the file is text or numeric, exact accuracy is required, or the file will be edited and recompressed repeatedly (avoids generation loss)

RUN-LENGTH ENCODING, RLE (syllabus 1.3, named technique, know this in detail)

- Lossless
- Finds runs of repeated values and replaces each run with one instance of the value plus a count
- Data is stored as pairs: (pattern, count)
- Well suited to images with small colour palettes and blocks of solid colour, cartoons, line art, logos
- Badly suited to photographs, continuous colour variation means few repeated runs, RLE can make the file bigger, not smaller
- Rule: the number of bits used for the count must be large enough to hold the biggest possible run

Worked example, from your source (28x28 image, 5 colours)

- 5 colours needs a 3-bit colour code (2^3 = 8, covers it)
- Uncompressed row of 28 pixels = 28 x 3 = 84 bits
- Compressed row stores colour+count pairs, 48 bits total in the example, well under 84

Practice example (4x4 black/white image, 1-bit colour code, 3-bit count)

- Last row 1 1 1 1 given as RLE "1 100" (colour 1 = white, count 100 = 4 in binary)
- First row is 0 0 0 1, that's a run of 3 blacks then 1 white
- Answer: 0 011 1 001 (colour 0, count 011 = 3, then colour 1, count 001 = 1)

DICTIONARY-BASED COMPRESSION (syllabus 1.3, text file example)

- Lossless
- Finds repeated patterns (usually words), patterns don't need to be adjacent, unlike RLE
- Each unique word gets a short code, the code is stored instead of the full word
- A dictionary (code list) is stored too, so decompression can substitute codes back for words
- Number of code bits depends on the number of unique words, 36 unique words needs 6 bits (2^6 = 64 is enough, 2^5 = 32 is not)
- Big savings on long or frequently repeated words, an 8-letter word at 128 bits in Unicode can become a single 6-bit code
- Fully lossless, original text is recreated exactly

JPEG (syllabus 1.3, bitmap image example, lossy)

- Exploits the fact that colour changes between neighbouring pixels are often invisible to the eye
- Groups blocks of similar pixels and records one sampled colour for the block, discarding detail the eye won't process
- Standard settings sample one colour per block of 9 pixels, around 90% file size reduction
- On decompression, missing pixels are recreated by approximating from surrounding colours
- Can cause compression artifacts, most visible at sharp colour changes (blurring)
- Compression level is adjustable, trade-off between file size and quality
- Typical compression ratio around 10:1, a 36MB image becomes about 3.6MB

MP3 (syllabus 1.3, sound file example, lossy)

- Exploits limits of human hearing, sounds masked by louder sounds or outside audible range get discarded entirely
- Recreates some missing sound on playback by predicting how real sound behaves
- Typically reduces file size to about 10% of the original (90% reduction)
- Example: 15MB uncompressed becomes roughly 1.5MB
- Resulting sound is not identical to the original, most people won't notice, playback equipment quality also affects perceived loss

SOUND SAMPLING BACKGROUND (syllabus 1.2 Sound, needed to understand MP3 and audio file size)

- Analogue sound must be digitised before a computer can use it, this is analogue to digital conversion, ADC
- Sampling = measuring the analogue wave at regular intervals
- Sampling rate = samples taken per second, in Hz, CD quality standard is 44,100 Hz
- Higher sampling rate = more accurate reconstruction of the sound
- Sample resolution = bits used per sample, more bits = more possible values = more accurate
- 8-bit resolution = lower quality, used where simple sound is fine
- 16-bit resolution = CD and sound card standard, 65,536 possible values
- Stereo doubles the number of samples per second compared to mono

File size formula  
sampling rate x length in seconds x sample resolution = file size in bits (mono, before compression)

Worked example (180 second track, 44,100 Hz, 16-bit, assuming mono since the source doesn't say stereo)

- 44,100 x 180 x 16 = 127,008,000 bits
- Divide by 8 for bytes = 15,876,000 bytes
- Decimal MB (1 MB = 1,000,000 bytes) = 15.876 MB
- Binary MiB (1 MiB = 1,048,576 bytes) = approx 15.14 MiB
- Flag: syllabus 1.1 tests kibi vs kilo, mebi vs mega specifically, check which unit the exam question actually wants before you commit to an answer

ZIP (syllabus 1.3, general file compression, lossless)

- Bundles one or more files or folders into a single compressed file
- Sends multiple files in one email
- Gets around email providers blocking certain file types (eg .exe) as harmful content, since zipping changes the apparent file type
- Useful for uploading/downloading to servers, especially ones that auto-unzip on receipt

MEASURING COMPRESSION (syllabus 1.3, evaluating a method)

Compression ratio

- Ratio of original size to compressed size
- Written as whole numbers, colon or fraction form
- Example: 8GB original, 2GB compressed = 2:8, simplified to 1:4

Saving percentage

- Percentage of space saved
- Example: 25GB original, 16.25GB compressed, compressed file is 65% of original, saving percentage is 35%

CHOOSING A COMPRESSION METHOD (syllabus 1.3, justification skill)

- Balance space saved against time taken to compress and decompress
- Storage/bandwidth-limited systems prioritise smaller size
- Performance-critical systems, video streaming for example, sometimes need specialist hardware to decompress fast enough, otherwise you get lag
- Lag might be tolerable watching something at home, not acceptable in a commercial setting