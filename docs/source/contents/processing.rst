===============
Receiving Files
===============

-----
Goals
-----

1. **Checksum check the files sent by Casey**: Since Casey sent us Checksums for each file, let's test them versus the
files we received.

2. **Keep the files we need**: In this first run, Casey gave us extra files to determine which files we wanted to preserve
and what our workflow should look like going forward.

3. **Get other files to the people that need them**: We won't be preserving all the files here, but we need to get
the files others need to them.

4. **Cleanup the drive**:  Casey will reuse this drive, so we need to cleanup the drive as we go.

5. **Ingest the Object and Restrict all datastreams**: As quickly as possible, we need to get this object into Fedora but
ensure that all datastreams and the object itself is restricted.

-----------------
What I think need
-----------------

Using the `directory structure <../directory.html>`_ documentation as a guide, we need to use Casey's preservation mkv as our OBJ and her
mp4 as our access copy. According to the `video solution pack documentation <https://wiki.duraspace.org/display/ISLANDORA/Video+Solution+Pack>`_,
"Most players require a datastream called "MP4". Check this option to create the MP4 datastream locally. Disable this if
another server will create derivatives." Since Casey has created this for us, let's try to use it and not rely on the
server to process the preservation file.

.. code-block:: rst
    :name: OBJ datastream
    :caption: OBJ datastream
    :emphasize-lines: 4

    20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_Clip0005M01.XML
    20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary.mkv
    20190920_James_Zachary.mp4
    20190920_James_Zachary_release.pdf

.. code-block:: rst
    :name: Temporary Access MP4 datastream
    :caption: Temporary Access MP4 datastream
    :emphasize-lines: 5

    20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_Clip0005M01.XML
    20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary.mkv
    20190920_James_Zachary.mp4
    20190920_James_Zachary_release.pdf

It's important to note that the access copy will be replaced before go live with something else altogether.  This processed
access copy will have branding and other data.  The access copy we will be storing for now will only be used if there is
a question or someone wants to review something.

We also need metadata for ingestion. The metadata file that Casey has provided for us is incomplete and will grow substantially
during the "cataloging" phase of the project. For this reason, we can create a simple metadata record with minimal data.

--------
Workflow
--------

What will our workflow look like going forward? Document here:
