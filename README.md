==================================================
DATASET DESCRIPTION
==================================================

■ Overview
--------------------------------------------------
The Guizhou traffic flow dataset is collected from real-world traffic operation data
on major urban road segments in Guiyang City, Guizhou Province, China.

The dataset consists of 132 road segments, together with their upstream and downstream
topological relationships, which describe the spatial structure of the road network.
It contains average travel time records from March to May 2016 and from March to May
2017.

In this study, travel time is selected as the prediction target, while the remaining
variables are used as input features.


■ File Structure
--------------------------------------------------
The dataset is organized into the following files:

  ▶ gy_link_info.txt
  ▶ gy_link_top.txt
  ▶ part1.txt, part2.txt, part3.txt


■ 1. Road Network Information
--------------------------------------------------
(gy_link_info.txt and gy_link_top.txt)

These files provide road segment attributes and connectivity information, which can be
used to construct the adjacency matrix of the traffic network.


  ◇ Variables

      ▸ link_ID
          Type: string
          Description: Unique identifier of a road segment, consistent with the
                       identifiers used in the travel time data.

      ▸ length
          Type: integer
          Description: Physical length of the road segment, measured in meters.

      ▸ width
          Type: integer
          Description: Width of the road segment, measured in meters.

      ▸ link_class
          Type: integer
          Description: Road classification level, indicating the functional
                       category of the road segment.


■ 2. Traffic Flow Data
--------------------------------------------------
(part1.txt, part2.txt, part3.txt)

Each file contains raw traffic flow records for road segments.


  ◇ Variables

      ▸ link_ID
          Description: Identifier of the road segment.

      ▸ date
          Description: Calendar date of the traffic observation.

      ▸ time_interval
          Description: Time interval during which the traffic measurement is
                       aggregated.

      ▸ travel_time
          Description: Average travel time of vehicles on the corresponding road
                       segment during the given time interval, measured in seconds.
