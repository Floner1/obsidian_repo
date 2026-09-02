JPEG compression removes colour details that the human eye cannot see, shrinking the file. MP3 does the same for audio: it discards frequencies beyond the audible range, cutting file size.

ZIP packages multiple files or folders into a single archive. This makes it easier to send several files in one email, and because the archive has a different file type, it can bypass email clients that block certain extensions, such as .exe. It also simplifies uploading and downloading to servers that automatically extract archives.

Lossless compression re‑encodes data so no information is lost, allowing the original file to be fully reconstructed. It’s used when precision matters, such as with PNG images or ZIP archives.

Run‑length encoding (RLE) is a lossless method that replaces long sequences of identical values with the value and a count, storing the data as value‑count pairs. RLE is ideal for images with few colours and large uniform areas, cartoons, line art, logos, where long runs occur. It performs poorly on photographs because colour changes rapidly, and the counter must be large enough to hold the longest run.

Dictionary compression is another lossless technique that replaces repeated patterns, typically words, with short codes. Each distinct word gets a code, and a dictionary of these codes is stored so the original text can be reconstructed. The number of bits required for a code depends on the number of unique words; for example, 36 distinct words need six bits, because 2⁶ = 64 while 2⁵ = 32 is insufficient. This method saves the most on long or frequently repeated words, for example, an eight‑letter word that would normally take 128 bits in Unicode can be represented by a single six‑bit code. No information is lost, and the original text can be recovered exactly.

Compression ratio is expressed as the original size divided by the compressed size, typically in a colon format such as 1:5. For example, compressing an 8‑GB file to 2 GB yields a ratio of 2:8, which simplifies to 1:4.

Saving percentage indicates the proportion of space saved. If a 25‑GB file compresses to 16.25 GB, the compressed file is 65 % of the original, meaning a 35 % reduction.