# Trajectory analysis on Dota 2

This group project contains the tools necessary to perform a trajectory analysis, here on data from Dota 2. You can find our results in the repport (in french).

To extract knowledge from our trajectory data, we performed a compression method based on the MDL principle, then a discretisation of the trajectories by using clustering and then used a given sequential pattern extraction using a library that implements a sequential prefixpan.

## Compression and clustering

In the directory compression_clustering, you will find the C++ code for the compression and clustering part. We use Open MP to do parallelization and Boost library for filesystem operations and for matrix structures. 

We implemented:
  - an approximate MDL compression algorithm introduced by Jae-Gil Lee and Jiawei Han. We were able to reduce the path size by 62.9%.
  - K-means
  - K-medoids
  - Affinity Propagation. /!\ this implementation while performing quite okay and parallelized, isn't perfectly implemented (as we lack knowledge about the boost library). Also, you must note that its space complexity make it unsuited for this application.
  
# Sequential pattern mining

In the directory extraction, you will find all the script you need to run an extraction from our previous results.

Sadly, we did not manage to extract interesting knowledge from this part as we didn't have enough time to study this part.

[![Plugin Version](https://img.shields.io/wordpress/plugin/v/dirtysuds-embed-pdf.svg)](https://wordpress.org/plugins/dirtysuds-embed-pdf/)
[![License](https://img.shields.io/badge/license-GPLv2-blue.svg)](https://wordpress.org/about/license/)
[![Tested Version](https://img.shields.io/wordpress/v/dirtysuds-embed-pdf.svg)](https://wordpress.org/plugins/dirtysuds-embed-pdf/)
[![Rating](https://img.shields.io/wordpress/plugin/r/dirtysuds-embed-pdf.svg)](https://wordpress.org/support/view/plugin-reviews/dirtysuds-embed-pdf)
[![Downloads](https://img.shields.io/wordpress/plugin/dt/dirtysuds-embed-pdf.svg)](https://wordpress.org/plugins/dirtysuds-embed-pdf/)

[embed]https://github.com/Linthora/trajectory_analysis_dota/blob/main/Rapport_projet_dota-1.pdf[/embed]
