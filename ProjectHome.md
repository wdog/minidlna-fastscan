"FastScan" is MiniDLNA fork (see http://sourceforge.net/projects/minidlna/) that is able to scan once processed drives much faster(external HDDs, USB sticks, etc.)

I use my raspberry pi as media server based on MiniDLNA. It rather annoying to wait while your mega-terrabyte external HDD being scanned each time you plug it. The "FastScan" fork solves this issue by speeding up rescan process. It creates files with meta-information on the drive. These files could be quickly processed and remain on device after media is removed. When you plug it again meta-files reduce rescan time up to 10x.

This code also includes sort fix for Panasonic TVs and force files to be sorted by name.

Compile instructions:

1. git clone https://code.google.com/p/minidlna-fastscan/

2. cd minidlna-fastscan/

3. ./configure

4. make