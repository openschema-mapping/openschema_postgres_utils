# openSCHEMA postgreSQL ORM and Interface Utils

## Structure
``` text
.
.devcontainer/              <-- VSCode devcontainer settings
.github/workflows/          <-- github specific workflow settings
.vscode/                    <-- VSCode specific settings, launch settings
src/openschema_alchemy/
  ├─ map_format/            <-- openVSLAM specific i/o lib for each format
  ├─ model/                 <-- openSCHEMA ORM model
  ├─ openschema_utils/      <-- math and i/o utils
  ├─ openschema_loader.py   <-- tool to load data to and from the db
  ├─ openschema_roi_editor.py   <-- tool to augment ROIs (defined in e.g. qgis) with additional meta info
  ├─ openschema_pointcloud_exporter.py   <-- tool to export data geometric data from the openSCHEMA DB
  ├─ openschema_loader.py   <-- tool to visualize meta data of the openSCHEMA DB
.gitignore
Dockerfile                  <-- Dockerfile used by VSCode with all deps
LICENSE
README.md
pyproject.toml
setup.cfg
setup.py
tox.ini
```

## Setup with Visual Studio Code (+devcontainer)
Navigate to base directory and open with VSCode:
``` bash
> cd openschema_postgres_utils
> code .
```
Use `Ctrl+Shift+P` and `Remote-Container: Reopen in Container`.

## How to Cite this project
The paper presenting the general database schema will be published at the ICMVA '24 (already accepted).
Please cite as
```
@inproceedings{wallner2024,
  author = {Wallner, Marco and Schörghuber, Matthias and Hofstätter, Markus},
  title = {A Unified Database Schema for Geometric and Semantic Data: Continuous Volumetric Stocktaking in Gravel Quarries},
  year = {2024},
  isbn = {TODO},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA},
  url = {TODO},
  doi = {TODO},
  pages = {TODO},
  numpages = {TODO},
  keywords = {spatial database, geometric and semantic data, application, volume estimate, continuous stocktaking},
  location = {Singapore, Singapore},
  series = {ICMVA '24}
}
```

## ROSCon Tech Talk
Parts of the project and a generic bridge from a PostgreSQL database with PostGIS elements to ROS2 were presented at ROSCon 2023 in New Orleans, LA, USA.

The code repo of the ROS2 node and an demo workspace can be found here:<br>
ROS2 Node: https://github.com/AIT-Assistive-Autonomous-Systems/postgis_ros_bridge <br>
VSCode Demo Workspace: https://github.com/AIT-Assistive-Autonomous-Systems/postgis_ros_bridge_demo_workspace

The talk and the slides are hosted here:<br>
Talk: https://vimeo.com/879001513/61784cb23e <br>
Slides: https://roscon.ros.org/talks/PostgreSQL__PostGIS_to_ROS_2_Bridge_for_Spatial_Data.pdf

## .gitignore

The [.gitignore](.gitignore) file is a copy of the [Github C++.gitignore file](https://github.com/github/gitignore/blob/master/C%2B%2B.gitignore),
with the addition of ignoring the build directory (`build/`).

## FFG Project
[DE ]Die FFG ist die zentrale nationale Förderorganisation und stärkt Österreichs Innovationskraft. Dieses Projekt wird aus Mitteln der FFG gefördert. 

[EN] FFG is the central national funding organization and strengthens Austria's innovative power. This project is funded by the FFG. 

[www.ffg.at](www.ffg.at)

Projekt: [openSCHEMA](https://iktderzukunft.at/de/projekte/open-semantic-collaborative-hierarchical-environment-mapping.php)