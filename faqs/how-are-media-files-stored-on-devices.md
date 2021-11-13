# How are media files stored on devices?

To keep bandwidth and storage usage low but provide a fast experience, Anytype downloads **Text** and **Images** to your device automatically as they are smaller in size.

Large **Videos** and **Files** are downloaded on demand, i.e., when you click on them, if it is possible to stream them, e.g., a 4k Video, Anytype will stream it directly from the backup node. If it is unable to stream, then Anytype will download the entire file.

To make the experience even better, we have implemented Caching of files, so if you are streaming or frequently using a large file, it will be pre-cached from the server.

{% content-ref url="../reference/storage-and-deletion.md" %}
[storage-and-deletion.md](../reference/storage-and-deletion.md)
{% endcontent-ref %}
