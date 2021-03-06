.. THIS IS A GENERATED FILE

CLI Reference
=============


General Options
---------------


``--workers``
   The number of concurrent downloads when requesting multiple scenes.



``--verbose``
   Specify verbosity



``--api_key``
   Valid API key - or via env variable PL_API_KEY



``--base_url``
   Optional for testing



``--version``
   Show the version and exit.



Commands
--------


:ref:`cli-command-download` Download full scene image(s).



:ref:`cli-command-download-quads` Download quad geotiffs



:ref:`cli-command-get-workspace` Get workspace.



:ref:`cli-command-help` Get command help



:ref:`cli-command-init` Login using email/password



:ref:`cli-command-list-workspaces` List workspaces.



:ref:`cli-command-metadata` Get scene metadata



:ref:`cli-command-mosaic` Describe a specified mosaic



:ref:`cli-command-mosaic-quads` Get quad info for the specified mosaic



:ref:`cli-command-mosaics` List all mosaics



:ref:`cli-command-search` Get a list of scenes.



:ref:`cli-command-set-workspace` Create or modify a workspace



:ref:`cli-command-sync` Synchronize a directory to a specified AOI or...



:ref:`cli-command-thumbnails` Fetch scene thumbnail(s)



.. index:: download

.. _cli-command-download:


download
........


Download full scene image(s).

Usage: download [OPTIONS] [SCENE_IDS]...

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - product
     - 
   * - dest
     - Destination directory
   * - scene_type
     - Type of scene
.. index:: download-quads

.. _cli-command-download-quads:


download-quads
..............


Download quad geotiffs

Usage: download-quads [OPTIONS] MOSAIC_NAME [QUAD_IDS]...

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - dest
     - Destination directory
.. index:: get-workspace

.. _cli-command-get-workspace:


get-workspace
.............


Get workspace.

Usage: get-workspace [OPTIONS] ID

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - pretty
     - Format JSON output
.. index:: help

.. _cli-command-help:


help
....


Get command help

Usage: help [OPTIONS] [COMMAND]

.. index:: init

.. _cli-command-init:


init
....


Login using email/password

Usage: init [OPTIONS]

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - email
     - 
   * - password
     - 
.. index:: list-workspaces

.. _cli-command-list-workspaces:


list-workspaces
...............


List workspaces.

Usage: list-workspaces [OPTIONS]

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - pretty
     - Format JSON output
.. index:: metadata

.. _cli-command-metadata:


metadata
........


Get scene metadata

Usage: metadata [OPTIONS] SCENE_ID

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - scene_type
     - Type of scene
   * - pretty
     - Format JSON output
.. index:: mosaic

.. _cli-command-mosaic:


mosaic
......


Describe a specified mosaic

Usage: mosaic [OPTIONS] MOSAIC_NAME

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - pretty
     - Format JSON output
.. index:: mosaic-quads

.. _cli-command-mosaic-quads:


mosaic-quads
............


Get quad info for the specified mosaic

Usage: mosaic-quads [OPTIONS] MOSAIC_NAME

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - limit
     - Limit the number of items.
   * - pretty
     - Format JSON output
.. index:: mosaics

.. _cli-command-mosaics:


mosaics
.......


List all mosaics

Usage: mosaics [OPTIONS]

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - limit
     - Limit the number of items.
   * - pretty
     - Format JSON output
.. index:: search

.. _cli-command-search:


search
......


Get a list of scenes.

Usage: search [OPTIONS] [AOI]

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - limit
     - Limit the number of items.
   * - where
     - Provide additional search criteria. See https://www.planet.com/docs/v0/scenes/#metadata for search metadata fields.
   * - workspace
     - Workspace ID
   * - scene_type
     - Type of scene
   * - pretty
     - Format JSON output
.. index:: set-workspace

.. _cli-command-set-workspace:


set-workspace
.............


Create or modify a workspace

Usage: set-workspace [OPTIONS] [WORKSPACE]

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - id
     - If provided, update the workspace with this id
   * - aoi
     - The geometry to use
   * - name
     - Workspace name
   * - create
     - Specify workspace creation
.. index:: sync

.. _cli-command-sync:


sync
....


Synchronize a directory to a specified AOI or workspace

Usage: sync [OPTIONS] DESTINATION

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - dryrun
     - Do not actually download
   * - limit
     - Limit the number of items.
   * - workspace
     - Workspace ID
   * - scene_type
     - Type of scene
.. index:: thumbnails

.. _cli-command-thumbnails:


thumbnails
..........


Fetch scene thumbnail(s)

Usage: thumbnails [OPTIONS] [SCENE_IDS]...

.. list-table:: Options
   :header-rows: 1

   * - Name
     - Description
   * - fmt
     - Thumbnail format
   * - size
     - Thumbnail size
   * - dest
     - Destination directory
   * - scene_type
     - Type of scene
