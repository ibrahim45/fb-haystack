# Objective
 * Application metadata describes the information needed to con- struct a URL that a browser can use to retrieve a photo.

 * Filesystem metadata identifies the data necessary for a host to retrieve the photos that reside on that host’s disk.

# Implementation
    1. Haystack Directory
    2. Haystack Cache
    3. haystack Storage

# Needle Info
    Header - Magic number used for recovery
    Cookie - Random number to mitigate brute force lookups
    Key    - 64-bit photo id
    Alternate key - 32-bit supplemental id
    Flags - Signifies deleted status
    Size - Data size
    Data - The actual photo data
    Footer - Magic number for recovery
    Data Checksum - Used to check integrity
    Padding - Total needle size is aligned to 8 ßytes

# Application Url
 ```
 http://⟨CDN⟩/⟨Cache⟩/⟨Machine id⟩/⟨Logical volume, Photo⟩
 ```


# Results
    . Graphs
    . Network Analysis