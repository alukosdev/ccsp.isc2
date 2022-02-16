# Storage Architectures

## Overview

| IaaS | PaaS | SaaS |
| :--- | :--- | :--- |
| Volume Storage | Structured Storage | Information Storage and Management \(long-term\) |
| Object Storage | Unstructured Storage | Content and File Storage \(long-term\) |
|  |  | Raw Storage |
|  |  | Ephemeral Storage |
|  |  | CDN |

:::info
If storage is accessible via API, then it's considered PaaS.
:::

## Storage Architectures

### Volume Storage

With volume storage, the customer is allocated a storage space within the cloud; this storage space is represented as an attached drive to the user's virtual machine. From the customer's perspective, the virtual drives performs very much in the same manner as would a physical drive attached to a tangible device.

Volume storage contains two subset storage types:

- File Storage
- Block Storage

#### File Storage

With file storage, the data is stored and displayed just as with a file structure in the legacy environment \(as files and folders\), with all the same hierarchical naming functions.

Features of file storage include:

- File sharing
- Local archiving
- Data protection

File storage is commonly implemented in:

- Big data analytical tools and processes
- NAS

#### Block Storage

Block storage is a blank volume that the customer or user can put anything into.

Features of block storage include:

- Flexibility
- Performance

Challenges of block storage include:

- Requires greater administration
- May require OS or application to store, sort, and retrieve data

Use cases for block storage include:

- Data of multiple types and kinds, such as enterprise backup services

Common implementations of block storage include:

- iSCSI
- SAN
- RAID
- VMFS
- Email servers \(such as Microsoft Exchange\)

### Object Storage

This type of cloud storage arrangement involves the use of associating metadata with the saved data. Data objects \(files\) are saved in the storage space along with relevant metadata such as content type and creation date. Data is stored as objects, not as files or blocks. Objects include the content, metadata describing the content and object, and a unique address identifier for locating that object.

An object storage system typically comes with minimal features. It gives the ability to store, copy, retrieve, and delete files and also gives authority to control which user can perform these actions. If you want to be able to search or have an object metadata central repository for other apps to draw on, you have to do it by yourself. Many storage systems such as Amazon S3 provide REST APIs and web interfaces to allow programmers to work with objects and containers.

Challenges of object storage include:

- Write-once, read many \(WORM\) makes object storage unsuitable for databases.
- Replication is not complete until all versions have been synchronized, which takes time. This makes object storage unsuitable for data that constantly changes, but a good solution for stagnant data.

Use cases for object storage include:

- When significant levels of description are required, including marking, labels, and classification and categorization.
- When data requires indexing capabilities.
- When data requires data policy enforcement \(such as IRM/DRM or DLP\).
- Centralization of some data management functions.
- Unstructured data such as music, images, and videos.
- Backup and log files.
- Large sets of historical data.
- Archived files.
- Big data endeavors.

Common implementations of object storage include:

- Amazon S3
- CDNs

Security for object storage can be provided by using:

- *IRM/DRM \(file-level or file-based encryption\).* Protects against *hardware* theft. Any process or user that has access to the OS still has access to the data.

### Structured Storage

Structured storage includes information with a high degree of organization, such that inclusion in a relational database is seamless and readily searchable by simple, straightforward search engine algorithms or other search operations.

#### Databases

Databases are considered structured data. Data will be arranged according to characteristics and elements in the data itself, including a specific trait required to file the data known as the primary key. In the cloud, the database is usually backend storage in the datacenter, accessed by users utilizing online apps or APIs through a browser.

Databases may be installed on object \(undesirable\) or volume storage.

:::info
Databases are most often configured to work with PaaS and SaaS.
:::

### Unstructured Storage

Unstructured storage includes information that does not reside in a traditional row-column database.

#### Examples

- Email messages
- Word processing documents
- Videos
- Photos
- Audio files
- Presentations
- Web pages

Although these sorts of files may have an internal structure, they are still considered unstructured because the data they contain does not fit neatly in a database.

### Information Storage and Management

Data is entered into the system through a web interface and stored within the SaaS application \(usually a back-end database\). This data storage utilizes database, which in turn are installed on object or volume storage.

### Content and File Storage

File-based content is stored within the application and made accessible via the web-based user interface.

### Ephemeral Storage

This type of storage exists only as long as the instance is online. It is typically used for swap files and other temporary storage needs and is terminated with its instance.

### CDN

With a CDN, content is stored in *object* storage, which is then distributed to multiple geographically distributed nodes to improve Internet consumption speed.

A CDN is a form of data caching, usually near geophysical locations of high use demand, for copies of data commonly requested by users.

Use cases for CDNs include:

- Online multimedia streaming services; rather than dragging data from a datacenter to users at variable distances across a continent, the streaming service provider can place copies of the most requested media near metropolitan areas where those requests are likely to be made, thus improving bandwidth and delivery quality.

### Raw Storage

Raw storage or raw device mapping \(RDM\) is an option in the VMware server virtualization environment that enables a storage LUN to be directly connected to a VM from the SAN.