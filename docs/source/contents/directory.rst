===================
Directory Structure
===================

-------------------
Top-Level Directory
-------------------

The top-level of the oral histories hard drive we receive from Casey looks like this:

.. code-block:: rst
    :name: Top-level Structure
    :caption: Top-level Structure

    20190920_James_Zachary
    20190920_Jensen_Russ
    _20190920_MD5.xlsx
    _20190920_metadata.xlsx
    20190920_Whaley_Seemona-Daniel


Each interview is split into directories and named according to YYYYMMDD_Last_First or YYYYMMDD_Last_First-First:

.. code-block:: rst
    :name: Interview Directories
    :caption: Interview Directories
    :emphasize-lines: 1,2,5

    20190920_James_Zachary
    20190920_Jensen_Russ
    _20190920_MD5.xlsx
    _20190920_metadata.xlsx
    20190920_Whaley_Seemona-Daniel

There are two spreadsheets that describe descriptive metadata and the MD5 Checksums for most files in the corresponding
interview directory.  More information can be found about this here.

.. code-block:: rst
    :name: Checksum and Descriptive Metadata Spreadsheets
    :caption: Checksum and Descriptive Metadata Spreadsheets
    :emphasize-lines: 3,4

    20190920_James_Zachary
    20190920_Jensen_Russ
    _20190920_MD5.xlsx
    _20190920_metadata.xlsx
    20190920_Whaley_Seemona-Daniel


------------------------------
Standard Interview Directories
------------------------------

Most interview directories look like the following:

.. code-block:: rst
    :name: Interview Directory Overview
    :caption: Interview Directory Overview

    ._20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_Clip0005M01.XML
    ._20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary.mkv
    ._20190920_James_Zachary.mp4
    20190920_James_Zachary.mp4
    ._20190920_James_Zachary_release.pdf
    20190920_James_Zachary_release.pdf

The hidden files are unneeded and can be removed:

.. code-block:: rst
    :name: Remove Hidden Files
    :caption: Remove Hidden Files
    :emphasize-lines: 1,4,7,9

    ._20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_Clip0005M01.XML
    ._20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary.mkv
    ._20190920_James_Zachary.mp4
    20190920_James_Zachary.mp4
    ._20190920_James_Zachary_release.pdf
    20190920_James_Zachary_release.pdf

Similarly, the original camera captured files are not needed.  The project team made a decision that we will not keep
these as Casey will generate a preservation file that normalizes the proprietary codec to an open standard.

.. code-block:: rst
    :name: Original Camera Files
    :caption: Original Camera Files
    :emphasize-lines: 2, 3

    20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_Clip0005M01.XML
    20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary.mkv
    20190920_James_Zachary.mp4
    20190920_James_Zachary_release.pdf

The preservation file is a Matroska wrapper with FFV1 codec.  It's much bigger than the compressed camera file with the
proprietary codec.

.. code-block:: rst
    :name: Preservation Matroska file with FFV1 video codec
    :caption: Preservation Matroska file with FFV1 video codec
    :emphasize-lines: 4

    -rwxrwxrwx 1 don don      247632 Oct 10 17:36 20190920_James_Zachary_bioform.pdf
    -rwxrwxrwx 1 don don        1976 Sep 20 15:56 20190920_James_Zachary_Clip0005M01.XML
    -rwxrwxrwx 1 don don  6961631280 Sep 20 15:56 20190920_James_Zachary_Clip0005.MXF
    -rwxrwxrwx 1 don don 40456371435 Sep 22 17:52 20190920_James_Zachary.mkv
    -rwxrwxrwx 1 don don   126651869 Oct  3 09:20 20190920_James_Zachary.mp4
    -rwxrwxrwx 1 don don      334656 Oct 10 17:37 20190920_James_Zachary_release.pdf

Casey has also created us an h264 mp4 proxy / access copy based on the preservation file.

.. code-block:: rst
    :name: Proxy file
    :caption: Proxy file
    :emphasize-lines: 5

    20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_Clip0005M01.XML
    20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary.mkv
    20190920_James_Zachary.mp4
    20190920_James_Zachary_release.pdf

The final 2 files in a standard interview directory are the release file and bioform.  These will not go online but will
be sent to Special Collections.  More information on that here.

.. code-block:: rst
    :name: Bioforms and Release files
    :caption: Bioforms and Release files
    :emphasize-lines: 5

    20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_Clip0005M01.XML
    20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary.mkv
    20190920_James_Zachary.mp4
    20190920_James_Zachary_release.pdf

--------------------
Abnormal Directories
--------------------

Occassionally, some directories may look slightly different. Here is an example:

.. code-block:: rst
    :name: Abnormal directories
    :caption: Abnormal directories

    20190920_Whaley_Daniel_bioform.pdf
    20190920_Whaley_Daniel_release.pdf
    20190920_Whaley_Seemona_bioform.pdf
    20190920_Whaley_Seemona-Daniel_Clip0002M01.XML
    20190920_Whaley_Seemona-Daniel_Clip0002.MXF
    20190920_Whaley_Seemona-Daniel_Clip0003M01.XML
    20190920_Whaley_Seemona-Daniel_Clip0003.MXF
    20190920_Whaley_Seemona-Daniel_combined.mxf
    20190920_Whaley_Seemona-Daniel.mkv
    20190920_Whaley_Seemona-Daniel.mp4
    20190920_Whaley_Seemona_release.pdf

This directory is different for two reasons.  First, there are multiple interviewees, so there are multiple releases and
multiple bioforms.  Again, these won't go online or into Fedora, but we will send these to Special Collections.  More
information about this can be found here.

.. code-block:: rst
    :name: Multiple Bioforms and Release Files
    :caption: Multiple Bioforms and Release Files
    :emphasize-lines: 1-3,11

    20190920_Whaley_Daniel_bioform.pdf
    20190920_Whaley_Daniel_release.pdf
    20190920_Whaley_Seemona_bioform.pdf
    20190920_Whaley_Seemona-Daniel_Clip0002M01.XML
    20190920_Whaley_Seemona-Daniel_Clip0002.MXF
    20190920_Whaley_Seemona-Daniel_Clip0003M01.XML
    20190920_Whaley_Seemona-Daniel_Clip0003.MXF
    20190920_Whaley_Seemona-Daniel_combined.mxf
    20190920_Whaley_Seemona-Daniel.mkv
    20190920_Whaley_Seemona-Daniel.mp4
    20190920_Whaley_Seemona_release.pdf

The other oddity here is that there are more than one original camera capture file.  This is due to the camera being
stopped during recording.  These will not be kept.

.. code-block:: rst
    :name: Multiple Camera Capture Files
    :caption: Multiple Camera Capture Files
    :emphasize-lines: 4-7

    20190920_Whaley_Daniel_bioform.pdf
    20190920_Whaley_Daniel_release.pdf
    20190920_Whaley_Seemona_bioform.pdf
    20190920_Whaley_Seemona-Daniel_Clip0002M01.XML
    20190920_Whaley_Seemona-Daniel_Clip0002.MXF
    20190920_Whaley_Seemona-Daniel_Clip0003M01.XML
    20190920_Whaley_Seemona-Daniel_Clip0003.MXF
    20190920_Whaley_Seemona-Daniel_combined.mxf
    20190920_Whaley_Seemona-Daniel.mkv
    20190920_Whaley_Seemona-Daniel.mp4
    20190920_Whaley_Seemona_release.pdf

