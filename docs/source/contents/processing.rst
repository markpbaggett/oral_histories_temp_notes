===============
Receiving Files
===============

-----
Goals
-----

1. **Keep the files we need**: In this first run, Casey gave us extra files to determine which files we wanted to preserve
and what our workflow should look like going forward.

2. **Get other files to the people that need them**: We won't be preserving all the files here, but we need to get
the files others need to them.

3. **Cleanup the drive**:  Casey will reuse this drive, so we need to cleanup the drive as we go.

------------
What we need
------------

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
    :name: MP4 datastream
    :caption: MP4 datastream
    :emphasize-lines: 5

    20190920_James_Zachary_bioform.pdf
    20190920_James_Zachary_Clip0005M01.XML
    20190920_James_Zachary_Clip0005.MXF
    20190920_James_Zachary.mkv
    20190920_James_Zachary.mp4
    20190920_James_Zachary_release.pdf
