# Facebook photo growth
![](assets/photo-stored.png)
# Blob hotness and age
![](assets/blob-hotness-and-age.png)
# Haystack: 2008
![](assets/haystack-vs-warm-storage.png)
- High throughput 
    - in memory index
    - single i/o per request
    - multiple copies
    ![](assets/haystack-2013.png)
- Fault tolerance 
    - RAID6
    - Multiple copies
- Central Storage size (RAID6)
    - 2 redundant drivers
    - 2 of 12 = 1.2x replication
# Motivation for warm storage
# F4
![](assets/f4.png)
# Serving user request
- New content written to haystack
- Warm content move to f4
- Read for new content goes to haystack
- Read for warm content goes to f4
![](assets/haystack-upload.png)
![](assets/f4-read.png)
# F4: What it is solving?
![](assets/f4-what-is-solving.png)
# F4: Data splitting
![](assets/f4-data-splitting.png)
# F4: Rebuild
![](assets/f4-rs-rebuild.png)
# F4: Block Placement Policy
![](assets/f4-block-placement.png)
# F4: Cell anatomy
![](assets/f4-cell-anatomy.png)
# F4: Reads
![](assets/f4-cell-1.png)
![](assets/f4-cell-2.png)
# F4: Reads on failure
![](assets/f4-data-center-failure.png)
![](assets/f4-failure-2.png)
![](assets/f4-read-3.png)
# Haystack vs F4
![](assets/h-vs-f4.png)
