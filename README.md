# Example dataset for MarsBaR

This dataset contains three EPI runs from a single subject.  See the
following abstract and poster for more details on the design of the
experiment:

<http://www.mrc-cbu.cam.ac.uk/Imaging/~matthew.brett/abstracts/ER/er_analysis.html>

The dataset is designed to be used with the MarsBaR tutorial, which
should be available via the MarsBaR home page:

<https://marsbar-toolbox.github.io/>

We acquired the three runs (sessions) during a task using visual
events presented with random intervals between events.  In session 1
the average interval between events was 1 second, the average interval
was 3 seconds for session 2 and 10 seconds for session 3.

The dataset contains slice-time corrected realigned undistorted
normalized images, with prefix "nrua", in three data directories,
sess1, sess2 and sess3.

All the preprocessing scripts are in the main marsbar distribution, in
the 'examples/batch' subdirectory.  To run initial processing on the
dataset in SPM, start Matlab, change to the `<marsbar>/examples/batch`
directory, and, from the console window run:

```
run_preprocess
```

The routines will create smoothed images and run a standard
SPM statistical model on each of the three sessions.

The routines should work with SPM99 through SPM12.

There is also an example batch script for MarsBaR that replicates the
analyses described in the MarsBaR tutorial; see
<https://marsbar-toolbox.github.io>.  To run:

```
run_tutorial
```

Please use the MarsBaR Disourse forum for any questions or to report
problems:

<https://marsbar.discourse.group>

We wish you a pleasant FMRI experience,

Matthew Brett (for the the team).
14 August 2004, 27 September 2021.
