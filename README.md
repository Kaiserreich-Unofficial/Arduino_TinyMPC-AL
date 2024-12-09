# TinyMPC-AL

Under Development

This is a previous attempt of TinyMPC that uses augmented Lagrange method and solve TVLQR online (applicable to nonlinear dynamics). No tricks are played here so it is slow.

New developments are at [https://tinympc.org/](https://tinympc.org/)

## Descriptions

- This is a full library, embedded (optimized) version is under development.
  However, it aims at highly modular integration. You can just use part of the
  sources at your need. Currently, assertion is not present. Users should be
  responsible for this during development.
- AL-TVLQR is ready to use. It is able to handle input/state box constraints and
  goal constraint within stabilization or tracking problems for LTI and LTV
  systems. Check `test/al_lqr_test` for all tests, experiments and examples. Check
  `examples` for MPC experiments.
- You can set constraints on/off in `CMakeLists.txt`, more are under development.
- AL-iLQR is under development. It is able to handle input/state box constraints
  and goal constraint within stabilization or tracking problems for nonlinear
  systems.
