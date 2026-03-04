---
title: Run NLL
updated: 2025-11-08T20:46:09
created: 2025-05-22T11:19:22
---

Run NLL
Kamis, 22 Mei 2025
11.19

Create 4 main folders:
1.  obs --\> pick data, station
2.  run --\> control file
3.  model --\> store vp vs model result
4.  time --\> store travel time and angle result
5.  Loc --\> store nlloc locate result
6.  Gmt --\> store plotted map

Control File setup
CONTROL 1 54321
TRANS SIMPLE -5.3143 104.5825 0.0 --\> central coordinate
VGOUT ./model/layer
VGTYPE P
VGTYPE S
VGGRID 2 401 351 -10.0 -10.0 -3.0 0.05 0.05 0.05 SLOW_LEN --\> velocity 2D model setup, vx = vy = vz
\#LAYER depth Vp_top Vp_grad Vs_top Vs_grad p_top p_grad
LAYER -0.1 2.60 0.00 1.48 0.00 2.2 0.0
Etc etc velocity model
…..

\#GTFILES ./model/layer ./time/layer P \# uncomment to generate P travel times
GTFILES ./model/layer ./time/layer S \# uncomment to generate S travel times
\#run 2 times, uncomment for each P and S

GTMODE GRID2D ANGLES_YES
INCLUDE obs/station_coordinates.txt --\> edit txt
GT_PLFD 1.0e-3 0
EQFILES ./time/layer ./obs/synth.obs
EQMECH DOUBLE 0.0 90.0 0.0
EQMODE SRCE_TO_STA
EQEVENT EQ001 0.0 0.0 10.0 0.0
EQSTA MEQ2S P GAU 0.01 GAU 0.1
EQSTA STAxx P GAU 0.01 GAU 0.1
Etc etc edit station list …..

EQVPVS 1.73
EQQUAL2ERR 0.1 0.2 0.4 0.8 99999.9
LOCSIG NonLinLoc - ALomax Scientific
LOCCOM ulubelu --\> change to loc ID
LOCFILES ./obs/\*.pick NLLOC_OBS ./time/layer ./loc/ulubelu
LOCHYPOUT SAVE_NLLOC_ALL SAVE_HYPOINV_SUM
LOCSEARCH OCT 21 21 11 0.001 100000 10000 0 1
LOCGRID 301 301 141 -5.0 -5.0 -0.6 0.03 0.03 0.03 PROB_DENSITY SAVE --\> change to match grid search space
LOCMETH EDT_OT_WT 9999.0 4 -1 -1 1.68 6 -1.0 1
LOCGAU 0.2 0.0
LOCGAU2 0.01 0.05 2.0
LOCQUAL2ERR 0.1 0.5 1.0 2.0 99999.9
LOCANGLES ANGLES_YES 5
LOCMAG ML_HB 1.0 1.110 0.00189
LOCPHSTAT 9999.0 -1 9999.0 1.0 1.0 9999.9 -9999.9 9999.9

Running
Vel2Grid run/PaluKoro.in
Grid2Time run/PaluKoro.in
NLLoc run/PaluKoro.in

