# TurboCopySearch
In response to a significant challenge, I developed a script to effectively address it. The challenge involved managing a folder containing images, scattered across nested subfolders in what seemed like a chaotic arrangement. The primary goal was to consolidate all these images into a single folder on a Windows system. However, the task presented a formidable obstacle due to the substantial volume—approximately 3 million images—with the primary folder size reaching around 225 GB. This posed a memory challenge during the search and copying process within the Windows environment.

To overcome this hurdle, the current code operates in two distinct steps. Initially, it copies all image paths into chunked text files. Subsequently, it processes these text files to copy the image files, intelligently avoiding direct storage of file names in memory. Instead, the code constructs a generator for more efficient memory usage and utilizes multiprocessing to scale up the operation.
