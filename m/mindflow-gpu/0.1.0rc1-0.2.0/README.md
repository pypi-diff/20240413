# Comparing `tmp/mindflow_gpu-0.1.0rc1-py3-none-any.whl.zip` & `tmp/mindflow_gpu-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,98 +1,108 @@
-Zip file size: 144569 bytes, number of entries: 96
--rw-r--r--  2.0 unx     2948 b- defN 23-Apr-04 12:21 mindflow/__init__.py
--rw-r--r--  2.0 unx     2239 b- defN 23-Apr-04 12:21 mindflow/setup.py
--rw-r--r--  2.0 unx     1012 b- defN 23-Apr-04 12:21 mindflow/cell/__init__.py
--rw-r--r--  2.0 unx     3492 b- defN 23-Apr-04 12:21 mindflow/cell/activation.py
--rw-r--r--  2.0 unx    21416 b- defN 23-Apr-04 12:21 mindflow/cell/basic_block.py
--rw-r--r--  2.0 unx     5040 b- defN 23-Apr-04 12:21 mindflow/cell/utils.py
--rw-r--r--  2.0 unx      811 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/__init__.py
--rw-r--r--  2.0 unx    14413 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/dft.py
--rw-r--r--  2.0 unx     7688 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/fno1d.py
--rw-r--r--  2.0 unx     9511 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/fno2d.py
--rw-r--r--  2.0 unx     2357 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/m2k.py
--rw-r--r--  2.0 unx     9671 b- defN 23-Apr-04 12:21 mindflow/cell/neural_operators/pdenet.py
--rw-r--r--  2.0 unx      699 b- defN 23-Apr-04 12:21 mindflow/cell/transformer/__init__.py
--rw-r--r--  2.0 unx    14042 b- defN 23-Apr-04 12:21 mindflow/cell/transformer/layer.py
--rw-r--r--  2.0 unx     6350 b- defN 23-Apr-04 12:21 mindflow/cell/transformer/vit.py
--rw-r--r--  2.0 unx      971 b- defN 23-Apr-04 12:21 mindflow/cfd/__init__.py
--rw-r--r--  2.0 unx     2531 b- defN 23-Apr-04 12:21 mindflow/cfd/mesh_info.py
--rw-r--r--  2.0 unx     4168 b- defN 23-Apr-04 12:21 mindflow/cfd/runtime.py
--rw-r--r--  2.0 unx     3298 b- defN 23-Apr-04 12:21 mindflow/cfd/simulator.py
--rw-r--r--  2.0 unx     4714 b- defN 23-Apr-04 12:21 mindflow/cfd/utils.py
--rw-r--r--  2.0 unx     2956 b- defN 23-Apr-04 12:21 mindflow/cfd/visualization.py
--rw-r--r--  2.0 unx      749 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/__init__.py
--rw-r--r--  2.0 unx     1165 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/base.py
--rw-r--r--  2.0 unx     2752 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/boundary_manager.py
--rw-r--r--  2.0 unx     1247 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/neumann.py
--rw-r--r--  2.0 unx     1173 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/periodic.py
--rw-r--r--  2.0 unx     1319 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/symmetry.py
--rw-r--r--  2.0 unx     1836 b- defN 23-Apr-04 12:21 mindflow/cfd/boundary_conditions/wall.py
--rw-r--r--  2.0 unx     1119 b- defN 23-Apr-04 12:21 mindflow/cfd/integrator/__init__.py
--rw-r--r--  2.0 unx      935 b- defN 23-Apr-04 12:21 mindflow/cfd/integrator/base.py
--rw-r--r--  2.0 unx     1056 b- defN 23-Apr-04 12:21 mindflow/cfd/integrator/euler.py
--rw-r--r--  2.0 unx     1307 b- defN 23-Apr-04 12:21 mindflow/cfd/integrator/runge_kutta3.py
--rw-r--r--  2.0 unx     1054 b- defN 23-Apr-04 12:21 mindflow/cfd/material/__init__.py
--rw-r--r--  2.0 unx     2685 b- defN 23-Apr-04 12:21 mindflow/cfd/material/base.py
--rw-r--r--  2.0 unx     1897 b- defN 23-Apr-04 12:21 mindflow/cfd/material/ideal_gas.py
--rw-r--r--  2.0 unx      735 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/__init__.py
--rw-r--r--  2.0 unx     1812 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/godunov_flux.py
--rw-r--r--  2.0 unx     2982 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/space_solver.py
--rw-r--r--  2.0 unx     6133 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/viscous_flux.py
--rw-r--r--  2.0 unx     1348 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/derivative_computer/__init__.py
--rw-r--r--  2.0 unx     1090 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/derivative_computer/base.py
--rw-r--r--  2.0 unx     2675 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/derivative_computer/forth_order_central_derivative_computer.py
--rw-r--r--  2.0 unx     2624 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/derivative_computer/forth_order_face_derivative_computer.py
--rw-r--r--  2.0 unx     1142 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/interpolator/__init__.py
--rw-r--r--  2.0 unx     1031 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/interpolator/base.py
--rw-r--r--  2.0 unx     2576 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/interpolator/central_forth_order_interpolator.py
--rw-r--r--  2.0 unx     1045 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/reconstructor/__init__.py
--rw-r--r--  2.0 unx     2064 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/reconstructor/base.py
--rw-r--r--  2.0 unx     6315 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/reconstructor/weno5.py
--rw-r--r--  2.0 unx     1114 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/riemann_computer/__init__.py
--rw-r--r--  2.0 unx     1021 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/riemann_computer/base.py
--rw-r--r--  2.0 unx     2374 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/riemann_computer/rusanov.py
--rw-r--r--  2.0 unx     3636 b- defN 23-Apr-04 12:21 mindflow/cfd/space_solver/riemann_computer/rusanov_net.py
--rw-r--r--  2.0 unx      884 b- defN 23-Apr-04 12:21 mindflow/common/__init__.py
--rw-r--r--  2.0 unx     9966 b- defN 23-Apr-04 12:21 mindflow/common/lr_scheduler.py
--rw-r--r--  2.0 unx     2014 b- defN 23-Apr-04 12:21 mindflow/common/math.py
--rw-r--r--  2.0 unx     1145 b- defN 23-Apr-04 12:21 mindflow/data/__init__.py
--rw-r--r--  2.0 unx     8430 b- defN 23-Apr-04 12:21 mindflow/data/boundary.py
--rw-r--r--  2.0 unx     5624 b- defN 23-Apr-04 12:21 mindflow/data/data_base.py
--rw-r--r--  2.0 unx    18758 b- defN 23-Apr-04 12:21 mindflow/data/dataset.py
--rw-r--r--  2.0 unx     5436 b- defN 23-Apr-04 12:21 mindflow/data/equation.py
--rw-r--r--  2.0 unx     6960 b- defN 23-Apr-04 12:21 mindflow/data/existed_data.py
--rw-r--r--  2.0 unx    12556 b- defN 23-Apr-04 12:21 mindflow/data/mind_dataset.py
--rw-r--r--  2.0 unx     1542 b- defN 23-Apr-04 12:21 mindflow/geometry/__init__.py
--rw-r--r--  2.0 unx    29673 b- defN 23-Apr-04 12:21 mindflow/geometry/csg.py
--rw-r--r--  2.0 unx     5593 b- defN 23-Apr-04 12:21 mindflow/geometry/geom_utils.py
--rw-r--r--  2.0 unx     2355 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_1d.py
--rw-r--r--  2.0 unx    15747 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_2d.py
--rw-r--r--  2.0 unx     9383 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_3d.py
--rw-r--r--  2.0 unx    11153 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_base.py
--rw-r--r--  2.0 unx    15732 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_nd.py
--rw-r--r--  2.0 unx    13857 b- defN 23-Apr-04 12:21 mindflow/geometry/geometry_td.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/__init__.py
--rw-r--r--  2.0 unx     2337 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/adapter.py
--rw-r--r--  2.0 unx     2708 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/pentagon.py
--rw-r--r--  2.0 unx     7023 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/rotating.py
--rw-r--r--  2.0 unx     3146 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/shapes.py
--rw-r--r--  2.0 unx     6579 b- defN 23-Apr-04 12:21 mindflow/geometry/shapes/simplex.py
--rw-r--r--  2.0 unx      926 b- defN 23-Apr-04 12:21 mindflow/loss/__init__.py
--rw-r--r--  2.0 unx    14215 b- defN 23-Apr-04 12:21 mindflow/loss/losses.py
--rw-r--r--  2.0 unx      804 b- defN 23-Apr-04 12:21 mindflow/operators/__init__.py
--rw-r--r--  2.0 unx     4635 b- defN 23-Apr-04 12:21 mindflow/operators/derivatives.py
--rw-r--r--  2.0 unx     1056 b- defN 23-Apr-04 12:21 mindflow/pde/__init__.py
--rw-r--r--  2.0 unx     8517 b- defN 23-Apr-04 12:21 mindflow/pde/flow_with_loss.py
--rw-r--r--  2.0 unx    15750 b- defN 23-Apr-04 12:21 mindflow/pde/pde_with_loss.py
--rw-r--r--  2.0 unx      788 b- defN 23-Apr-04 12:21 mindflow/pde/sympy2mindspore/__init__.py
--rw-r--r--  2.0 unx     3087 b- defN 23-Apr-04 12:21 mindflow/pde/sympy2mindspore/parse_sympy.py
--rw-r--r--  2.0 unx     6012 b- defN 23-Apr-04 12:21 mindflow/pde/sympy2mindspore/pde_node.py
--rw-r--r--  2.0 unx     7047 b- defN 23-Apr-04 12:21 mindflow/pde/sympy2mindspore/sympy_translation.py
--rw-r--r--  2.0 unx      773 b- defN 23-Apr-04 12:21 mindflow/utils/__init__.py
--rw-r--r--  2.0 unx     5419 b- defN 23-Apr-04 12:21 mindflow/utils/check_func.py
--rw-r--r--  2.0 unx     1898 b- defN 23-Apr-04 12:21 mindflow/utils/load_config.py
--rw-r--r--  2.0 unx      691 b- defN 23-Apr-04 12:21 mindflow_gpu-0.1.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-04 12:21 mindflow_gpu-0.1.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-04 12:21 mindflow_gpu-0.1.0rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8909 b- defN 23-Apr-04 12:21 mindflow_gpu-0.1.0rc1.dist-info/RECORD
-96 files, 461567 bytes uncompressed, 130253 bytes compressed:  71.8%
+Zip file size: 166618 bytes, number of entries: 106
+-rw-r--r--  2.0 unx     2948 b- defN 24-Mar-15 07:24 mindflow/__init__.py
+-rw-r--r--  2.0 unx     2239 b- defN 24-Mar-15 07:24 mindflow/setup.py
+-rw-r--r--  2.0 unx     1115 b- defN 24-Mar-15 07:24 mindflow/cell/__init__.py
+-rw-r--r--  2.0 unx     3516 b- defN 24-Mar-15 07:24 mindflow/cell/activation.py
+-rw-r--r--  2.0 unx    21680 b- defN 24-Mar-15 07:24 mindflow/cell/basic_block.py
+-rw-r--r--  2.0 unx     7064 b- defN 24-Mar-15 07:24 mindflow/cell/unet2d.py
+-rw-r--r--  2.0 unx     5355 b- defN 24-Mar-15 07:24 mindflow/cell/utils.py
+-rw-r--r--  2.0 unx      936 b- defN 24-Mar-15 07:24 mindflow/cell/neural_operators/__init__.py
+-rw-r--r--  2.0 unx    34318 b- defN 24-Mar-15 07:24 mindflow/cell/neural_operators/dft.py
+-rw-r--r--  2.0 unx    28824 b- defN 24-Mar-15 07:24 mindflow/cell/neural_operators/fno.py
+-rw-r--r--  2.0 unx     4667 b- defN 24-Mar-15 07:24 mindflow/cell/neural_operators/kno1d.py
+-rw-r--r--  2.0 unx     4867 b- defN 24-Mar-15 07:24 mindflow/cell/neural_operators/kno2d.py
+-rw-r--r--  2.0 unx     2357 b- defN 24-Mar-15 07:24 mindflow/cell/neural_operators/m2k.py
+-rw-r--r--  2.0 unx     9695 b- defN 24-Mar-15 07:24 mindflow/cell/neural_operators/pdenet.py
+-rw-r--r--  2.0 unx    12845 b- defN 24-Mar-15 07:24 mindflow/cell/neural_operators/percnn.py
+-rw-r--r--  2.0 unx      699 b- defN 24-Mar-15 07:24 mindflow/cell/transformer/__init__.py
+-rw-r--r--  2.0 unx    14082 b- defN 24-Mar-15 07:24 mindflow/cell/transformer/layer.py
+-rw-r--r--  2.0 unx     6402 b- defN 24-Mar-15 07:24 mindflow/cell/transformer/vit.py
+-rw-r--r--  2.0 unx      971 b- defN 24-Mar-15 07:24 mindflow/cfd/__init__.py
+-rw-r--r--  2.0 unx     2531 b- defN 24-Mar-15 07:24 mindflow/cfd/mesh_info.py
+-rw-r--r--  2.0 unx     4178 b- defN 24-Mar-15 07:24 mindflow/cfd/runtime.py
+-rw-r--r--  2.0 unx     3302 b- defN 24-Mar-15 07:24 mindflow/cfd/simulator.py
+-rw-r--r--  2.0 unx     4746 b- defN 24-Mar-15 07:24 mindflow/cfd/utils.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-Mar-15 07:24 mindflow/cfd/visualization.py
+-rw-r--r--  2.0 unx      749 b- defN 24-Mar-15 07:24 mindflow/cfd/boundary_conditions/__init__.py
+-rw-r--r--  2.0 unx     1165 b- defN 24-Mar-15 07:24 mindflow/cfd/boundary_conditions/base.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-Mar-15 07:24 mindflow/cfd/boundary_conditions/boundary_manager.py
+-rw-r--r--  2.0 unx     1247 b- defN 24-Mar-15 07:24 mindflow/cfd/boundary_conditions/neumann.py
+-rw-r--r--  2.0 unx     1173 b- defN 24-Mar-15 07:24 mindflow/cfd/boundary_conditions/periodic.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-Mar-15 07:24 mindflow/cfd/boundary_conditions/symmetry.py
+-rw-r--r--  2.0 unx     1836 b- defN 24-Mar-15 07:24 mindflow/cfd/boundary_conditions/wall.py
+-rw-r--r--  2.0 unx     1119 b- defN 24-Mar-15 07:24 mindflow/cfd/integrator/__init__.py
+-rw-r--r--  2.0 unx      935 b- defN 24-Mar-15 07:24 mindflow/cfd/integrator/base.py
+-rw-r--r--  2.0 unx     1056 b- defN 24-Mar-15 07:24 mindflow/cfd/integrator/euler.py
+-rw-r--r--  2.0 unx     1307 b- defN 24-Mar-15 07:24 mindflow/cfd/integrator/runge_kutta3.py
+-rw-r--r--  2.0 unx     1054 b- defN 24-Mar-15 07:24 mindflow/cfd/material/__init__.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-Mar-15 07:24 mindflow/cfd/material/base.py
+-rw-r--r--  2.0 unx     1897 b- defN 24-Mar-15 07:24 mindflow/cfd/material/ideal_gas.py
+-rw-r--r--  2.0 unx      735 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/__init__.py
+-rw-r--r--  2.0 unx     1812 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/godunov_flux.py
+-rw-r--r--  2.0 unx     2982 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/space_solver.py
+-rw-r--r--  2.0 unx     6133 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/viscous_flux.py
+-rw-r--r--  2.0 unx     1348 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/derivative_computer/__init__.py
+-rw-r--r--  2.0 unx     1090 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/derivative_computer/base.py
+-rw-r--r--  2.0 unx     2675 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/derivative_computer/forth_order_central_derivative_computer.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/derivative_computer/forth_order_face_derivative_computer.py
+-rw-r--r--  2.0 unx     1142 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/interpolator/__init__.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/interpolator/base.py
+-rw-r--r--  2.0 unx     2576 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/interpolator/central_forth_order_interpolator.py
+-rw-r--r--  2.0 unx     1135 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/reconstructor/__init__.py
+-rw-r--r--  2.0 unx     2064 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/reconstructor/base.py
+-rw-r--r--  2.0 unx     4739 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/reconstructor/weno3.py
+-rw-r--r--  2.0 unx     6315 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/reconstructor/weno5.py
+-rw-r--r--  2.0 unx     8658 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/reconstructor/weno7.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/riemann_computer/__init__.py
+-rw-r--r--  2.0 unx     1021 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/riemann_computer/base.py
+-rw-r--r--  2.0 unx     6303 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/riemann_computer/hllc.py
+-rw-r--r--  2.0 unx    15258 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/riemann_computer/roe.py
+-rw-r--r--  2.0 unx     2374 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/riemann_computer/rusanov.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-Mar-15 07:24 mindflow/cfd/space_solver/riemann_computer/rusanov_net.py
+-rw-r--r--  2.0 unx      884 b- defN 24-Mar-15 07:24 mindflow/common/__init__.py
+-rw-r--r--  2.0 unx    10167 b- defN 24-Mar-15 07:24 mindflow/common/lr_scheduler.py
+-rw-r--r--  2.0 unx     2331 b- defN 24-Mar-15 07:24 mindflow/common/math.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-Mar-15 07:24 mindflow/data/__init__.py
+-rw-r--r--  2.0 unx     8533 b- defN 24-Mar-15 07:24 mindflow/data/boundary.py
+-rw-r--r--  2.0 unx     5744 b- defN 24-Mar-15 07:24 mindflow/data/data_base.py
+-rw-r--r--  2.0 unx    19200 b- defN 24-Mar-15 07:24 mindflow/data/dataset.py
+-rw-r--r--  2.0 unx     5450 b- defN 24-Mar-15 07:24 mindflow/data/equation.py
+-rw-r--r--  2.0 unx     7040 b- defN 24-Mar-15 07:24 mindflow/data/existed_data.py
+-rw-r--r--  2.0 unx    12848 b- defN 24-Mar-15 07:24 mindflow/data/mind_dataset.py
+-rw-r--r--  2.0 unx     1567 b- defN 24-Mar-15 07:24 mindflow/geometry/__init__.py
+-rw-r--r--  2.0 unx    29715 b- defN 24-Mar-15 07:24 mindflow/geometry/csg.py
+-rw-r--r--  2.0 unx     5587 b- defN 24-Mar-15 07:24 mindflow/geometry/geom_utils.py
+-rw-r--r--  2.0 unx     2363 b- defN 24-Mar-15 07:24 mindflow/geometry/geometry_1d.py
+-rw-r--r--  2.0 unx    17748 b- defN 24-Mar-15 07:24 mindflow/geometry/geometry_2d.py
+-rw-r--r--  2.0 unx     9475 b- defN 24-Mar-15 07:24 mindflow/geometry/geometry_3d.py
+-rw-r--r--  2.0 unx    11185 b- defN 24-Mar-15 07:24 mindflow/geometry/geometry_base.py
+-rw-r--r--  2.0 unx    15897 b- defN 24-Mar-15 07:24 mindflow/geometry/geometry_nd.py
+-rw-r--r--  2.0 unx    13955 b- defN 24-Mar-15 07:24 mindflow/geometry/geometry_td.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-15 07:24 mindflow/geometry/shapes/__init__.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-Mar-15 07:24 mindflow/geometry/shapes/adapter.py
+-rw-r--r--  2.0 unx     2708 b- defN 24-Mar-15 07:24 mindflow/geometry/shapes/pentagon.py
+-rw-r--r--  2.0 unx     2617 b- defN 24-Mar-15 07:24 mindflow/geometry/shapes/polygon.py
+-rw-r--r--  2.0 unx     7023 b- defN 24-Mar-15 07:24 mindflow/geometry/shapes/rotating.py
+-rw-r--r--  2.0 unx     3162 b- defN 24-Mar-15 07:24 mindflow/geometry/shapes/shapes.py
+-rw-r--r--  2.0 unx     6650 b- defN 24-Mar-15 07:24 mindflow/geometry/shapes/simplex.py
+-rw-r--r--  2.0 unx      926 b- defN 24-Mar-15 07:24 mindflow/loss/__init__.py
+-rw-r--r--  2.0 unx    14261 b- defN 24-Mar-15 07:24 mindflow/loss/losses.py
+-rw-r--r--  2.0 unx      804 b- defN 24-Mar-15 07:24 mindflow/operators/__init__.py
+-rw-r--r--  2.0 unx     4635 b- defN 24-Mar-15 07:24 mindflow/operators/derivatives.py
+-rw-r--r--  2.0 unx     1056 b- defN 24-Mar-15 07:24 mindflow/pde/__init__.py
+-rw-r--r--  2.0 unx     8546 b- defN 24-Mar-15 07:24 mindflow/pde/flow_with_loss.py
+-rw-r--r--  2.0 unx    16271 b- defN 24-Mar-15 07:24 mindflow/pde/pde_with_loss.py
+-rw-r--r--  2.0 unx      788 b- defN 24-Mar-15 07:24 mindflow/pde/sympy2mindspore/__init__.py
+-rw-r--r--  2.0 unx     3212 b- defN 24-Mar-15 07:24 mindflow/pde/sympy2mindspore/parse_sympy.py
+-rw-r--r--  2.0 unx     6445 b- defN 24-Mar-15 07:24 mindflow/pde/sympy2mindspore/pde_node.py
+-rw-r--r--  2.0 unx     7632 b- defN 24-Mar-15 07:24 mindflow/pde/sympy2mindspore/sympy_translation.py
+-rw-r--r--  2.0 unx      892 b- defN 24-Mar-15 07:24 mindflow/utils/__init__.py
+-rw-r--r--  2.0 unx     5419 b- defN 24-Mar-15 07:24 mindflow/utils/check_func.py
+-rw-r--r--  2.0 unx     1892 b- defN 24-Mar-15 07:24 mindflow/utils/load_config.py
+-rw-r--r--  2.0 unx     1503 b- defN 24-Mar-15 07:24 mindflow/utils/log_utils.py
+-rw-r--r--  2.0 unx      392 b- defN 24-Mar-15 07:24 mindflow/utils/time_utils.py
+-rw-r--r--  2.0 unx      660 b- defN 24-Mar-15 07:24 mindflow_gpu-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-15 07:24 mindflow_gpu-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Mar-15 07:24 mindflow_gpu-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     9855 b- defN 24-Mar-15 07:24 mindflow_gpu-0.2.0.dist-info/RECORD
+106 files, 570408 bytes uncompressed, 150796 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -9,35 +9,44 @@
 
 Filename: mindflow/cell/activation.py
 Comment: 
 
 Filename: mindflow/cell/basic_block.py
 Comment: 
 
+Filename: mindflow/cell/unet2d.py
+Comment: 
+
 Filename: mindflow/cell/utils.py
 Comment: 
 
 Filename: mindflow/cell/neural_operators/__init__.py
 Comment: 
 
 Filename: mindflow/cell/neural_operators/dft.py
 Comment: 
 
-Filename: mindflow/cell/neural_operators/fno1d.py
+Filename: mindflow/cell/neural_operators/fno.py
 Comment: 
 
-Filename: mindflow/cell/neural_operators/fno2d.py
+Filename: mindflow/cell/neural_operators/kno1d.py
+Comment: 
+
+Filename: mindflow/cell/neural_operators/kno2d.py
 Comment: 
 
 Filename: mindflow/cell/neural_operators/m2k.py
 Comment: 
 
 Filename: mindflow/cell/neural_operators/pdenet.py
 Comment: 
 
+Filename: mindflow/cell/neural_operators/percnn.py
+Comment: 
+
 Filename: mindflow/cell/transformer/__init__.py
 Comment: 
 
 Filename: mindflow/cell/transformer/layer.py
 Comment: 
 
 Filename: mindflow/cell/transformer/vit.py
@@ -138,23 +147,35 @@
 
 Filename: mindflow/cfd/space_solver/reconstructor/__init__.py
 Comment: 
 
 Filename: mindflow/cfd/space_solver/reconstructor/base.py
 Comment: 
 
+Filename: mindflow/cfd/space_solver/reconstructor/weno3.py
+Comment: 
+
 Filename: mindflow/cfd/space_solver/reconstructor/weno5.py
 Comment: 
 
+Filename: mindflow/cfd/space_solver/reconstructor/weno7.py
+Comment: 
+
 Filename: mindflow/cfd/space_solver/riemann_computer/__init__.py
 Comment: 
 
 Filename: mindflow/cfd/space_solver/riemann_computer/base.py
 Comment: 
 
+Filename: mindflow/cfd/space_solver/riemann_computer/hllc.py
+Comment: 
+
+Filename: mindflow/cfd/space_solver/riemann_computer/roe.py
+Comment: 
+
 Filename: mindflow/cfd/space_solver/riemann_computer/rusanov.py
 Comment: 
 
 Filename: mindflow/cfd/space_solver/riemann_computer/rusanov_net.py
 Comment: 
 
 Filename: mindflow/common/__init__.py
@@ -219,14 +240,17 @@
 
 Filename: mindflow/geometry/shapes/adapter.py
 Comment: 
 
 Filename: mindflow/geometry/shapes/pentagon.py
 Comment: 
 
+Filename: mindflow/geometry/shapes/polygon.py
+Comment: 
+
 Filename: mindflow/geometry/shapes/rotating.py
 Comment: 
 
 Filename: mindflow/geometry/shapes/shapes.py
 Comment: 
 
 Filename: mindflow/geometry/shapes/simplex.py
@@ -270,20 +294,26 @@
 
 Filename: mindflow/utils/check_func.py
 Comment: 
 
 Filename: mindflow/utils/load_config.py
 Comment: 
 
-Filename: mindflow_gpu-0.1.0rc1.dist-info/METADATA
+Filename: mindflow/utils/log_utils.py
+Comment: 
+
+Filename: mindflow/utils/time_utils.py
+Comment: 
+
+Filename: mindflow_gpu-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: mindflow_gpu-0.1.0rc1.dist-info/WHEEL
+Filename: mindflow_gpu-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: mindflow_gpu-0.1.0rc1.dist-info/top_level.txt
+Filename: mindflow_gpu-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mindflow_gpu-0.1.0rc1.dist-info/RECORD
+Filename: mindflow_gpu-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mindflow/cell/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 Huawei Technologies Co., Ltd
+# Copyright 2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,13 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """init"""
 from .activation import get_activation
 from .basic_block import LinearBlock, ResBlock, InputScale, FCSequential, MultiScaleFCSequential
-from .neural_operators import FNO1D, FNO2D, PDENet
+from .neural_operators import FNO1D, FNO2D, FNO3D, KNO1D, KNO2D, PDENet, PeRCNN
 from .transformer import ViT
+from .unet2d import UNet2D
 
-__all__ = ['FNO1D', 'FNO2D', 'ViT', 'PDENet']
+__all__ = ['FNO1D', 'FNO2D', 'FNO3D', 'KNO1D', 'KNO2D', 'ViT', 'PDENet', 'UNet2D', 'PeRCNN']
 __all__.extend(activation.__all__)
 __all__.extend(basic_block.__all__)
```

## mindflow/cell/activation.py

```diff
@@ -82,18 +82,18 @@
 
 
 def get_activation(name):
     """
     Gets the activation function.
 
     Args:
-        name (Union[str, None]): The name of the activation function. If name was None, it would return None.
+        name (Union[str, None]): The name of the activation function. If name was ``None``, it would return ``None``.
 
     Returns:
-        Function, the activation function.
+        Function(mindspore.cell), the activation function.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindflow.cell import get_activation
```

## mindflow/cell/basic_block.py

```diff
@@ -43,20 +43,22 @@
     r"""
     The LinearBlock. Applies a linear transformation to the incoming data.
 
     Args:
         in_channels (int): The number of channels in the input space.
         out_channels (int): The number of channels in the output space.
         weight_init (Union[Tensor, str, Initializer, numbers.Number]): The trainable weight_init parameter. The dtype
-            is same as input `input` . For the values of str, refer to the function `initializer`. Default: "normal".
+            is same as input `input` . For the values of str, refer to the function `mindspore.common.initializer`.
+            Default: ``"normal"``.
         bias_init (Union[Tensor, str, Initializer, numbers.Number]): The trainable bias_init parameter. The dtype is
-            same as input `input` . The values of str refer to the function `initializer`. Default: "zeros".
-        has_bias (bool): Specifies whether the layer uses a bias vector. Default: True.
+            same as input `input` . The values of str refer to the function `mindspore.common.initializer`.
+            Default: ``"zeros"``.
+        has_bias (bool): Specifies whether the layer uses a bias vector. Default: ``True``.
         activation (Union[str, Cell, Primitive, None]): activate function applied to the output of the fully connected
-            layer. Default: None.
+            layer. Default: ``None``.
 
     Inputs:
         - **input** (Tensor) - Tensor of shape :math:`(*, in\_channels)`.
 
     Outputs:
         Tensor of shape :math:`(*, out\_channels)`.
 
@@ -101,21 +103,21 @@
     r"""
     The ResBlock of dense layer.
 
     Args:
         in_channels (int): The number of channels in the input space.
         out_channels (int): The number of channels in the output space.
         weight_init (Union[Tensor, str, Initializer, numbers.Number]): The trainable weight_init parameter. The dtype
-            is same as input x. The values of str refer to the function `initializer`. Default: 'normal'.
+            is same as input x. The values of str refer to the function `initializer`. Default: ``'normal'``.
         bias_init (Union[Tensor, str, Initializer, numbers.Number]): The trainable bias_init parameter. The dtype is
-            same as input x. The values of str refer to the function `initializer`. Default: 'zeros'.
-        has_bias (bool): Specifies whether the layer uses a bias vector. Default: True.
+            same as input x. The values of str refer to the function `initializer`. Default: ``'zeros'``.
+        has_bias (bool): Specifies whether the layer uses a bias vector. Default: ``True``.
         activation (Union[str, Cell, Primitive, None]): activate function applied to the output of the dense layer.
-            Default: None.
-        weight_norm (bool): Whether to compute the sum of squares of weight. Default: False.
+            Default: ``None``.
+        weight_norm (bool): Whether to compute the sum of squares of weight. Default: ``False``.
 
     Inputs:
         - **input** (Tensor) - Tensor of shape :math:`(*, in\_channels)`.
 
     Outputs:
         Tensor of shape :math:`(*, out\_channels)`.
 
@@ -156,15 +158,16 @@
                              "out_channels: {}".format(in_channels, out_channels))
         self.dense = LinearBlock(in_channels,
                                  out_channels,
                                  weight_init=weight_init,
                                  bias_init=bias_init,
                                  has_bias=has_bias,
                                  activation=None)
-        self.activation = get_activation(activation) if isinstance(activation, str) else activation
+        self.activation = get_activation(activation) if isinstance(
+            activation, str) else activation
         if activation is not None and not isinstance(self.activation, (nn.Cell, ops.Primitive)):
             raise TypeError(
                 "The activation must be str or Cell or Primitive,"" but got {}.".format(type(activation)))
         if not activation:
             self.activation = ops.Identity()
 
     def construct(self, x):
@@ -177,29 +180,29 @@
     bound = 1 / math.sqrt(fan_in) if fan_in > 0 else 0
     out = np.random.uniform(-bound, bound, fan_out)
     return Tensor(out, mstype.float32)
 
 
 class InputScale(nn.Cell):
     r"""
-    Scale the input value to specified region.
+    Scale the input value to specified region based on :math:`(x_i - input\_center)*input\_scale`
 
     Args:
-        input_scale (list): The scale factor of input x/y/t.
-        input_center (Union[list, None]): Center position of coordinate translation. Default: None.
+        input_scale (list): The scale factor of input.
+        input_center (Union[list, None]): Position offset of coordinate translation. Default: ``None``.
 
     Inputs:
         - **input** (Tensor) - Tensor of shape :math:`(*, channels)`.
 
     Outputs:
         Tensor of shape :math:`(*, channels)`.
 
     Raises:
         TypeError: If `input_scale` is not a list.
-        TypeError: If `input_center` is not a list or None.
+        TypeError: If `input_center` is not a list or ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindflow.cell import InputScale
@@ -245,23 +248,23 @@
     A sequential container of the dense layers, dense layers are added to the container sequentially.
 
     Args:
         in_channels (int): The number of channels in the input space.
         out_channels (int): The number of channels in the output space.
         layers (int): The total number of layers, include input/hidden/output layers.
         neurons (int): The number of neurons of hidden layers.
-        residual (bool): full-connected of residual block for the hidden layers. Default: True.
+        residual (bool): full-connected of residual block for the hidden layers. Default: ``True``.
         act (Union[str, Cell, Primitive, None]): activate function applied to the output of the fully connected layer,
-            eg. 'ReLU'.Default: "sin".
+            eg. ``'ReLU'``.Default: ``"sin"``.
         weight_init (Union[Tensor, str, Initializer, numbers.Number]): The trainable weight_init parameter. The dtype
-            is same as input x. The values of str refer to the function `initializer`. Default: 'normal'.
-        has_bias (bool): Specifies whether the layer uses a bias vector. Default: True.
+            is same as input x. The values of str refer to the function `initializer`. Default: ``'normal'``.
+        has_bias (bool): Specifies whether the layer uses a bias vector. Default: ``True``.
         bias_init (Union[Tensor, str, Initializer, numbers.Number]): The trainable bias_init parameter. The dtype
-            is same as input x. The values of str refer to the function `initializer`. Default: 'default'.
-        weight_norm (bool): Whether to compute the sum of squares of weight. Default: False.
+            is same as input x. The values of str refer to the function `initializer`. Default: ``'default'``.
+        weight_norm (bool): Whether to compute the sum of squares of weight. Default: ``False``.
 
     Inputs:
         - **input** (Tensor) - Tensor of shape :math:`(*, in\_channels)`.
 
     Outputs:
         Tensor of shape :math:`(*, out\_channels)`.
 
@@ -313,21 +316,26 @@
         self.network = nn.SequentialCell()
         self._create_networks()
 
     def construct(self, x):
         return self.network(x)
 
     def _create_networks(self):
-        self._add_linear_block(self.in_channels, self.neurons, weight_init=self.weight_init)
-        self._add_hidden_blocks(self.neurons, self.neurons, weight_init=self.weight_init)
-        self._add_linear_block(self.neurons, self.out_channels, weight_init=self.weight_init, is_out_net=True)
+        self._add_linear_block(
+            self.in_channels, self.neurons, weight_init=self.weight_init)
+        self._add_hidden_blocks(
+            self.neurons, self.neurons, weight_init=self.weight_init)
+        self._add_linear_block(
+            self.neurons, self.out_channels, weight_init=self.weight_init, is_out_net=True)
 
     def _check_params(self):
-        check_param_type(self.layers, "layers", data_type=int, exclude_type=bool)
-        check_param_type(self.neurons, "neurons", data_type=int, exclude_type=bool)
+        check_param_type(self.layers, "layers",
+                         data_type=int, exclude_type=bool)
+        check_param_type(self.neurons, "neurons",
+                         data_type=int, exclude_type=bool)
         check_param_type(self.residual, "residual", data_type=bool)
         if self.layers < 3:
             raise ValueError(
                 "FCSequential have at least 3 layers, but got layers: {}".format(self.layers))
 
     def _add_linear_block(self, in_channels, out_channels, weight_init, is_out_net=False):
         act = _get_out_net_activation(is_out_net, self.act)
@@ -366,44 +374,44 @@
     The multi-scale fully conneted network.
 
     Args:
         in_channels (int): The number of channels in the input space.
         out_channels (int): The number of channels in the output space.
         layers (int): The total number of layers, include input/hidden/output layers.
         neurons (int): The number of neurons of hidden layers.
-        residual (bool): full-connected of residual block for the hidden layers. Default: True.
+        residual (bool): full-connected of residual block for the hidden layers. Default: ``True``.
         act (Union[str, Cell, Primitive, None]): activate function applied to the output of the fully connected layer,
-            eg. 'ReLU'.Default: "sin".
+            eg. ``'ReLU'``.Default: ``"sin"``.
         weight_init (Union[Tensor, str, Initializer, numbers.Number]): The trainable weight_init parameter. The dtype
-            is same as input x. The values of str refer to the function `initializer`. Default: 'normal'.
-        weight_norm (bool): Whether to compute the sum of squares of weight. Default: False.
-        has_bias (bool): Specifies whether the layer uses a bias vector. Default: True.
+            is same as `input`. The values of str refer to the function `initializer`. Default: ``'normal'``.
+        weight_norm (bool): Whether to compute the sum of squares of weight. Default: ``False``.
+        has_bias (bool): Specifies whether the layer uses a bias vector. Default: ``True``.
         bias_init (Union[Tensor, str, Initializer, numbers.Number]): The trainable bias_init parameter. The dtype
-            is same as input x. The values of str refer to the function `initializer`. Default: 'default'.
-        num_scales (int): The subnet number of multi-scale network. Default: 4
-        amp_factor (Union[int, float]): The amplification factor of input. Default: 1.0
-        scale_factor (Union[int, float]): The base scale factor. Default: 2.0
-        input_scale (Union[list, None]): The scale factor of input x/y/t. If not None, the inputs will be scaled before
-            set in the network. Default: None.
-        input_center (Union[list, None]): Center position of coordinate translation. If not None, the inputs will be
-            translated before set in the network. Default: None.
+            is same as `input`. The values of str refer to the function `initializer`. Default: ``'default'``.
+        num_scales (int): The subnet number of multi-scale network. Default: ``4``.
+        amp_factor (Union[int, float]): The amplification factor of input. Default: ``1.0``.
+        scale_factor (Union[int, float]): The base scale factor. Default: ``2.0``.
+        input_scale (Union[list, None]): The scale factor of input x/y/t. If not ``None``, the inputs will be
+            scaled before set in the network. Default: ``None``.
+        input_center (Union[list, None]): Center position of coordinate translation. If not ``None``, the inputs will be
+            translated before set in the network. Default: ``None``.
         latent_vector (Union[Parameter, None]): Trainable papameter which will be concated will the sampling inputs
-            and updated during training. Default: None.
+            and updated during training. Default: ``None``.
 
     Inputs:
         - **input** (Tensor) - Tensor of shape :math:`(*, in\_channels)`.
 
     Outputs:
         Tensor of shape :math:`(*, out\_channels)`.
 
     Raises:
         TypeError: If `num_scales` is not an int.
         TypeError: If `amp_factor` is neither int nor float.
         TypeError: If `scale_factor` is neither int nor float.
-        TypeError: If `latent_vector` is neither a Parameter nor None.
+        TypeError: If `latent_vector` is neither a Parameter nor ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindflow.cell import MultiScaleFCSequential
@@ -487,15 +495,15 @@
 
     def construct(self, x):
         x = self.input_scale(x)
         if self.latent_vector is not None:
             batch_size = x.shape[0]
             latent_vectors = self.latent_vector.view(self.num_scenarios, 1,
                                                      self.latent_size).repeat(
-                                                        batch_size // self.num_scenarios,
-                                                        axis=1).view((-1, self.latent_size))
+                batch_size // self.num_scenarios,
+                axis=1).view((-1, self.latent_size))
             x = self.concat((x, latent_vectors))
         out = 0
         for i in range(self.num_scales):
             x_s = x * self.scale_coef[i]
             out = out + self.cast(self.cell_list[i](x_s), mstype.float32)
         return out
```

## mindflow/cell/utils.py

```diff
@@ -14,15 +14,28 @@
 # limitations under the License.
 # ============================================================================
 '''
 
 import numpy as np
 import mindspore.ops.operations as P
 
-__all__ = ['to_2tuple', 'unpatchify', 'patchify', 'get_2d_sin_cos_pos_embed']
+__all__ = ['to_2tuple', 'to_3tuple', 'unpatchify',
+           'patchify', 'get_2d_sin_cos_pos_embed']
+
+
+def to_3tuple(t):
+    """
+    Args:
+        t (Union[int, tuple(int)]): The grid height and width.
+
+    Returns:
+        Same as input or a tuple as (t,t,t).
+
+    """
+    return t if isinstance(t, tuple) else (t, t, t)
 
 
 def to_2tuple(t):
     """
     Args:
         t (Union[int, tuple(int)]): The grid height and width.
 
@@ -30,21 +43,21 @@
         Same as input or a tuple as (t,t).
 
     """
     return t if isinstance(t, tuple) else (t, t)
 
 
 def get_2d_sin_cos_pos_embed(embed_dim, grid_size):
-    """
+    r"""
     Args:
         embed_dim (int): The output dimension for each position.
         grid_size (tuple(int)): The grid height and width.
 
     Returns:
-        The numpy array with shape of (1, grid_height*grid_width, embed_dim)
+        The numpy array with shape of :math:`(1, grid\_height*grid\_width, embed\_dim)`
 
     """
     grid_size = to_2tuple(grid_size)
     grid_height = np.arange(grid_size[0], dtype=np.float32)
     grid_width = np.arange(grid_size[1], dtype=np.float32)
     grid = np.meshgrid(grid_width, grid_height)  # here w goes first
     grid = np.stack(grid, axis=0)
@@ -52,39 +65,41 @@
     grid = grid.reshape([2, 1, grid_size[0], grid_size[1]])
     pos_embed = get_2d_sin_cos_pos_embed_from_grid(embed_dim, grid)
     pos_embed = np.expand_dims(pos_embed, 0)
     return pos_embed
 
 
 def get_2d_sin_cos_pos_embed_from_grid(embed_dim, grid):
-    """
+    r"""
     use half of dimensions to encode grid_height
 
     Args:
         embed_dim (int): output dimension for each position.
         grid (int): a numpy array of positions to be encoded: size (M,).
 
     Returns:
-        The numpy array with shape of (M/2, embed_dim)
+        The numpy array with shape of :math:`(M/2, embed\_dim)`
     """
-    emb_height = get_1d_sin_cos_pos_embed_from_grid(embed_dim // 2, grid[0])  # (H*W, D/2)
-    emb_width = get_1d_sin_cos_pos_embed_from_grid(embed_dim // 2, grid[1])  # (H*W, D/2)
+    emb_height = get_1d_sin_cos_pos_embed_from_grid(
+        embed_dim // 2, grid[0])  # (H*W, D/2)
+    emb_width = get_1d_sin_cos_pos_embed_from_grid(
+        embed_dim // 2, grid[1])  # (H*W, D/2)
 
     emb = np.concatenate([emb_height, emb_width], axis=1)  # (H*W, D)
     return emb
 
 
 def get_1d_sin_cos_pos_embed_from_grid(embed_dim, pos):
-    """
+    r"""
     Args:
         embed_dim (int): output dimension for each position.
         pos (int): a numpy array of positions to be encoded: size (M,).
 
     Returns:
-        The numpy array with shape of (M, embed_dim)
+        The numpy array with shape of :math:`(M, embed\_dim)`
     """
     omega = np.arange(embed_dim // 2, dtype=np.float)
     omega /= embed_dim / 2.
     omega = 1. / 10000 ** omega  # (D/2,)
 
     pos = pos.reshape(-1)  # (M,)
     out = np.einsum('m,d->md', pos, omega)  # (M, D/2), outer product
@@ -96,18 +111,18 @@
     return emb
 
 
 def patchify(label, patch_size=16):
     """
     Args:
         label (Union[int, float]): output dimension for each position.
-        patch_size (int): The patch size of image. Default: 16.
+        patch_size (int): The patch size of image. Default: ``16``.
 
     Returns:
-        The numpy array with new shape of (H, W).
+        The numpy array with new shape of :math:`(H, W)`.
     """
     label_shape = label.shape
     label = np.reshape(label, (label_shape[0] // patch_size,
                                patch_size,
                                label_shape[1] // patch_size,
                                patch_size,
                                label_shape[2]))
@@ -123,15 +138,15 @@
     Args:
         labels (Union[int, float]): output dimension for each position.
         img_size (tuple(int)): Input image size. Default (192, 384).
         patch_size (int): The patch size of image. Default: 16.
         nchw (bool): If True, the unpatchify shape contains N, C, H, W.
 
     Returns:
-        The tensor with shape of (N, H, W, C).
+        The tensor with shape of :math:`(N, H, W, C)`.
     """
     label_shape = labels.shape
     output_dim = label_shape[-1] // (patch_size * patch_size)
     labels = P.Reshape()(labels, (label_shape[0],
                                   img_size[0] // patch_size,
                                   img_size[1] // patch_size,
                                   patch_size,
```

## mindflow/cell/neural_operators/__init__.py

```diff
@@ -1,22 +1,24 @@
-# Copyright 2022 Huawei Technologies Co., Ltd
+# Copyright 2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """init"""
-from .fno1d import FNO1D
-from .fno2d import FNO2D
+from .fno import FNOBlocks, FNO1D, FNO2D, FNO3D
+from .kno1d import KNO1D
+from .kno2d import KNO2D
 from .pdenet import PDENet
+from .percnn import PeRCNN
 
-__all__ = ["FNO1D", "FNO2D", "PDENet"]
+__all__ = ["FNOBlocks", "FNO1D", "FNO2D", "FNO3D", "KNO1D", "KNO2D", "PDENet", "PeRCNN"]
 
 __all__.sort()
```

## mindflow/cell/neural_operators/dft.py

```diff
@@ -1,30 +1,31 @@
 ''''
-# Copyright 2022 Huawei Technologies Co., Ltd
+# Copyright 2023 Huawei Technologies Co., Ltd
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 '''
-
 import numpy as np
 from scipy.linalg import dft
 
 import mindspore
-from mindspore import nn, ops, Tensor
+import mindspore.common.dtype as mstype
+from mindspore import nn, ops, Tensor, Parameter
 from mindspore.common.initializer import Zero
+from mindspore.ops import operations as P
 
 from ...utils.check_func import check_param_no_greater, check_param_value, check_param_type, check_param_even
 
 
 class DFT1d(nn.Cell):
     '''One dimensional Discrete Fourier Transformation'''
 
@@ -33,14 +34,15 @@
 
         self.n = n
         self.dft_mat = dft(n, scale="sqrtn")
         self.modes = modes
         self.last_index = last_index
         self.inv = inv
         self.idx = idx
+        self.compute_dtype = compute_dtype
 
         self.dft_mode_mat_upper = self.dft_mat[:, :modes]
         self.a_re_upper = Tensor(
             self.dft_mode_mat_upper.real, dtype=compute_dtype)
         self.a_im_upper = Tensor(
             self.dft_mode_mat_upper.imag, dtype=compute_dtype)
 
@@ -88,21 +90,23 @@
     def complex_matmul(self, x_re, x_im, a_re, a_im):
         y_re = ops.matmul(x_re, a_re) - ops.matmul(x_im, a_im)
         y_im = ops.matmul(x_im, a_re) + ops.matmul(x_re, a_im)
         return y_re, y_im
 
     def construct(self, x):
         x_re, x_im = x
-
+        x_re, x_im = P.Cast()(x_re, self.compute_dtype), P.Cast()(x_im, self.compute_dtype)
         if not self.inv:
             x_re, x_im = self.swap_axes(x_re, x_im)
-            y_re, y_im = self.complex_matmul(x_re=x_re, x_im=x_im, a_re=self.a_re_upper, a_im=self.a_im_upper)
+            y_re, y_im = self.complex_matmul(
+                x_re=x_re, x_im=x_im, a_re=self.a_re_upper, a_im=self.a_im_upper)
 
             if not self.last_index:
-                y_re2, y_im2 = self.complex_matmul(x_re=x_re, x_im=x_im, a_re=self.a_re_lower, a_im=self.a_im_lower)
+                y_re2, y_im2 = self.complex_matmul(
+                    x_re=x_re, x_im=x_im, a_re=self.a_re_lower, a_im=self.a_im_lower)
 
                 if self.n == self.modes * 2:
                     y_re = self.concat((y_re, y_re2))
                     y_im = self.concat((y_im, y_im2))
                 else:
                     dims = x_re.shape[:-1]
                     length = len(dims)
@@ -118,15 +122,16 @@
         x_re, x_im = self.swap_axes(x_re, x_im)
         y_re, y_im = self.complex_matmul(x_re=x_re[..., :self.modes], x_im=x_im[..., :self.modes],
                                          a_re=self.a_re_upper,
                                          a_im=self.a_im_upper)
         y_re, y_im = self.swap_axes(y_re, y_im)
 
         if self.last_index:
-            y_re_res, y_im_res = self.complex_matmul(x_re=x_re, x_im=x_im, a_re=self.a_re_res, a_im=-self.a_im_res)
+            y_re_res, y_im_res = self.complex_matmul(
+                x_re=x_re, x_im=x_im, a_re=self.a_re_res, a_im=-self.a_im_res)
         else:
             y_re_res, y_im_res = self.complex_matmul(x_re=x_re[..., -self.modes:], x_im=x_im[..., -self.modes:],
                                                      a_re=self.a_re_res, a_im=self.a_im_res)
 
         y_re_res, y_im_res = self.swap_axes(y_re_res, y_im_res)
         return y_re + y_re_res, y_im + y_im_res
 
@@ -159,14 +164,160 @@
 
 def _idftn(shape, modes, dim=None, compute_dtype=mindspore.float32):
     idftn_ = DFTn(shape=shape, modes=modes, dim=dim,
                   inv=True, compute_dtype=compute_dtype)
     return idftn_
 
 
+def dft3(shape, modes, dim=(-3, -2, -1), compute_dtype=mindspore.float32):
+    r"""
+    Calculate three-dimensional discrete Fourier transform. Corresponding to the rfftn operator in torch.
+
+    Args:
+        shape (tuple): Dimension of the input 'x'.
+        modes (tuple): The length of the output transform axis. The `modes` must be no greater than half of the
+            dimension of input 'x'.
+        dim (tuple): Dimensions to be transformed.
+        compute_dtype (mindspore.dtype): The type of input tensor. Default: mindspore.float32.
+
+    Inputs:
+        - **x** (Tensor, Tensor): The input data. It's 3-D tuple of Tensor. It's a complex,
+          including x real and imaginary. Tensor of shape :math:`(*, *)`.
+
+    Returns:
+        Complex tensor with the same shape of input x.
+
+    Raises:
+        TypeError: If `shape` is not a tuple.
+        ValueError: If the length of `shape` is no equal to 3.
+
+    Examples:
+        >>> import numpy as np
+        >>> from mindspore import Tensor, ops
+        >>> import mindspore.common.dtype as mstype
+        >>> from mindflow.cell.neural_operators.dft import dft3
+        >>> array = np.ones((6, 6, 6)) * np.arange(1, 7)
+        >>> x_re = Tensor(array, dtype=mstype.float32)
+        >>> x_im = x_re
+        >>> dft3_cell = dft3(shape=array.shape, modes=(2, 2, 2), compute_dtype=mstype.float32)
+        >>> ret, _ = dft3_cell((x_re, x_im))
+        >>> print(ret)
+        [[[ 5.1439293e+01 -2.0076393e+01]
+        [ 7.9796671e-08 -1.9494735e-08]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 9.0537789e-08  1.0553553e-07]
+        [ 3.3567730e-07  1.0368046e-07]]
+
+        [[ 4.7683722e-07 -3.1770034e-07]
+        [ 6.5267522e-15 -2.7775875e-15]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [-2.1755840e-15 -1.5215135e-15]
+        [ 3.6259736e-15 -4.0336615e-15]]
+
+        [[ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]]
+
+        [[ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]]
+
+        [[ 1.1920930e-07 -5.1619136e-08]
+        [-3.6259733e-16 -1.0747753e-15]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 3.6259733e-16 -1.8129867e-16]
+        [ 3.6259733e-16 -1.4373726e-15]]
+
+        [[ 5.9604650e-07 -2.5809570e-07]
+        [ 8.7023360e-15 -1.9812689e-15]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 0.0000000e+00  0.0000000e+00]
+        [ 2.9007787e-15  7.2519467e-16]
+        [ 8.7023360e-15 -1.7869532e-15]]]
+
+    """
+    check_param_type(shape, "shape", data_type=tuple)
+    check_param_type(modes, "modes", data_type=tuple)
+    check_param_value(len(shape), "shape length", 3)
+    check_param_value(len(modes), "modes length", 3)
+    check_param_even(shape, "shape")
+    check_param_no_greater(modes[0], "mode1", shape[0] // 2)
+    check_param_no_greater(modes[1], "mode2", shape[1] // 2)
+    check_param_no_greater(modes[2], "mode3", shape[2] // 2 + 1)
+    return _dftn(shape, modes, dim=dim, compute_dtype=compute_dtype)
+
+
+def idft3(shape, modes, dim=(-3, -2, -1), compute_dtype=mindspore.float32):
+    r"""
+    Calculate three-dimensional discrete Fourier transform. Corresponding to the irfftn operator in torch.
+
+    Args:
+        shape (tuple): Dimension of the input 'x'.
+        modes (tuple): The length of the output transform axis. The `modes` must be no greater than half of the
+            dimension of input 'x'.
+        dim (tuple): Dimensions to be transformed.
+        compute_dtype (mindspore.dtype): The type of input tensor. Default: mindspore.float32.
+
+    Inputs:
+        - **x** (Tensor, Tensor): The input data. It's 3-D tuple of Tensor. It's a complex, including x real and
+          imaginary. Tensor of shape :math:`(*, *)`.
+
+    Returns:
+        Complex tensor with the same shape of input x.
+
+    Raises:
+        TypeError: If `shape` is not a tuple.
+        ValueError: If the length of `shape` is no equal to 3.
+
+    Examples:
+        >>> import numpy as np
+        >>> from mindspore import Tensor, ops
+        >>> import mindspore.common.dtype as mstype
+        >>> from mindflow.cell.neural_operators.dft import idft3
+        >>> array = np.ones((2, 2, 2)) * np.arange(1, 3)
+        >>> x_re = Tensor(array, dtype=mstype.float32)
+        >>> x_im = ops.zeros_like(x_re)
+        >>> idft3_cell = idft3(shape=(6, 6, 6), modes=(2, 2, 2), compute_dtype=mstype.float32)
+        >>> ret, _ = idft3_cell((x_re, x_im))
+        >>> print(ret)
+        [[[ 5.44331074e+00  3.26598644e+00 -1.08866215e+00 -3.26598644e+00 -1.08866215e+00  3.26598644e+00]
+        [ 2.04124165e+00  2.04124165e+00  4.08248246e-01 -1.22474492e+00 -1.22474492e+00  4.08248365e-01]
+        [-6.80413842e-01 -1.22474492e+00 -6.80413783e-01  4.08248305e-01 9.52579379e-01  4.08248246e-01]
+        [ 0.00000000e+00 -2.30921616e-16 -2.30921616e-16  6.53092730e-32 2.30921616e-16  2.30921616e-16]
+        [-6.80413842e-01  4.08248246e-01  9.52579379e-01  4.08248305e-01 -6.80413783e-01 -1.22474492e+00]
+        [ 2.04124165e+00  4.08248365e-01 -1.22474492e+00 -1.22474492e+00 4.08248246e-01  2.04124165e+00]]
+        ......
+        [[ 2.04124165e+00  4.08248544e-01 -1.22474492e+00 -1.22474504e+00 4.08248186e-01  2.04124165e+00]
+        [ 1.02062082e+00  6.12372518e-01 -2.04124182e-01 -6.12372518e-01 -2.04124182e-01  6.12372518e-01]
+        [-5.10310411e-01 -5.10310411e-01 -1.02062061e-01  3.06186229e-01 3.06186229e-01 -1.02062091e-01]
+        [-7.21630050e-17 -1.29893429e-16 -7.21630183e-17  4.32978030e-17 1.01028220e-16  4.32978163e-17]
+        [-6.08337416e-08  4.08248246e-01  4.08248305e-01  3.65002428e-08 -4.08248246e-01 -4.08248305e-01]
+        [ 5.10310471e-01 -3.06186140e-01 -7.14434564e-01 -3.06186318e-01 5.10310352e-01  9.18558717e-01]]]
+
+    """
+    check_param_type(shape, "shape", data_type=tuple)
+    check_param_type(modes, "modes", data_type=tuple)
+    check_param_value(len(shape), "shape length", 3)
+    check_param_value(len(modes), "modes length", 3)
+    check_param_even(shape, "shape")
+    check_param_no_greater(modes[0], "mode1", shape[0] // 2)
+    check_param_no_greater(modes[1], "mode2", shape[1] // 2)
+    check_param_no_greater(modes[2], "mode3", shape[2] // 2 + 1)
+    return _idftn(shape, modes, dim=dim, compute_dtype=compute_dtype)
+
+
 def dft2(shape, modes, dim=(-2, -1), compute_dtype=mindspore.float32):
     """
     Calculate two-dimensional discrete Fourier transform. Corresponding to the rfft2 operator in torch.
 
     Args:
         shape (tuple): Dimension of the input 'x'.
         modes (tuple): The length of the output transform axis. The `modes` must be no greater than half of the
@@ -346,7 +497,227 @@
     check_param_type(shape, "shape", data_type=tuple)
     check_param_type(modes, "modes", data_type=int)
     check_param_value(len(shape), "shape length", 1)
     check_param_even(shape, "shape")
     check_param_no_greater(modes, "mode1", shape[0] // 2 + 1)
     modes = (modes,)
     return _idftn(shape, modes, dim=dim, compute_dtype=compute_dtype)
+
+
+class SpectralConvDft(nn.Cell):
+    """Base Class for Fourier Layer, including DFT, linear transform, and Inverse DFT"""
+
+    def __init__(self, in_channels, out_channels, n_modes, resolutions, compute_dtype=mstype.float32):
+        super().__init__()
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        if isinstance(n_modes, int):
+            n_modes = [n_modes]
+        self.n_modes = n_modes
+        if isinstance(resolutions, int):
+            resolutions = [resolutions]
+        self.resolutions = resolutions
+        if len(self.n_modes) != len(self.resolutions):
+            raise ValueError(
+                "The dimension of n_modes should be equal to that of resolutions, \
+                but got dimension of n_modes {} and dimension of resolutions {}".format(len(self.n_modes),
+                                                                                        len(self.resolutions)))
+        self.compute_dtype = compute_dtype
+
+    def construct(self, x: Tensor):
+        raise NotImplementedError()
+
+    def _einsum(self, inputs, weights):
+        weights = weights.expand_dims(0)
+        inputs = inputs.expand_dims(2)
+        out = inputs * weights
+        return out.sum(1)
+
+
+class SpectralConv1dDft(SpectralConvDft):
+    """1D Fourier Layer. It does DFT, linear transform, and Inverse DFT."""
+
+    def __init__(self, in_channels, out_channels, n_modes, resolutions, compute_dtype=mstype.float32):
+        super().__init__(in_channels, out_channels, n_modes, resolutions)
+        self._scale = (1. / (self.in_channels * self.out_channels))
+        w_re = Tensor(self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0]),
+                      dtype=mstype.float32)
+        w_im = Tensor(self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0]),
+                      dtype=mstype.float32)
+        self._w_re = Parameter(w_re, requires_grad=True)
+        self._w_im = Parameter(w_im, requires_grad=True)
+        self._dft1_cell = dft1(shape=(self.resolutions[0],), modes=self.n_modes[0], compute_dtype=self.compute_dtype)
+        self._idft1_cell = idft1(shape=(self.resolutions[0],), modes=self.n_modes[0], compute_dtype=self.compute_dtype)
+
+    def construct(self, x: Tensor):
+        x_re = x
+        x_im = ops.zeros_like(x_re)
+        x_ft_re, x_ft_im = self._dft1_cell((x_re, x_im))
+        w_re = P.Cast()(self._w_re, self.compute_dtype)
+        w_im = P.Cast()(self._w_im, self.compute_dtype)
+        out_ft_re = self._einsum(x_ft_re[:, :, :self.n_modes[0]], w_re) - self._einsum(x_ft_im[:, :, :self.n_modes[0]],
+                                                                                       w_im)
+        out_ft_im = self._einsum(x_ft_re[:, :, :self.n_modes[0]], w_im) + self._einsum(x_ft_im[:, :, :self.n_modes[0]],
+                                                                                       w_re)
+
+        x, _ = self._idft1_cell((out_ft_re, out_ft_im))
+
+        return x
+
+
+class SpectralConv2dDft(SpectralConvDft):
+    """2D Fourier Layer. It does DFT, linear transform, and Inverse DFT."""
+
+    def __init__(self, in_channels, out_channels, n_modes, resolutions, compute_dtype=mstype.float32):
+        super().__init__(in_channels, out_channels, n_modes, resolutions)
+        self._scale = (1. / (self.in_channels * self.out_channels))
+        w_re1 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1]),
+            dtype=self.compute_dtype)
+        w_im1 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1]),
+            dtype=self.compute_dtype)
+        w_re2 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1]),
+            dtype=self.compute_dtype)
+        w_im2 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1]),
+            dtype=self.compute_dtype)
+
+        self._w_re1 = Parameter(w_re1, requires_grad=True)
+        self._w_im1 = Parameter(w_im1, requires_grad=True)
+        self._w_re2 = Parameter(w_re2, requires_grad=True)
+        self._w_im2 = Parameter(w_im2, requires_grad=True)
+
+        self._dft2_cell = dft2(shape=(self.resolutions[0], self.resolutions[1]),
+                               modes=(self.n_modes[0], self.n_modes[1]), compute_dtype=self.compute_dtype)
+        self._idft2_cell = idft2(shape=(self.resolutions[0], self.resolutions[1]),
+                                 modes=(self.n_modes[0], self.n_modes[1]), compute_dtype=self.compute_dtype)
+        self._mat = Tensor(shape=(1, self.out_channels, self.resolutions[1] - 2 * self.n_modes[0], self.n_modes[1]),
+                           dtype=self.compute_dtype, init=Zero())
+        self._concat = ops.Concat(-2)
+
+    def construct(self, x: Tensor):
+        x_re = x
+        x_im = ops.zeros_like(x_re)
+        x_ft_re, x_ft_im = self._dft2_cell((x_re, x_im))
+
+        out_ft_re1 = self._einsum(x_ft_re[:, :, :self.n_modes[0], :self.n_modes[1]], self._w_re1) - self._einsum(
+            x_ft_im[:, :, :self.n_modes[0], :self.n_modes[1]], self._w_im1)
+        out_ft_im1 = self._einsum(x_ft_re[:, :, :self.n_modes[0], :self.n_modes[1]], self._w_im1) + self._einsum(
+            x_ft_im[:, :, :self.n_modes[0], :self.n_modes[1]], self._w_re1)
+
+        out_ft_re2 = self._einsum(x_ft_re[:, :, -self.n_modes[0]:, :self.n_modes[1]], self._w_re2) - self._einsum(
+            x_ft_im[:, :, -self.n_modes[0]:, :self.n_modes[1]], self._w_im2)
+        out_ft_im2 = self._einsum(x_ft_re[:, :, -self.n_modes[0]:, :self.n_modes[1]], self._w_im2) + self._einsum(
+            x_ft_im[:, :, -self.n_modes[0]:, :self.n_modes[1]], self._w_re2)
+
+        batch_size = x.shape[0]
+        mat = self._mat.repeat(batch_size, 0)
+        out_re = self._concat((out_ft_re1, mat, out_ft_re2))
+        out_im = self._concat((out_ft_im1, mat, out_ft_im2))
+
+        x, _ = self._idft2_cell((out_re, out_im))
+
+        return x
+
+
+class SpectralConv3dDft(SpectralConvDft):
+    """3D Fourier layer. It does DFT, linear transform, and Inverse DFT."""
+
+    def __init__(self, in_channels, out_channels, n_modes, resolutions, compute_dtype=mstype.float32):
+        super().__init__(in_channels, out_channels, n_modes, resolutions)
+        self._scale = (1 / (self.in_channels * self.out_channels))
+
+        w_re1 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1],
+                                         self.n_modes[2]), dtype=self.compute_dtype)
+        w_im1 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1],
+                                         self.n_modes[2]), dtype=self.compute_dtype)
+        w_re2 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1],
+                                         self.n_modes[2]), dtype=self.compute_dtype)
+        w_im2 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1],
+                                         self.n_modes[2]), dtype=self.compute_dtype)
+        w_re3 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1],
+                                         self.n_modes[2]), dtype=self.compute_dtype)
+        w_im3 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1],
+                                         self.n_modes[2]), dtype=self.compute_dtype)
+        w_re4 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1],
+                                         self.n_modes[2]), dtype=self.compute_dtype)
+        w_im4 = Tensor(
+            self._scale * np.random.rand(self.in_channels, self.out_channels, self.n_modes[0], self.n_modes[1],
+                                         self.n_modes[2]), dtype=self.compute_dtype)
+
+        self._w_re1 = Parameter(w_re1, requires_grad=True)
+        self._w_im1 = Parameter(w_im1, requires_grad=True)
+        self._w_re2 = Parameter(w_re2, requires_grad=True)
+        self._w_im2 = Parameter(w_im2, requires_grad=True)
+        self._w_re3 = Parameter(w_re3, requires_grad=True)
+        self._w_im3 = Parameter(w_im3, requires_grad=True)
+        self._w_re4 = Parameter(w_re4, requires_grad=True)
+        self._w_im4 = Parameter(w_im4, requires_grad=True)
+
+        self._dft3_cell = dft3(shape=(self.resolutions[0], self.resolutions[1], self.resolutions[2]),
+                               modes=(self.n_modes[0], self.n_modes[1], self.n_modes[2]),
+                               compute_dtype=self.compute_dtype)
+        self._idft3_cell = idft3(shape=(self.resolutions[0], self.resolutions[1], self.resolutions[2]),
+                                 modes=(self.n_modes[0], self.n_modes[1], self.n_modes[2]),
+                                 compute_dtype=self.compute_dtype)
+        self._mat_x = Tensor(
+            shape=(1, self.out_channels, self.resolutions[0] - 2 * self.n_modes[0], self.n_modes[1], self.n_modes[2]),
+            dtype=self.compute_dtype, init=Zero())
+        self._mat_y = Tensor(
+            shape=(1, self.out_channels, self.resolutions[0], self.resolutions[1] - 2 * self.n_modes[1],
+                   self.n_modes[2]),
+            dtype=self.compute_dtype, init=Zero())
+        self._concat = ops.Concat(-2)
+
+    def construct(self, x: Tensor):
+        x_re = x
+        x_im = ops.zeros_like(x_re)
+        x_ft_re, x_ft_im = self._dft3_cell((x_re, x_im))
+
+        out_ft_re1 = self._einsum(x_ft_re[:, :, :self.n_modes[0], :self.n_modes[1], :self.n_modes[2]],
+                                  self._w_re1) - self._einsum(x_ft_im[:, :, :self.n_modes[0], :self.n_modes[1],
+                                                                      :self.n_modes[2]], self._w_im1)
+        out_ft_im1 = self._einsum(x_ft_re[:, :, :self.n_modes[0], :self.n_modes[1], :self.n_modes[2]],
+                                  self._w_im1) + self._einsum(x_ft_im[:, :, :self.n_modes[0], :self.n_modes[1],
+                                                                      :self.n_modes[2]], self._w_re1)
+        out_ft_re2 = self._einsum(x_ft_re[:, :, -self.n_modes[0]:, :self.n_modes[1], :self.n_modes[2]],
+                                  self._w_re2) - self._einsum(x_ft_im[:, :, -self.n_modes[0]:, :self.n_modes[1],
+                                                                      :self.n_modes[2]], self._w_im2)
+        out_ft_im2 = self._einsum(x_ft_re[:, :, -self.n_modes[0]:, :self.n_modes[1], :self.n_modes[2]],
+                                  self._w_im2) + self._einsum(x_ft_im[:, :, -self.n_modes[0]:, :self.n_modes[1],
+                                                                      :self.n_modes[2]], self._w_re2)
+        out_ft_re3 = self._einsum(x_ft_re[:, :, :self.n_modes[0], -self.n_modes[1]:, :self.n_modes[2]],
+                                  self._w_re3) - self._einsum(x_ft_im[:, :, :self.n_modes[0], -self.n_modes[1]:,
+                                                                      :self.n_modes[2]], self._w_im3)
+        out_ft_im3 = self._einsum(x_ft_re[:, :, :self.n_modes[0], -self.n_modes[1]:, :self.n_modes[2]],
+                                  self._w_im3) + self._einsum(x_ft_im[:, :, :self.n_modes[0], -self.n_modes[1]:,
+                                                                      :self.n_modes[2]], self._w_re3)
+        out_ft_re4 = self._einsum(x_ft_re[:, :, -self.n_modes[0]:, -self.n_modes[1]:, :self.n_modes[2]],
+                                  self._w_re4) - self._einsum(x_ft_im[:, :, -self.n_modes[0]:, -self.n_modes[1]:,
+                                                                      :self.n_modes[2]], self._w_im4)
+        out_ft_im4 = self._einsum(x_ft_re[:, :, -self.n_modes[0]:, -self.n_modes[1]:, :self.n_modes[2]],
+                                  self._w_im4) + self._einsum(x_ft_im[:, :, -self.n_modes[0]:, -self.n_modes[1]:,
+                                                                      :self.n_modes[2]], self._w_re4)
+
+        batch_size = x.shape[0]
+        mat_x = self._mat_x.repeat(batch_size, 0)
+        mat_y = self._mat_y.repeat(batch_size, 0)
+
+        out_re1 = ops.concat((out_ft_re1, mat_x, out_ft_re2), -3)
+        out_im1 = ops.concat((out_ft_im1, mat_x, out_ft_im2), -3)
+
+        out_re2 = ops.concat((out_ft_re3, mat_x, out_ft_re4), -3)
+        out_im2 = ops.concat((out_ft_im3, mat_x, out_ft_im4), -3)
+        out_re = ops.concat((out_re1, mat_y, out_re2), -2)
+        out_im = ops.concat((out_im1, mat_y, out_im2), -2)
+        x, _ = self._idft3_cell((out_re, out_im))
+
+        return x
```

## mindflow/cell/neural_operators/pdenet.py

```diff
@@ -50,20 +50,20 @@
 
     Args:
         height (int): The height number of the input and output tensor of the PDE-Net.
         width (int): The width number of the input and output tensor of the PDE-Net.
         channels (int): The channel number of the input and output tensor of the PDE-Net.
         kernel_size (int): Specifies the height and width of the 2D convolution kernel.
         max_order (int): The max order of the PDE models.
-        dx (float): The spatial resolution of x dimension. Default: 0.01.
-        dy (float): The spatial resolution of y dimension. Default: 0.01.
-        dt (float): The time step of the PDE-Net. Default: 0.01.
-        periodic (bool): Specifies whether periodic pad is used with convolution kernels. Default: True.
-        enable_moment (bool): Specifies whether the convolution kernels are constrained by moments. Default: True.
-        if_fronzen (bool): Specifies whether the moment is frozen. Default: False.
+        dx (float): The spatial resolution of x dimension. Default: ``0.01``.
+        dy (float): The spatial resolution of y dimension. Default: ``0.01``.
+        dt (float): The time step of the PDE-Net. Default: ``0.01``.
+        periodic (bool): Specifies whether periodic pad is used with convolution kernels. Default: ``True``.
+        enable_moment (bool): Specifies whether the convolution kernels are constrained by moments. Default: ``True``.
+        if_fronzen (bool): Specifies whether the moment is frozen. Default: ``False``.
 
     Inputs:
         - **input** (Tensor) - Tensor of shape :math:`(batch\_size, channels, height, width)`.
 
     Outputs:
         Tensor, has the same shape as `input` with data type of float32.
```

## mindflow/cell/transformer/layer.py

```diff
@@ -180,23 +180,23 @@
 
 class Encoder(nn.Cell):
     r"""
      Encoder module with multi-layer stacked of `Block`, including multihead self attention and feedforward layer.
 
      Args:
           grid_size (tuple[int]): The grid_size size of input.
-          in_channels (int): The input feature size of input. Default: 3.
-          patch_size (int): The patch size of image. Default: 16.
+          in_channels (int): The input feature size of input. Default: ``3``.
+          patch_size (int): The patch size of image. Default: ``16``.
           depths (int): The encoder depth of encoder layer.
-          embed_dim (int): The encoder embedding dimension of encoder layer. Default: 768.
-          num_heads (int): The encoder heads' number of encoder layer. Default: 16.
-          mlp_ratio (int): The rate of mlp layer. Default: 4.
-          dropout_rate (float): The rate of dropout layer. Default: 1.0.
+          embed_dim (int): The encoder embedding dimension of encoder layer. Default: ``768``.
+          num_heads (int): The encoder heads' number of encoder layer. Default: ``16``.
+          mlp_ratio (int): The rate of mlp layer. Default: ``4``.
+          dropout_rate (float): The rate of dropout layer. Default: ``1.0``.
           compute_dtype (dtype): The data type for encoder, encoding_embedding, encoder and dense layer.
-                                Default: mstype.float16.
+                                Default: ``mstype.float16``.
 
      Inputs:
              - **input** (Tensor) - Tensor of shape :math:`(batch\_size, feature\_size, image\_height, image\_width)`.
 
      Outputs:
              - **output** (Tensor) - Tensor of shape :math:`(batch\_size, patchify\_size, embed\_dim)`.
              where patchify_size = (image_height * image_width) / (patch_size * patch_size).
@@ -266,18 +266,18 @@
     Decoder module with multi-layer stacked of `Block`, including multihead self attention and feedforward layer.
 
     Args:
         grid_size (tuple[int]): The grid_size size of input.
         depths (int): The decoder depth of decoder layer.
         embed_dim (int): The decoder embedding dimension of decoder layer.
         num_heads (int): The decoder heads' number of decoder layer.
-        mlp_ratio (int): The rate of mlp layer. Default: 4.
-        dropout_rate (float): The rate of dropout layer. Default: 1.0.
+        mlp_ratio (int): The rate of mlp layer. Default: ``4``.
+        dropout_rate (float): The rate of dropout layer. Default: ``1.0``.
         compute_dtype (dtype): The data type for encoder, decoding_embedding, decoder and dense layer.
-            Default: mstype.float16.
+            Default: ``mstype.float16``.
 
     Inputs:
         - **input** (Tensor) - Tensor of shape :math:`(batch\_size, patchify\_size, embed\_dim)`.
 
     Outputs:
         - **output** (Tensor) - Tensor of shape :math:`(batch\_size, patchify\_size, embed\_dim)`.
           where patchify_size = (image_height * image_width) / (patch_size * patch_size).
```

## mindflow/cell/transformer/vit.py

```diff
@@ -27,28 +27,28 @@
 
 
 class ViT(nn.Cell):
     r"""
     This module based on ViT backbone which including encoder, decoding_embedding, decoder and dense layer.
 
     Args:
-        image_size (tuple[int]): The image size of input. Default: (192, 384).
-        in_channels (int): The input feature size of input. Default: 7.
-        out_channels (int): The output feature size of output. Default: 3.
-        patch_size (int): The patch size of image. Default: 16.
-        encoder_depths (int): The encoder depth of encoder layer. Default: 12.
-        encoder_embed_dim (int): The encoder embedding dimension of encoder layer. Default: 768.
-        encoder_num_heads (int): The encoder heads' number of encoder layer. Default: 12.
-        decoder_depths (int): The decoder depth of decoder layer. Default: 8.
-        decoder_embed_dim (int): The decoder embedding dimension of decoder layer. Default: 512.
-        decoder_num_heads (int): The decoder heads' number of decoder layer. Default: 16.
-        mlp_ratio (int): The rate of mlp layer. Default: 4.
-        dropout_rate (float): The rate of dropout layer. Default: 1.0.
+        image_size (tuple[int]): The image size of input. Default: ``(192, 384)``.
+        in_channels (int): The input feature size of input. Default: ``7``.
+        out_channels (int): The output feature size of output. Default: ``3``.
+        patch_size (int): The patch size of image. Default: ``16``.
+        encoder_depths (int): The encoder depth of encoder layer. Default: ``12``.
+        encoder_embed_dim (int): The encoder embedding dimension of encoder layer. Default: ``768``.
+        encoder_num_heads (int): The encoder heads' number of encoder layer. Default: ``12``.
+        decoder_depths (int): The decoder depth of decoder layer. Default: ``8``.
+        decoder_embed_dim (int): The decoder embedding dimension of decoder layer. Default: ``512``.
+        decoder_num_heads (int): The decoder heads' number of decoder layer. Default: ``16``.
+        mlp_ratio (int): The rate of mlp layer. Default: ``4``.
+        dropout_rate (float): The rate of dropout layer. Default: ``1.0``.
         compute_dtype (dtype): The data type for encoder, decoding_embedding, decoder and dense layer.
-            Default: mstype.float16.
+            Default: ``mstype.float16``.
 
     Inputs:
         - **input** (Tensor) - Tensor of shape :math:`(batch\_size, feature\_size, image\_height, image\_width)`.
 
     Outputs:
         - **output** (Tensor) - Tensor of shape :math:`(batch\_size, patchify\_size, embed\_dim)`.
           where patchify_size = (image_height * image_width) / (patch_size * patch_size)
```

## mindflow/cfd/runtime.py

```diff
@@ -87,24 +87,24 @@
         """
         if not self.timestep:
             raise NotImplementedError()
         self.current_time += self.timestep
 
     def time_loop(self, pri_var):
         """
-        Weather to continue the simulation. When current time reaches end time or NAN value detected,
+        Weather to continue the simulation. When current time reaches end time or ``NAN`` value detected,
         return False.
 
         Args:
             pri_var (Tensor): The primitive variables.
 
         Returns:
             Bool. Weather to continue the simulation.
 
         Raises:
-            ValueError: If pri_var has NAN values.
+            ValueError: If `pri_var` has ``NAN`` values.
         """
         if mnp.isnan(pri_var).sum() > 0:
             raise ValueError('Nan value detected!')
         if self.timestep and self.timestep < self.eps:
             return False
         return self.current_time < self.end_time
```

## mindflow/cfd/simulator.py

```diff
@@ -26,15 +26,15 @@
 @jit_class
 class Simulator:
     r"""
     CFD Simulator. It is the top-level class in MindFlow CFD.
 
     Args:
         config (dict): The dict of parameters.
-        net_dict (dict): The dict of netwoks. Default: None.
+        net_dict (dict): The dict of netwoks. Default: ``None``.
 
     Supported Platforms:
         ``GPU``
 
     Examples:
         >>> from mindflow import cfd
         >>> config = {'mesh': {'dim': 1, 'nx': 100, 'gamma': 1.4, 'x_range': [0, 1], 'pad_size': 3},
```

## mindflow/cfd/utils.py

```diff
@@ -21,18 +21,18 @@
 
 def cal_con_var(pri_var, material):
     """
     Calculate conservative variables from primitive variables and material.
 
     Args:
         pri_var (Tensor): The primitive variables.
-        material (Material): Material of the fluid.
+        material (mindflow.cfd.Material): Material of the fluid.
 
     Returns:
-        Tensor, with the same shape as pri_var.
+        Tensor, with the same shape as `pri_var`.
 
     Supported Platforms:
         ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindspore import Tensor
@@ -56,18 +56,18 @@
 
 def cal_pri_var(con_var, material):
     """
     Calculate primitive variables from conservative variables and material.
 
     Args:
         con_var (Tensor): The conservative variables.
-        material (Material): Material of the fluid.
+        material (mindflow.cfd.Material): Material of the fluid.
 
     Returns:
-        Tensor, with the same shape as con_var.
+        Tensor, with the same shape as `con_var`.
 
     Supported Platforms:
         ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindspore import Tensor
@@ -100,15 +100,15 @@
         pri_var (Tensor): The primitive variables.
         axis (int): Axis of the flux.
 
     Supported Platforms:
         ``GPU``
 
     Returns:
-        Tensor, with the same shape as pri_var.
+        Tensor, with the same shape as `pri_var`.
 
     Examples:
         >>> import numpy as np
         >>> from mindspore import Tensor
         >>> from mindflow.utils import cal_pri_var, cal_flux
         >>> from mindflow import material
         >>> config =  {'type': 'IdealGas', 'heat_ratio': 1.4, 'specific_heat_ratio': 1.4, 'specific_gas_constant': 1.0}
```

## mindflow/cfd/visualization.py

```diff
@@ -9,25 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """visualization tools"""
+import os
+import stat
 import matplotlib.pyplot as plt
 import numpy as np
 
 
-def vis_1d(pri_var, file_name='vis.jpg'):
+def vis_1d(pri_var, file_name='vis.jpg', permission=stat.S_IREAD + stat.S_IWRITE):
     """
     Visualize the 1d flow field.
 
     Args:
         pri_var (Tensor): The primitive variables.
-        file_name (str): The name of the picture. Default: 'vis.jpg'.
+        file_name (str): The name of the picture. Default: ``'vis.jpg'``.
+        permission (int): The file permission. Default: ``stat.S_IREAD + stat.S_IWRITE``.
 
     Supported Platforms:
         ``GPU``
     """
     data = pri_var.asnumpy()
     nx = list(data.shape)[1]
     dx = 1 / nx
@@ -38,23 +41,25 @@
 
     ax[1].set_title = 'u'
     ax[1].plot(cell_centers, data[1, :, 0, 0])
 
     ax[2].set_title = 'p'
     ax[2].plot(cell_centers, data[4, :, 0, 0])
     plt.savefig(file_name)
+    os.chmod(file_name, permission)
 
 
-def vis_2d(pri_var, file_name='vis.jpg'):
+def vis_2d(pri_var, file_name='vis.jpg', permission=stat.S_IREAD + stat.S_IWRITE):
     """
     Visualize the 2d flow field.
 
     Args:
         pri_var (Tensor): The primitive variables.
-        file_name (str): The name of the picture. Default: 'vis.jpg'.
+        file_name (str): The name of the picture. Default: ``'vis.jpg'``.
+        permission (int): The file permission. Default: ``stat.S_IREAD + stat.S_IWRITE``.
 
     Supported Platforms:
         ``GPU``
     """
     data = pri_var.asnumpy()
     data = np.transpose(data, (0, 2, 1, 3))
     nx = list(data.shape)[1]
@@ -92,7 +97,8 @@
     plt.subplot(2, 2, 4)
     plt.title("pressure")
     plt.scatter(x, y, c=p, cmap=plt.cm.gray, vmin=min(p[:]), vmax=max(p[:]))
     plt.colorbar()
 
     plt.subplots_adjust(left=0.05, right=0.97, top=0.9, bottom=0.1)
     plt.savefig(file_name)
+    os.chmod(file_name, permission)
```

## mindflow/cfd/space_solver/reconstructor/__init__.py

```diff
@@ -9,18 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """init of reconstructor."""
+from .weno3 import WENO3
 from .weno5 import WENO5
+from .weno7 import WENO7
 
 _reconstructor_dict = {
+    'WENO3': WENO3,
     'WENO5': WENO5,
+    'WENO7': WENO7,
 }
 
 
 def define_reconstructor(name):
     """Define interpolator according to interpolator configuration"""
     ret = _reconstructor_dict.get(name)
     if ret is None:
```

## mindflow/cfd/space_solver/riemann_computer/__init__.py

```diff
@@ -9,21 +9,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """init of riemann computer."""
+from .hllc import HLLC
+from .roe import Roe
 from .rusanov import Rusanov
 from .rusanov_net import RusanovNet
 
-_riemann_dict = {
-    'Rusanov': Rusanov,
-    'RusanovNet': RusanovNet
-}
+_riemann_dict = {'Rusanov': Rusanov, 'RusanovNet': RusanovNet, 'HLLC': HLLC, 'Roe': Roe}
 
 
 def define_riemann_computer(name):
     """Define riemann computer according to riemann computer configuration"""
     ret = _riemann_dict.get(name)
     if ret is None:
         err = "riemann {} has not been implied".format(name)
```

## mindflow/cfd/space_solver/riemann_computer/rusanov_net.py

```diff
@@ -36,15 +36,15 @@
         con_var_right (Tensor): Conservative variables on right side face.
         axis (int): 0, 1, 2 indicate x-dimension, y-dimension and z-dimension respectively.
 
     Outputs:
         Tensor, calculated riemann flux.
 
     Raises:
-        ValueError: If net_dict do not have 'rusanov_net'.
+        ValueError: If `net_dict` do not have 'rusanov_net'.
 
     Supported Platforms:
         ``GPU``
     """
 
     def __init__(self, material, net_dict):
         super(RusanovNet, self).__init__(material)
```

## mindflow/common/lr_scheduler.py

```diff
@@ -22,14 +22,16 @@
 from ..utils.check_func import check_lr_param_type_value, check_param_type
 
 
 def get_poly_lr(global_step, lr_init, lr_end, lr_max, warmup_steps, total_steps, poly_power):
     r"""
     Generate polynomial decay learning rate array.
     The learning rate decays in a polynomial manner as training goes along.
+    it follows :math:`lr = step * (lr\_max - lr\_init)/warmup\_steps` ,
+    then :math:`lr = lr\_end + (lr\_max - lr\_end) * [(1 - i + step)/(total\_steps - warmup\_steps)]**poly\_power`
 
     Args:
         global_step (int): current step number, non-negtive int value.
         lr_init (float): init learning rate, positive float value.
         lr_end (float): end learning rate, non-negtive float value.
         lr_max (float): max learning rate, positive float value.
         warmup_steps (int): number of warmup epochs, non-negtive int value.
@@ -184,17 +186,17 @@
     .. math::
         warmup\_learning\_rate[i] = (lr\_init - warmup\_lr\_init) * i / warmup\_steps + warmup\_lr\_init
 
     Args:
         lr_init (float): init learning rate, positive float value.
         steps_per_epoch (int): number of steps to each epoch, positive int value.
         last_epoch (int): total epoch of training, positive int value.
-        warmup_epochs (int): total epoch of warming up, default:0.
-        warmup_lr_init (float): warmup init learning rate, default:0.0.
-        eta_min (float): minimum learning rate, default: 1e-6.
+        warmup_epochs (int): total epoch of warming up, default: ``0``.
+        warmup_lr_init (float): warmup init learning rate, default: ``0.0``.
+        eta_min (float): minimum learning rate, default: ``1e-6``.
 
     Returns:
         Numpy.array, learning rate array.
 
     Raises:
         TypeError: If `lr_init` or `warmup_lr_init` or `eta_min` is not a float.
         TypeError: If `steps_per_epoch` or `warmup_epochs` or `last_epoch` is not an int.
```

## mindflow/common/math.py

```diff
@@ -12,50 +12,49 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 '''
 math operators
 '''
 import numpy as np
-import mindspore.numpy as mnp
 
-from ..cell.utils import to_2tuple
+from ..cell.utils import to_2tuple, to_3tuple
 
-__all__ = ['get_grid_1d', 'get_grid_2d', 'fftshift', 'ifftshift']
+__all__ = ['get_grid_1d', 'get_grid_2d', 'get_grid_3d']
 
 
 def get_grid_1d(resolution):
-    grid_x = np.linspace(0, 1, resolution)
-    return grid_x.reshape(1, resolution, 1)
+    """get grid 1d"""
+    grid_x = np.linspace(0, 1, resolution).reshape(1, resolution, 1) \
+        if isinstance(resolution, int) else np.linspace(0, 1, resolution[0]).reshape(1, resolution[0], 1)
+    return grid_x
 
 
 def get_grid_2d(resolution):
-    resolution = to_2tuple(resolution)
+    """get grid 2d"""
+    resolution = to_2tuple(resolution) if isinstance(resolution, int) else resolution
     res_x = resolution[0]
     res_y = resolution[1]
     grid_x = np.linspace(0, 1, res_x).reshape(1, res_x, 1, 1)
     grid_y = np.linspace(0, 1, res_y).reshape(1, 1, res_y, 1)
     grid_x = np.repeat(grid_x, res_y, axis=2)
     grid_y = np.repeat(grid_y, res_x, axis=1)
     return np.concatenate((grid_x, grid_y), axis=-1)
 
 
-def fftshift(x, axes=None):
-    if axes is None:
-        axes = tuple(range(x.ndim))
-        shift = [dim // 2 for dim in x.shape]
-    elif isinstance(axes, int):
-        shift = x.shape[axes] // 2
-    else:
-        shift = [x.shape[ax] // 2 for ax in axes]
-    return mnp.roll(x, shift, axes)
-
-
-def ifftshift(x, axes=None):
-    if axes is None:
-        axes = tuple(range(x.ndim))
-        shift = [-(dim // 2) for dim in x.shape]
-    elif isinstance(axes, int):
-        shift = -(x.shape[axes] // 2)
-    else:
-        shift = [-(x.shape[ax] // 2) for ax in axes]
-    return mnp.roll(x, shift, axes)
+def get_grid_3d(resolution):
+    """get grid 3d"""
+    resolution = to_3tuple(resolution) if isinstance(resolution, int) else resolution
+    res_x = resolution[0]
+    res_y = resolution[1]
+    res_z = resolution[2]
+    grid_x = np.linspace(0, 1, res_x).reshape(1, res_x, 1, 1, 1)
+    grid_y = np.linspace(0, 1, res_y).reshape(1, 1, res_y, 1, 1)
+    grid_z = np.linspace(0, 1, res_z).reshape(1, 1, 1, res_z, 1)
+    grid_x = np.repeat(grid_x, res_y, axis=2)
+    grid_x = np.repeat(grid_x, res_z, axis=3)
+    grid_y = np.repeat(grid_y, res_x, axis=1)
+    grid_y = np.repeat(grid_y, res_z, axis=3)
+    grid_z = np.repeat(grid_z, res_x, axis=1)
+    grid_z = np.repeat(grid_z, res_y, axis=2)
+
+    return np.concatenate((grid_x, grid_y, grid_z), axis=-1)
```

## mindflow/data/boundary.py

```diff
@@ -30,16 +30,16 @@
     """
     Base class of boundary condition and initial condition.
 
     Args:
         geometry (Geometry): specifies geometry information of boundary condition and initial condition.
 
     Raises:
-        ValueError: if sampling_config of geometry is None.
-        TypeError: if geometry is not an instance of Geometry.
+        ValueError: if `sampling_config` of geometry is ``None``.
+        TypeError: if `geometry` is not an instance of Geometry.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Geometry
         >>> from mindflow.data import Boundary
@@ -118,18 +118,19 @@
 
 
 class BoundaryBC(Boundary):
     """
     Sampling data of boundary condition.
 
     Args:
-        geometry (Geometry): specifies geometry information of boundary condition.
+        geometry (Geometry): specifies geometry information of boundary condition. Derived from mindflow.geometry,
+            the geometry could be cube or disk, etc.
 
     Raises:
-        ValueError: if sampling_config.bc of geometry is None.
+        ValueError: if sampling_config.bc of `geometry` is ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Geometry
         >>> from mindflow.data import BoundaryBC
@@ -165,15 +166,15 @@
     """
     Sampling data of initial condition.
 
     Args:
         geometry (Geometry): specifies geometry information of initial condition.
 
     Raises:
-        ValueError: if sampling_config.ic of geometry is None.
+        ValueError: if sampling_config.ic of geometry is ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Geometry
         >>> from mindflow.data import BoundaryIC
```

## mindflow/data/data_base.py

```diff
@@ -28,22 +28,23 @@
 
 class Data:
     """
     This class is the base class of Dataset, Equation, Boundary and ExistedDataset. It represents
     a node in the data flow graph.
 
     Args:
-        name (str): distinguished name of specified dataset (default=None).
-        columns_list (Union[list, tuple]): list of column names (default=None).
+        name (str): distinguished name of specified dataset. Default: ``None``.
+        columns_list (Union[list, tuple]): list of column names. Default: ``None``.
         constraint_type (str, optional): constraint type of the specified dataset to get it's corresponding loss
-            function (default=None). The constraint_type can be equation, bc, ic, label or function.
+            function. Default: ``None``. The `constraint_type` can be ``"equation"``, ``"bc"``, ``"ic"``,
+            ``"label"`` or ``"function"``.
 
     Raises:
-        TypeError: if constraint_type is None or constraint_type.lower() not in ["equation", "bc", "ic", "label",
-                   "function"].
+        TypeError: if `constraint_type` is ``None`` or `constraint_type.lower()` is not in
+            [``"equation"``, ``"bc"``, ``"ic"``, ``"label"``, ``"function"``].
 
     Supported Platforms:
         ``Ascend``
     """
     def __init__(self, name=None, columns_list=None, constraint_type=None):
         none_type = type(None)
         check_param_type(name, "name", data_type=[str, none_type])
@@ -87,18 +88,20 @@
     """
     Set arguments of ExistedDataset.
 
     Args:
         name (str): specifies the name of dataset.
         data_dir (Union[str, list, tuple]): the path of existed data files.
         columns_list (Union[str, list, tuple]): list of column names of the dataset.
-        data_format (str, optional): the format of existed data files (default='npy'). The format of 'npy'
-            is supported now.
-        constraint_type (str, optional): specifies the constraint type of the created dataset (default="Label").
-        random_merge (bool, optional): specifies whether randomly merge the given datasets (default=True).
+        data_format (str, optional): the format of existed data files. Default: ``'npy'``.
+            The format of ``'npy'`` is supported now.
+        constraint_type (str, optional): specifies the constraint type of the created dataset.
+            Default: ``"Label"``.
+        random_merge (bool, optional): specifies whether randomly merge the given datasets.
+            Default: ``True``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
     """
     def __init__(self, name, data_dir, columns_list, data_format="npy", constraint_type="Label", random_merge=True):
         check_param_type(name, "name", data_type=str)
         self.name = name
```

## mindflow/data/dataset.py

```diff
@@ -41,28 +41,29 @@
 class Dataset(Data):
     r"""
     Combine datasets together.
 
     Parameters:
         geometry_dict (dict, optional): specifies geometry datasets to be merged. The key is geometry instance and
             value is a list of type of geometry. For example, geometry_dict = {geom : ["domain", "BC", "IC"]}.
-            Default: None.
+            Default: ``None``.
         existed_data_list (Union[list, tuple, ExistedDataConfig], optional): specifies existed datasets to be merged.
-            For example, existed_data_list = [ExistedDataConfig_Instance1, ExistedDataConfig_Instance2]. Default: None.
+            For example, existed_data_list = [ExistedDataConfig_Instance1, ExistedDataConfig_Instance2].
+            Default: ``None``.
         dataset_list (Union[list, tuple, Data], optional): specifies instances of data to be merged. For example,
             dataset_list=[BoundaryIC_Instance, Equation_Instance, BoundaryBC_Instance and ExistedData_Instance].
-            Default: None.
+            Default: ``None``.
 
     Raises:
-        ValueError: If geometry_dict, existed_data_list and dataset_list are all None.
-        TypeError: If the type of geometry_dict is not dict.
+        ValueError: If `geometry_dict`, existed_data_list and dataset_list are all ``None``.
+        TypeError: If the type of `geometry_dict` is not dict.
         TypeError: If the type of key of geometry_dict is not instance of class Geometry.
-        TypeError: If the type of existed_data_list is not list, tuple or instance of ExistedDataConfig.
-        TypeError: If the element of existed_data_list is not instance of ExistedDataConfig.
-        TypeError: If the element of dataset_list is not instance of class Data.
+        TypeError: If the type of `existed_data_list` is not list, tuple or instance of ExistedDataConfig.
+        TypeError: If the element of `existed_data_list` is not instance of ExistedDataConfig.
+        TypeError: If the element of `dataset_list` is not instance of class Data.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import Rectangle, generate_sampling_config
         >>> from mindflow.data import Dataset
@@ -144,44 +145,49 @@
                        input_output_columns_map=None,
                        shuffle=True,
                        drop_remainder=True,
                        prebatched_data=False,
                        num_parallel_workers=1,
                        num_shards=None,
                        shard_id=None,
-                       python_multiprocessing=False):
+                       python_multiprocessing=False,
+                       sampler=None):
         """
         create the final mindspore type dataset to merge all the sub-datasets.
 
         Args:
-            batch_size (int, optional): An int number of rows each batch is created with. Default: 1.
+            batch_size (int, optional): An int number of rows each batch is created with. Default: ``1``.
             preprocess_fn (Union[list[TensorOp], list[functions]], optional): List of operations to be
-                applied on the dataset. Operations are applied in the order they appear in this list. Default: None.
+                applied on the dataset. Operations are applied in the order they appear in this list.
+                Default: ``None``.
             input_output_columns_map (dict, optional): specifies which columns to replace and to what.
                 The key is the column name to be replaced and the value is the name you want to replace with.
-                There's no need to set this argument if all columns are not changed after mapping. Default: None.
+                There's no need to set this argument if all columns are not changed after mapping.
+                Default: ``None``.
             shuffle (bool, optional): Whether or not to perform shuffle on the dataset. Random accessible input is
-                required. Default: True, expected order behavior shown in the table.
+                required. Default: ``True``, expected order behavior shown in the table.
             drop_remainder (bool, optional): Determines whether or not to drop the last block
-                whose data row number is less than batch size. If True, and if there are less
+                whose data row number is less than batch size. If ``True``, and if there are less
                 than batch_size rows available to make the last batch, then those rows will
-                be dropped and not propagated to the child node. Default: True.
-            prebatched_data (bool, optional): Generate pre-batched data before create mindspore dataset. If True,
+                be dropped and not propagated to the child node. Default: ``True``.
+            prebatched_data (bool, optional): Generate pre-batched data before create mindspore dataset. If ``True``,
                 pre-batched data will be returned when get each sub-dataset data by index. Else, the batch operation
                 will be done by mindspore dataset interface: dataset.batch. When batch_size is very large, it's
-                recommended to set this option to be True in order to improve performance on host. Default: False.
+                recommended to set this option to be ``True`` in order to improve performance on host.
+                Default: ``False``.
             num_parallel_workers (int, optional): Number of workers(threads) to process the dataset in parallel.
-                Default: 1.
+                Default: ``1``.
             num_shards (int, optional): Number of shards that the dataset will be divided into.
                 Random accessible input is required. When this argument is specified, `num_samples` reflects the
-                maximum sample number of per shard. Default: None.
+                maximum sample number of per shard. Default: ``None``.
             shard_id (int, optional): The shard ID within num_shards. This argument must be specified
-                only when num_shards is also specified. Random accessible input is required. Default: None.
+                only when num_shards is also specified. Random accessible input is required. Default: ``None``.
             python_multiprocessing (bool, optional): Parallelize Python function per_batch_map with multi-processing.
-                This option could be beneficial if the function is computational heavy. Default: False.
+                This option could be beneficial if the function is computational heavy. Default: ``False``.
+            sampler (Sampler, optional): Dataset Sampler. Default: ``None``.
 
         Returns:
             BatchDataset, dataset batched.
 
         Examples:
             >>> data = dataset.create_dataset()
         """
@@ -218,14 +224,18 @@
         self.dataset_columns_map, self.dataset_constraint_map, self.column_index_map = self._create_trace_maps()
         logger.info("Dataset columns map: {}".format(self.dataset_columns_map))
         logger.info("Dataset column index map: {}".format(
             self.column_index_map))
         logger.info("Dataset constraints map: {}".format(
             self.dataset_constraint_map))
 
+        if sampler:
+            logger.info("Dataset uses sampler")
+            dataset.use_sampler(sampler)
+
         if preprocess_fn:
             input_columns = copy.deepcopy(self.columns_list)
             check_param_type(input_output_columns_map,
                              "input_output_columns_map", (type(None), dict))
             if input_output_columns_map:
                 new_columns_list, new_dataset_columns_map = self._update_columns_list(
                     input_output_columns_map)
@@ -241,17 +251,17 @@
                 logger.info("Dataset constraints after preprocess: {}".format(
                     self.dataset_constraint_map))
             output_columns = self.columns_list
 
             dataset = dataset.map(operations=preprocess_fn,
                                   input_columns=input_columns,
                                   output_columns=output_columns,
-                                  column_order=output_columns,
                                   num_parallel_workers=num_parallel_workers,
                                   python_multiprocessing=python_multiprocessing)
+            dataset = dataset.project(output_columns)
             logger.info("Get all dataset columns names after preprocess: {}".format(
                 self.columns_list))
 
         if not prebatched_data:
             dataset = dataset.batch(batch_size=batch_size,
                                     drop_remainder=drop_remainder,
                                     num_parallel_workers=num_parallel_workers)
@@ -294,16 +304,14 @@
         for name in new_dataset_columns_map:
             new_columns_list += new_dataset_columns_map[name]
         return new_columns_list, new_dataset_columns_map
 
     def get_columns_list(self):
         """get columns list
 
-        Args:
-
         Returns:
             list[str]. column names list of the final unified dataset.
 
         Examples:
             >>> columns_list = dataset.get_columns_list()
         """
         if not self.columns_list:
@@ -333,15 +341,16 @@
 
     def set_constraint_type(self, constraint_type="Equation"):
         """set constraint type of dataset
 
         Args:
             constraint_type (Union[str, dict]): The constraint type of specified dataset. If is string, the constraint
                 type of all subdataset will be set to the same one. If is dict, the subdataset and it's constraint type
-                is specified by the pair (key, value). Default: "Equation".
+                is specified by the pair (key, value). Default: ``"Equation"``. It also supports ``"bc"``, ``"ic"``,
+                ``"label"``, ``"function"``, and ``"custom"``.
 
         Examples:
             >>> dataset.set_constraint_type("Equation")
         """
         if isinstance(constraint_type, str):
             logger.warning("Argument constraint_type: {} is str, the same type will be set for all of the sub-datasets"
                            .format(constraint_type))
```

## mindflow/data/equation.py

```diff
@@ -33,17 +33,17 @@
     """
     Sampling data of equation domain.
 
     Args:
         geometry (Geometry): specifies geometry information of equation domain.
 
     Raises:
-        TypeError: if geometry is not instance of class Geometry.
-        ValueError: if sampling_config of geometry is None.
-        KeyError: if sampling_config.domain of geometry is None.
+        TypeError: if `geometry` is not instance of class Geometry.
+        ValueError: if sampling_config of `geometry` is ``None``.
+        KeyError: if sampling_config.domain of `geometry` is ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Geometry
         >>> from mindflow.data import Equation
```

## mindflow/data/existed_data.py

```diff
@@ -28,35 +28,35 @@
 
 
 class ExistedDataset(Data):
     r"""
     Creates a dataset with given data path.
 
     Note:
-        The `npy` data format is supported now.
+        The ``'npy'`` data format is supported now.
 
     Parameters:
-        name (str, optional): specifies the name of dataset (default=None). If `data_config` is None, the `name` should
-            not be None.
-        data_dir (Union[str, list, tuple], optional): the path of existed data files (default=None). If `data_config`
-            is None, the `data_dir` should not be None.
-        columns_list (Union[str, list, tuple], optional): list of column names of the dataset (default=None). If
-            `data_config` is None, the `columns_list` should not be None.
-        data_format (str, optional): the format of existed data files (default='npy').
-        constraint_type (str, optional): specifies the constraint type of the created dataset (default="Label").
-        random_merge (bool, optional): specifies whether randomly merge the given datasets (default=True).
+        name (str, optional): specifies the name of dataset. Default: ``None``. If `data_config` is ``None``,
+            the `name` should not be ``None``.
+        data_dir (Union[str, list, tuple], optional): the path of existed data files. Default: ``None``.
+            If `data_config` is ``None``, the `data_dir` should not be ``None``.
+        columns_list (Union[str, list, tuple], optional): list of column names of the dataset. Default: ``None``. If
+            `data_config` is ``None``, the `columns_list` should not be ``None``.
+        data_format (str, optional): the format of existed data files. Default: ``'npy'``.
+        constraint_type (str, optional): specifies the constraint type of the created dataset. Default: "Label".
+        random_merge (bool, optional): specifies whether randomly merge the given datasets. Default: ``True``.
         data_config (ExistedDataConfig, optional): Instance of ExistedDataConfig which collect the info
-            described above (default=None). If it's not None, the dataset class will be create by using it for
-            simplifying. If it's None, the info of (name, data_dir, columns_list, data_format, constraint_type,
-            random_merge) will be used for replacement.
+            described above. Default: ``None``. If it's not ``None``, the dataset class will be create by
+            using it for simplifying. If it's ``None``, the info of (name, data_dir, columns_list, data_format,
+            constraint_type, random_merge) will be used for replacement.
 
     Raises:
-        ValueError: Argument name/data_dir/columns_list is None when data_config is None.
+        ValueError: Argument `name`/`data_dir`/`columns_list` is ``None`` when `data_config` is ``None``.
         TypeError: If data_config is not a instance of ExistedDataConfig.
-        ValueError: If data_format is not 'npy'.
+        ValueError: If data_format is not ``'npy'``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.data import ExistedDataConfig, ExistedDataset
         >>> data_config = ExistedDataConfig(name='exist',
```

## mindflow/data/mind_dataset.py

```diff
@@ -28,47 +28,48 @@
 
 
 class MindDataset(Data):
     """
     Create dataset from MindRecord-type data.
 
     Args:
-        dataset_files (Union[str, list[str]]): If dataset_file is a str, it represents for
+        dataset_files (Union[str, list[str]]): If `dataset_file` is a str, it represents for
             a file name of one component of a mindrecord source, other files with identical source
-            in the same path will be found and loaded automatically. If dataset_file is a list,
+            in the same path will be found and loaded automatically. If `dataset_file` is a list,
             it represents for a list of dataset files to be read directly.
-        dataset_name (str, optional): name of dataset, Default: "dataset_name"
+        dataset_name (str, optional): name of dataset. Default: ``"dataset_name"``.
         constraint_type (str, optional): constraint type of the specified dataset to get it's corresponding loss
-            function. Default: "Label"
+            function. Default: ``"Label"``. Other supported types can be found in `mindflow.data.Dataset`.
         shuffle (Union[bool, Shuffle level], optional): Perform reshuffling of the data every epoch
-            If shuffle is False, no shuffling will be performed.
-            If shuffle is True, performs global shuffle. Default: True.
+            If `shuffle` is ``False``, no shuffling will be performed.
+            If `shuffle` is ``True``, performs global shuffle. Default: ``True``.
             Otherwise, there are two levels of shuffling:
 
-            - Shuffle.GLOBAL: Shuffle both the files and sample.
-            - Shuffle.FILES: Shuffle files only.
+            - ``Shuffle.GLOBAL``: Shuffle both the files and sample.
+            - ``Shuffle.FILES``: Shuffle files only.
 
-        num_shards (int, optional): Number of shards that the dataset will be divided into (default=None).
+        num_shards (int, optional): Number of shards that the dataset will be divided into. Default: ``None``.
             When this argument is specified, 'num_samples' reflects the maximum sample number of per shard.
-        shard_id (int, optional): The shard ID within `num_shards` (default=None). This
+        shard_id (int, optional): The shard ID within `num_shards`. Default: ``None``. This
             argument can only be specified when `num_shards` is also specified.
         sampler (Sampler, optional): Object used to choose samples from the
-            dataset (default=None, sampler is exclusive
-            with shuffle and block_reader). Support list: SubsetRandomSampler,
-            PkSampler, RandomSampler, SequentialSampler, DistributedSampler.
-        num_samples (int, optional): The number of samples to be included in the dataset
-            (default=None, all samples).
-        num_parallel_workers (int, optional): The number of readers (default=None).
+            dataset. Default: ``None``, sampler is exclusive
+            with shuffle and block_reader. Support list: ``SubsetRandomSampler``,
+            ``PkSampler``, ``RandomSampler``, ``SequentialSampler``, ``DistributedSampler``.
+        num_samples (int, optional): The number of samples to be included in the dataset. Default: ``None``,
+            all samples.
+        num_parallel_workers (int, optional): The number of readers. Default: ``None``.
 
     Raises:
-        ValueError: If dataset_files are not valid or do not exist.
-        TypeError: If dataset_name is not string.
-        ValueError: If constraint_type.lower() not in ["equation", "bc", "ic", "label", "function", "custom"].
-        RuntimeError: If `num_shards` is specified but `shard_id` is None.
-        RuntimeError: If `shard_id` is specified but `num_shards` is None.
+        ValueError: If `dataset_files` are not valid or do not exist.
+        TypeError: If `dataset_name` is not string.
+        ValueError: If `constraint_type.lower()` not in [``"equation"``, ``"bc"``, ``"ic"``, ``"label"``,
+            ``"function"``, ``"custom"``].
+        RuntimeError: If `num_shards` is specified but `shard_id` is ``None``.
+        RuntimeError: If `shard_id` is specified but `num_shards` is ``None``.
         ValueError: If `shard_id` is invalid (< 0 or >= `num_shards`).
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.data import MindDataset
@@ -93,22 +94,22 @@
         self.dataset_columns_map = {dataset_name: self.columns_list}
         for i in range(len(self.columns_list)):
             self.column_index_map[self.columns_list[i]] = i
         self.dataset_constraint_map = {dataset_name: constraint_type}
         self.dataset_name = [dataset_name]
 
     def split_dataset(self, dataset_dict, constraint_dict=None):
-        """split the original dataset in order to set difference loss functions
+        """split the original dataset in order to set difference loss functions.
 
         Args:
             dataset_dict (dict): dictionary of each sub-dataset, the key is the labeled name while the value
                 refers to the specified columns contained in the sub-dataset.
-            constraint_dict (Union[None, str, dict]): The constraint type of specified dataset. If None, "Label" will be
-                set for all. If is string, all will be set to the same one. If is dict,
-                the subdataset and it's constraint type is specified by the pair (key, value). Default: None.
+            constraint_dict (Union[None, str, dict]): The constraint type of specified dataset. If ``None``,
+                "Label" will be set for all. If is string, all will be set to the same one. If is dict,
+                the subdataset and it's constraint type is specified by the pair (key, value). Default: ``None``.
 
         Examples:
             >>> dataset.split_dataset({"Equation" : "inner_points", "BC" : "bc_points"})
         """
         check_dict_type_value(dataset_dict, "sub-dataset dict", key_type=str, value_type=str,
                               value_value=self.columns_list)
         if constraint_dict:
@@ -161,27 +162,31 @@
                        prebatched_data=False,
                        num_parallel_workers=1,
                        python_multiprocessing=False):
         """
         create the final mindspore type dataset.
 
         Args:
-            batch_size (int, optional): An int number of rows each batch is created with. Default: 1.
+            batch_size (int, optional): An int number of rows each batch is created with. Default: ``1``.
             preprocess_fn (Union[list[TensorOp], list[functions]], optional): List of operations to be
-                applied on the dataset. Operations are applied in the order they appear in this list. Default: None.
-            updated_columns_list (list, optional): List of columns to be applied on the dataset. Default: None.
+                applied on the dataset. Operations are applied in the order they appear in this list.
+                Default: ``None``.
+            updated_columns_list (list, optional): List of columns to be applied on the dataset.
+                Default: ``None``.
             drop_remainder (bool, optional): Determines whether or not to drop the last block
-                whose data row number is less than batch size. If True, and if there are less
+                whose data row number is less than batch size. If ``True``, and if there are less
                 than batch_size rows available to make the last batch, then those rows will
-                be dropped and not propagated to the child node. Default: True.
-            prebatched_data (bool, optional): Generate pre-batched data before data preprocessing. Default: False.
+                be dropped and not propagated to the child node. Default: ``True``.
+            prebatched_data (bool, optional): Generate pre-batched data before data preprocessing.
+                Default: ``False``.
             num_parallel_workers (int, optional): Number of workers(threads) to process the dataset in parallel.
                 Default: 1.
             python_multiprocessing (bool, optional): Parallelize Python function per_batch_map with multi-processing.
-                This option could be beneficial if the function is computational heavy. Default: False.
+                This option could be beneficial if the function is computational heavy.
+                Default: ``False``.
 
         Returns:
             BatchDataset, dataset batched.
 
         Examples:
             >>> data = dataset.create_dataset()
         """
```

## mindflow/geometry/__init__.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """init"""
 from .geometry_base import Geometry, PartSamplingConfig, SamplingConfig
 from .geometry_1d import Interval
-from .geometry_2d import Disk, Rectangle, Triangle, Pentagon
+from .geometry_2d import Disk, Rectangle, Triangle, Pentagon, Polygon
 from .geometry_3d import Cuboid, Cylinder, Cone, Tetrahedron
 from .geometry_nd import FixedPoint, HyperCube
 from .geometry_td import TimeDomain, GeometryWithTime
 from .csg import CSGIntersection, CSGDifference, CSGUnion, CSGXOR, CSG
 from .geom_utils import generate_sampling_config
 
 __all__ = [
@@ -27,23 +27,24 @@
     "PartSamplingConfig",
     "SamplingConfig",
     "Interval",
     "Disk",
     "Rectangle",
     "Triangle",
     "Pentagon",
+    "Polygon",
     "Cuboid",
     "Cylinder",
     "Cone",
     "Tetrahedron",
     "FixedPoint",
     "HyperCube",
     "TimeDomain",
     "GeometryWithTime",
     "CSGIntersection",
     "CSGDifference",
     "CSGUnion",
     "CSGXOR",
-    "generate_sampling_config"
+    "generate_sampling_config",
 ]
 
 __all__.sort()
```

## mindflow/geometry/csg.py

```diff
@@ -96,24 +96,24 @@
         self.name = name
 
     def sampling(self, geom_type="domain"):
         """
         sampling points
 
         Args:
-            geom_type (str): geometry type
+            geom_type (str): geometry type.
 
         Returns:
-            Numpy.array, numpy array with or without boundary normal vectors
+            Numpy.array, numpy array with or without boundary normal vectors.
 
         Raises:
-            ValueError: If `config` is None.
-            KeyError: If `geom_type` is `domain` but `config.domain` is None.
-            KeyError: If `geom_type` is `BC` but `config.bc` is None.
-            ValueError: If `geom_type` is neither `BC` nor `domain`.
+            ValueError: If `config` is ``None``.
+            KeyError: If `geom_type` is `domain` but `config.domain` is ``None``.
+            KeyError: If `geom_type` is ``"BC"`` but `config.bc` is ``None``.
+            ValueError: If `geom_type` is neither ``"BC"`` nor ``"domain"``.
         """
         self._check_sampling_config(self.sampling_config)
         config = self.sampling_config
         check_param_type_value(geom_type, "geom_type", valid_value=GEOM_TYPES, data_type=str)
         if geom_type.lower() == "domain":
             check_param_type(config.domain, _SPACE.join((self.geom_type, self.name, "'s domain config")),
                              exclude_type=type(None))
@@ -149,15 +149,15 @@
 class CSGDifference(CSG):
     r"""
     CSG class for difference of geometry.
 
     Args:
         geom1 (Geometry): a geometry object.
         geom2 (Geometry): a geometry object to be subtracted from geom1.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Disk, Rectangle, CSGDifference
         >>> sampling_config_csg = dict({
@@ -272,15 +272,15 @@
 class CSGUnion(CSG):
     r"""
     CSG class for union of geometries.
 
     Args:
         geom1 (Geometry): a geometry object.
         geom2 (Geometry): a geometry object to be subtracted from geom1.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Disk, Rectangle, CSGUnion
         >>> sampling_config_csg = dict({
@@ -389,15 +389,15 @@
 class CSGIntersection(CSG):
     r"""
     CSG class for intersection of geometries.
 
     Args:
         geom1 (Geometry): a geometry object.
         geom2 (Geometry): a geometry object to be subtracted from geom1.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Disk, Rectangle, CSGIntersection
         >>> sampling_config_csg = dict({
@@ -508,15 +508,15 @@
 class CSGXOR(CSG):
     r"""
     CSG class for xor of geometries.
 
     Args:
         geom1 (Geometry): a geometry object.
         geom2 (Geometry): a geometry object to be subtracted from geom1.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Disk, Rectangle, CSGXOR
         >>> sampling_config_csg = dict({
```

## mindflow/geometry/geom_utils.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """utils for geometry"""
 from __future__ import absolute_import
 import numpy as np
-import scipy.stats as ss
+from scipy.stats import qmc
 
 from .geometry_base import PartSamplingConfig, SamplingConfig, GEOM_TYPES, SAMPLER_TYPES
 from ..utils.check_func import check_param_type
 
 
 def generate_sampling_config(dict_config):
     """
@@ -65,17 +65,17 @@
                                                              dict_config[geom_type].get("with_sdf", False))
     if part_dict_config:
         return SamplingConfig(part_dict_config)
     raise ValueError("Unknown sampling info, please check your config")
 
 
 _sampler_method = {
-    "lhs": ss.qmc.LatinHypercube,
-    "halton": ss.qmc.Halton,
-    "sobol": ss.qmc.Sobol,
+    "lhs": qmc.LatinHypercube,
+    "halton": qmc.Halton,
+    "sobol": qmc.Sobol,
     "uniform": np.random.rand
 }
 
 
 def sample(size, dimension, sampler="uniform"):
     """function for sampling points by different random methods"""
     sampler = sampler.lower()
```

## mindflow/geometry/geometry_1d.py

```diff
@@ -25,16 +25,16 @@
     r"""
     Definition of Interval object.
 
     Args:
         name (str): name of the interval.
         coord_min (Union[int, float]): left of the interval.
         coord_max (Union[int, float]): right of the interval.
-        dtype (numpy.dtype): Data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        dtype (numpy.dtype): Data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Raises:
         ValueError: If `coord_min` or `coord_max` is neither int nor float .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
```

## mindflow/geometry/geometry_2d.py

```diff
@@ -19,31 +19,31 @@
 import numpy as np
 import numpy.linalg as LA
 from mindspore import log as logger
 
 from .geometry_base import Geometry, DATA_TYPES, GEOM_TYPES, SamplingConfig
 from .geometry_nd import HyperCube
 from .geom_utils import sample, polar_sample, generate_mesh
-from .shapes import adapter, simplex, pentagon
+from .shapes import adapter, simplex, pentagon, polygon
 from ..utils.check_func import check_param_type, check_param_type_value
 
 _SPACE = " "
 
 
 class Disk(Geometry):
     r"""
     Definition of Disk object.
 
     Args:
         name (str): name of the disk.
         center (Union[tuple[int, int], tuple[float, float], list[int, int], list[float, float], numpy.ndarray]):
             center coordinates of the disk.
         radius (Union[int, float]): radius of the disk.
-        dtype (numpy.dtype): data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        dtype (numpy.dtype): data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Raises:
         ValueError: If `center` is neither list nor tuple of length 2.
         ValueError: If `radius` is negative.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
@@ -150,28 +150,28 @@
         return -sdf
 
     def sampling(self, geom_type="domain"):
         """
         sampling domain and boundary points
 
         Args:
-            geom_type (str): geometry type: can be 'domain' or 'BC'. Default: 'domain'.
+            geom_type (str): geometry type: can be ``'domain'`` or ``'BC'``. Default: ``'domain'``.
 
-                - 'domain', feasible domain of the problem.
-                - 'BC', boundary of the problem.
+                - ``'domain'``, feasible domain of the problem.
+                - ``'BC'``, boundary of the problem.
 
         Returns:
             Numpy.array. If the with_normal property of boundary configuration is true, returns 2D numpy array with
             boundary normal vectors. Otherwise, returns 2D numpy array without boundary normal vectors.
 
         Raises:
-            ValueError: If `config` is None.
-            KeyError: If `geom_type` is `domain` but `config.domain` is None.
-            KeyError: If `geom_type` is `BC` but `config.bc` is None.
-            ValueError: If `geom_type` is neither `BC` nor `domain`.
+            ValueError: If `config` is ``None``.
+            KeyError: If `geom_type` is ``'domain'`` but `config.domain` is ``None``.
+            KeyError: If `geom_type` is ``'BC'`` but `config.bc` is ``None``.
+            ValueError: If `geom_type` is neither ``'BC'`` nor ``'domain'``.
         """
         config = self.sampling_config
         check_param_type(config, _SPACE.join((self.geom_type, self.name, "'s sampling_config")),
                          data_type=SamplingConfig)
         check_param_type_value(geom_type, _SPACE.join((self.geom_type, self.name, "'s geom_type")),
                                GEOM_TYPES, data_type=str)
 
@@ -229,16 +229,16 @@
 
     Args:
         name (str): name of the rectangle.
         coord_min (Union[tuple[int, int], tuple[float, float], list[int, int], list[float, float], numpy.ndarray]):
             coordinates of the bottom left corner of rectangle.
         coord_max (Union[tuple[int, int], tuple[float, float], list[int, int], list[float, float], numpy.ndarray]):
             coordinates of the top right corner of rectangle.
-        dtype (numpy.dtype): data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        dtype (numpy.dtype): data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Rectangle
         >>> rectangle_mesh = dict({'domain': dict({'random_sampling': False, 'size': [50, 25]}),
@@ -257,22 +257,22 @@
 class Triangle(adapter.Geometry):
     r"""
     Definition of triangle object.
 
     Args:
         name (str): name of the triangle.
         vertices (numpy.ndarray): vertices of the triangle.
-        boundary_type (str): this can be 'uniform' or 'unweighted'. Default: 'uniform'.
+        boundary_type (str): this can be ``'uniform'`` or ``'unweighted'``. Default: ``'uniform'``.
 
-            - 'uniform', the expected number of samples in each boundary is proportional to the
+            - ``'uniform'``, the expected number of samples in each boundary is proportional to the
               area (length) of the boundary.
-            - 'unweighted', the expected number of samples in each boundary is the same.
+            - ``'unweighted'``, the expected number of samples in each boundary is the same.
 
-        dtype (numpy.dtype): data type of sampled point data type. Default: np.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: none.
+        dtype (numpy.dtype): data type of sampled point data type. Default: ``np.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``none``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Triangle
         >>> triangle_mesh = dict({'domain': dict({'random_sampling': True, 'size': 300}),
@@ -301,22 +301,22 @@
 class Pentagon(adapter.Geometry):
     r"""
     Definition of pentagon object.
 
     Args:
         name (str): name of the pentagon.
         vertices (numpy.ndarray): vertices of the pentagon in an anti-clockwise order.
-        boundary_type (str): this can be 'uniform' or 'unweighted'. Default: 'uniform'.
+        boundary_type (str): this can be ``'uniform'`` or ``'unweighted'``. Default: ``'uniform'``.
 
-            - 'uniform', the expected number of samples in each boundary is proportional to the
+            - ``'uniform'``, the expected number of samples in each boundary is proportional to the
               area (length) of the boundary.
-            - 'unweighted', the expected number of samples in each boundary is the same.
+            - ``'unweighted'``, the expected number of samples in each boundary is the same.
 
-        dtype (numpy.dtype): data type of sampled point data type. Default: np.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: none.
+        dtype (numpy.dtype): data type of sampled point data type. Default: ``np.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``none``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Pentagon
         >>> pentagon_mesh = dict({'domain': dict({'random_sampling': True, 'size': 300}),
@@ -338,9 +338,50 @@
             coord_min=np.min(vertices, axis=0),
             coord_max=np.max(vertices, axis=0),
             dtype=dtype,
             sampling_config=sampling_config,
         )
 
 
-class Polygon(Geometry):
-    pass
+class Polygon(adapter.Geometry):
+    r"""
+    Definition of polygon object.
+
+    Args:
+        name (str): name of the polygon.
+        vertices (numpy.ndarray): vertices of the polygon in an anti-clockwise order.
+        boundary_type (str): this can be ``'uniform'`` or ``'unweighted'``. Default: ``'uniform'``.
+
+            - ``'uniform'``, the expected number of samples in each boundary is proportional to the
+              area (length) of the boundary.
+            - ``'unweighted'``, the expected number of samples in each boundary is the same.
+
+        dtype (numpy.dtype): data type of sampled point data type. Default: ``np.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``none``.
+
+    Supported Platforms:
+        ``Ascend`` ``GPU``
+
+    Examples:
+        >>> from mindflow.geometry import generate_sampling_config, Polygon
+        >>> polygon_mesh = dict({'domain': dict({'random_sampling': True, 'size': 300}),
+        ...                      'BC': dict({'random_sampling': True, 'size': 300, 'with_normal': False,}),})
+        >>> vertices = np.array([[0., 0], [1, 0], [1, 1], [.5, 1], [0.5, 0.5], [0, 0.5]])
+        >>> polygon = Polygon("polygon", vertices,
+        ...                   sampling_config=generate_sampling_config(polygon_mesh))
+        >>> domain = polygon.sampling(geom_type="domain")
+        >>> bc = polygon.sampling(geom_type="bc")
+        >>> print(domain.shape)
+        (300, 2)
+    """
+
+    def __init__(self, name, vertices,
+                 boundary_type="uniform", dtype=np.float32, sampling_config=None):
+        super(Polygon, self).__init__(
+            name=name,
+            shape=polygon.Polygon(vertices, boundary_type),
+            dim=2,
+            coord_min=np.min(vertices, axis=0),
+            coord_max=np.max(vertices, axis=0),
+            dtype=dtype,
+            sampling_config=sampling_config,
+        )
```

## mindflow/geometry/geometry_3d.py

```diff
@@ -29,16 +29,16 @@
 
     Args:
         name (str): name of the cuboid.
         coord_min (Union[tuple[int, int], tuple[float, float], list[int, int], list[float, float], numpy.ndarray]):
             coordinates of the bottom left back corner of cuboid.
         coord_max (Union[tuple[int, int], tuple[float, float], list[int, int], list[float, float], numpy.ndarray]):
             coordinates of the top right front corner of cuboid.
-        dtype (numpy.dtype): data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        dtype (numpy.dtype): data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Cuboid
         >>> cuboid_mesh = dict({'domain': dict({'random_sampling': False, 'size': [50, 50, 25]}),
@@ -56,22 +56,22 @@
 class Tetrahedron(adapter.Geometry):
     r"""
     Definition of tetrahedron object.
 
     Args:
         name (str): name of the tetrahedron.
         vertices (numpy.ndarray): vertices of the tetrahedron.
-        boundary_type (str): this can be 'uniform' or 'unweighted'. Default: 'uniform'.
+        boundary_type (str): this can be ``'uniform'`` or ``'unweighted'``. Default: ``'uniform'``.
 
-            - 'uniform', the expected number of samples in each boundary is proportional to the
+            - ``'uniform'``, the expected number of samples in each boundary is proportional to the
               area (length) of the boundary.
-            - 'unweighted', the expected number of samples in each boundary is the same.
+            - ``'unweighted'``, the expected number of samples in each boundary is the same.
 
-        dtype (numpy.dtype): data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: none.
+        dtype (numpy.dtype): data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``none``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindflow.geometry import generate_sampling_config, Tetrahedron
@@ -109,22 +109,22 @@
     Args:
         name (str): name of the cylinder.
         centre (numpy.ndarray): origin of the bottom disk.
         radius (float): Radius of the cylinder.
         h_min (float): Height coordinate of the bottom disk.
         h_max (float): Height coordinate of the top disk.
         h_axis (int): Axis of the normal vector of the bottom disk.
-        boundary_type (str): this can be 'uniform' or 'unweighted'. Default: 'uniform'.
+        boundary_type (str): this can be ``'uniform'`` or ``'unweighted'``. Default: ``'uniform'``.
 
-            - 'uniform', the expected number of samples in each boundary is proportional to the
+            - ``'uniform'``, the expected number of samples in each boundary is proportional to the
               area (length) of the boundary.
-            - 'unweighted', the expected number of samples in each boundary is the same.
+            - ``'unweighted'``, the expected number of samples in each boundary is the same.
 
-        dtype (numpy.dtype): data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: none.
+        dtype (numpy.dtype): data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``none``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindflow.geometry import generate_sampling_config, Cylinder
@@ -167,22 +167,22 @@
     Args:
         name (str): name of the cone.
         centre (numpy.ndarray): origin of the bottom disk.
         radius (float): Radius of the bottom disk.
         h_min (float): Height coordinate of the bottom disk.
         h_max (float): Maximum Height coordinate of the cone.
         h_axis (int): Axis of the normal vector of the bottom disk.
-        boundary_type (str): this can be 'uniform' or 'unweighted'. Default: 'uniform'.
+        boundary_type (str): this can be ``'uniform'`` or ``'unweighted'``. Default: ``'uniform'``.
 
-            - 'uniform', the expected number of samples in each boundary is proportional to the
+            - ``'uniform'``, the expected number of samples in each boundary is proportional to the
               area (length) of the boundary.
-            - 'unweighted', the expected number of samples in each boundary is the same.
+            - ``'unweighted'``, the expected number of samples in each boundary is the same.
 
-        dtype (numpy.dtype): data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: none.
+        dtype (numpy.dtype): data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``none``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindflow.geometry import generate_sampling_config, Cone
```

## mindflow/geometry/geometry_base.py

```diff
@@ -28,23 +28,23 @@
 
 class PartSamplingConfig:
     """
     Definition of partial sampling configuration.
 
     Args:
         size (Union[int, tuple[int], list[int]]): number of sampling points.
-        random_sampling (bool): Whether randomly sampling points. Default: True.
-        sampler (str): method for random sampling. Default: uniform.
-        random_merge (bool): Specifies whether randomly merge coordinates of different dimensions. Default: True.
-        with_normal (bool): Specifies whether generating the normal vectors of the boundary. Default: False.
+        random_sampling (bool): Whether randomly sampling points. Default: ``True``.
+        sampler (str): method for random sampling. Default: ``"uniform"``.
+        random_merge (bool): Specifies whether randomly merge coordinates of different dimensions. Default: ``True``.
+        with_normal (bool): Specifies whether generating the normal vectors of the boundary. Default: ``False``.
         with_sdf (bool): Specifies whether return the sign-distance-function result of the inner domain points.
-                         Default: False.
+                         Default: ``False``.
 
     Raises:
-        TypeError: size is not int number when random sampling.
+        TypeError: `size` is not int number when random sampling.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import PartSamplingConfig
         >>> partsampling = PartSamplingConfig(100, True, "uniform", True, True)
@@ -73,21 +73,20 @@
     r"""
     Definition of global sampling configuration.
 
     Args:
         part_sampling_dict (dict): sampling configuration.
 
     Raises:
-        ValueError: If `coord_min` or `coord_max` is neither int nor float .
         TypeError: If `part_sampling_dict` is not dict.
-        KeyError: If `geom_type` not "domain", "BC", "IC" or "time".
+        KeyError: If `geom_type` not ``"domain"``, ``"BC"``, ``"IC"`` or ``"time"``.
         TypeError: If 'config' is not PartSamplingConfig object.
-        ValueError: If `self.domain.size` is neither list nor tuple.
-        ValueError: If `self.ic.size` is neither list nor tuple.
-        ValueError: If `self.time.size` is neither list nor tuple.
+        ValueError: If `domain.size` in `part_sampling_dict` is neither list nor tuple.
+        ValueError: If `ic.size` in `part_sampling_dict` is neither list nor tuple.
+        ValueError: If `time.size` in `part_sampling_dict` is neither list nor tuple.
 
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import SamplingConfig, PartSamplingConfig
@@ -122,16 +121,16 @@
     Args:
         name (str): name of the geometry.
         dim (int): number of dimensions.
         coord_min (Union[int, float, list[int, float], tuple[int, float], numpy.ndarray]):
             minimal coordinate of the geometry.
         coord_max (Union[int, float, list[int, float], tuple[int, float], numpy.ndarray]):
             maximal coordinate of the geometry.
-        dtype (numpy.dtype): Data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: None
+        dtype (numpy.dtype): Data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Geometry
         >>> geometry_config = dict({'domain' : dict({'random_sampling' : True, 'size' : 100}),
@@ -169,33 +168,33 @@
         self.dtype = dtype
         check_param_type(sampling_config, "sampling_config", data_type=(type(None), SamplingConfig))
         self.sampling_config = sampling_config
         self.geom_type = type(self).__name__
 
     def set_name(self, name):
         """
-        set geometry instance name
+        Set geometry instance name.
 
         Args:
-            name (str): name of geometry instance
+            name (str): name of geometry instance.
 
         Raises:
             TypeError: If `name` is not string.
 
         Examples:
             >>> from mindflow.geometry import generate_sampling_config, Geometry
             >>> geom = Geometry("geom", 1, 0.0, 1.0)
             >>> geom.set_name("geom_name")
         """
         check_param_type(name, "geometry name", data_type=str)
         self.name = name
 
     def set_sampling_config(self, sampling_config: SamplingConfig):
         """
-        set sampling info
+        Set sampling info.
 
         Args:
             sampling_config (SamplingConfig): sampling configuration.
 
         Raises:
             TypeError: If `sampling_config` is not instance of SamplingConfig.
```

## mindflow/geometry/geometry_nd.py

```diff
@@ -30,16 +30,16 @@
     r"""
     Definition of fixed point object.
 
     Args:
         name (str): name of the fixed point.
         coord (Union[int, float, tuple, list, numpy.ndarray]): coordinate of the fixed point. if the parameter type is
             tuple or list, the element support tuple[int, int], tuple[float, float], list[int, int], list[float, float].
-        dtype (numpy.dtype): Data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        dtype (numpy.dtype): Data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, FixedPoint
         >>> hypercube_random = dict({
@@ -75,24 +75,24 @@
         raise NotImplementedError("{}._boundary_normal not implemented".format(self.geom_type))
 
     def sampling(self, geom_type="domain"):
         """
         sampling points
 
         Args:
-            geom_type (str): geometry type
+            geom_type (str): geometry type, which supports ``'domain'`` and ``'BC'``. Default: ``'domain'``.
 
         Returns:
-            Numpy.array, 2D numpy array with or without boundary normal vectors
+            Numpy.ndarray, 2D numpy array with or without boundary normal vectors.
 
         Raises:
-            ValueError: If `config` is None.
-            KeyError: If `geom_type` is `domain` but `config.domain` is None.
-            KeyError: If `geom_type` is `BC` but `config.bc` is None.
-            ValueError: If `geom_type` is neither `BC` nor `domain`.
+            ValueError: If `config` is ``None``.
+            KeyError: If `geom_type` is ``'domain'`` but `config.domain` is ``None``.
+            KeyError: If `geom_type` is ``'BC'`` but `config.bc` is ``None``.
+            ValueError: If `geom_type` is neither ``'BC'`` nor ``'domain'``.
         """
         config = self.sampling_config
         check_param_type_value(geom_type, _SPACE.join((self.geom_type, self.name, "'s geom_type")),
                                GEOM_TYPES, data_type=str)
         if geom_type.lower() == "domain":
             logger.info("Sampling domain points for {}:{}, config info: {}"
                         .format(self.geom_type, self.name, config.domain))
@@ -126,19 +126,19 @@
         dim (int): number of dimensions.
         coord_min (Union[int, float, tuple, list, numpy.ndarray]): minimal coordinate of the hyper cube. if the
             parameter type is tuple or list, the element support tuple[int, int], tuple[float, float], list[int, int],
             list[float, float].
         coord_max (Union[int, float, tuple, list, numpy.ndarray]): maximal coordinate of the hyper cube. if the
             parameter type is tuple or list, the element support tuple[int, int], tuple[float, float], list[int, int],
             list[float, float].
-        dtype (numpy.dtype): Data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        dtype (numpy.dtype): Data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Raises:
-        TypeError: sampling_config is not instance of class SamplingConfig.
+        TypeError: `sampling_config` is not instance of class SamplingConfig.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, HyperCube
         >>> hypercube_random = dict({
@@ -269,28 +269,28 @@
         return -sdf
 
     def sampling(self, geom_type="domain"):
         """
         sampling points
 
         Args:
-            geom_type (str): geometry type: can be 'domain' or 'BC'. Default: 'domain'.
+            geom_type (str): geometry type: can be ``'domain'`` or ``'BC'``. Default: ``'domain'``.
 
-                - 'domain', feasible domain of the problem.
-                - 'BC', boundary of the problem.
+                - ``'domain'``, feasible domain of the problem.
+                - ``'BC'``, boundary of the problem.
 
         Returns:
-            Numpy.array, if the with_normal property of boundary configuration is true, returns 2D numpy array with
+            Numpy.ndarray, if the with_normal property of boundary configuration is true, returns 2D numpy array with
                          boundary normal vectors. Otherwise, returns 2D numpy array without boundary normal vectors.
 
         Raises:
-            ValueError: If `config` is None.
-            KeyError: If `geom_type` is `domain` but `config.domain` is None.
-            KeyError: If `geom_type` is `BC` but `config.bc` is None.
-            ValueError: If `geom_type` is neither `BC` nor `domain`.
+            ValueError: If `config` is ``None``.
+            KeyError: If `geom_type` is ``'domain'`` but `config.domain` is ``None``.
+            KeyError: If `geom_type` is ``'BC'`` but `config.bc` is ``None``.
+            ValueError: If `geom_type` is neither ``'BC'`` nor ``'domain'``.
         """
         config = self.sampling_config
         check_param_type(config, _SPACE.join((self.geom_type, self.name, "'s sampling_config")),
                          data_type=SamplingConfig)
         check_param_type_value(geom_type, _SPACE.join((self.geom_type, self.name, "'s geom_type")),
                                GEOM_TYPES, data_type=str)
         if geom_type.lower() == "domain":
```

## mindflow/geometry/geometry_td.py

```diff
@@ -30,18 +30,18 @@
 
 class TimeDomain(Interval):
     """
     Definition of Time Domain.
 
     Args:
         name (str): name of the time domain.
-        start (Union[int, float]): start of the time domain. Default: 0.0.
-        end (Union[int, float]): end of the time domain. Default: 1.0.
-        dtype (numpy.dtype): Data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        start (Union[int, float]): start of the time domain. Default: ``0.0``.
+        end (Union[int, float]): end of the time domain. Default: ``1.0``.
+        dtype (numpy.dtype): Data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, TimeDomain
         >>> time_config = dict({
@@ -65,20 +65,20 @@
 
 
 class GeometryWithTime(Geometry):
     """
     Definition of geometry with time.
 
     Args:
-        geometry (Geometry): geometry
-        timedomain (TimeDomain): time domain
-        sampling_config (SamplingConfig): sampling configuration. Default: None.
+        geometry (Geometry): geometry.
+        timedomain (TimeDomain): time domain.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Raises:
-        ValueError: If `sampling_config` is not None but `sampling_config.time` is None .
+        ValueError: If `sampling_config` is not ``None`` but `sampling_config.time` is ``None`` .
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.geometry import generate_sampling_config, Rectangle, TimeDomain, GeometryWithTime
         >>> rect_with_time_config = dict({
@@ -229,30 +229,30 @@
         return samples
 
     def sampling(self, geom_type="domain"):
         """
         sampling points
 
         Args:
-            geom_type (str): geometry type: can be 'domain' or 'BC' or 'IC'. Default: 'domain'.
+            geom_type (str): geometry type: can be ``'domain'`` or ``'BC'`` or ``'IC'``. Default: ``'domain'``.
 
-                - 'domain', feasible domain of the problem.
-                - 'BC', boundary of the problem.
-                - 'IC', initial condition of the problem.
+                - ``'domain'``, feasible domain of the problem.
+                - ``'BC'``, boundary of the problem.
+                - ``'IC'``, initial condition of the problem.
 
         Returns:
             Numpy.array, if the with_normal property of boundary configuration is true, returns 2D numpy array with
                          boundary normal vectors. Otherwise, returns 2D numpy array without boundary normal vectors.
 
         Raises:
-            ValueError: If `config` is None.
-            KeyError: If `geom_type` is `domain` but `config.domain` is None.
-            KeyError: If `geom_type` is `BC` but `config.bc` is None.
-            KeyError: If `geom_type` is `IC` but `config.ic` is None.
-            ValueError: If `geom_type` is not `BC`, `IC` nor `domain`.
+            ValueError: If `config` is ``None``.
+            KeyError: If `geom_type` is ``'domain'`` but `config.domain` is ``None``.
+            KeyError: If `geom_type` is ``'BC'`` but `config.bc` is ``None``.
+            KeyError: If `geom_type` is ``'IC'`` but `config.ic` is ``None``.
+            ValueError: If `geom_type` is not ``'BC'``, ``'IC'`` nor ``'domain'``.
         """
         config = self.sampling_config
         check_param_type(config, _space.join((self.geom_type, self.name, "'s sampling_config")),
                          data_type=SamplingConfig)
         check_param_type_value(geom_type, _space.join((self.geom_type, self.name, "'s geom_type")),
                                GEOM_TYPES, data_type=str)
         if geom_type.lower() == "domain":
```

## mindflow/geometry/shapes/adapter.py

```diff
@@ -12,16 +12,16 @@
         shape (Shape): an object for sampling the points.
         name (str): name of the geometry.
         dim (int): number of dimensions.
         coord_min (Union[int, float, list[int, float], tuple[int, float], numpy.ndarray]):
             minimal coordinate of the geometry.
         coord_max (Union[int, float, list[int, float], tuple[int, float], numpy.ndarray]):
             maximal coordinate of the geometry.
-        dtype (numpy.dtype): Data type of sampled point data type. Default: numpy.float32.
-        sampling_config (SamplingConfig): sampling configuration. Default: None
+        dtype (numpy.dtype): Data type of sampled point data type. Default: ``numpy.float32``.
+        sampling_config (SamplingConfig): sampling configuration. Default: ``None``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
     """
     def __init__(self, shape, name, dim, coord_min, coord_max,
                  dtype=np.float32, sampling_config=None):
         self._shape = shape
```

## mindflow/geometry/shapes/shapes.py

```diff
@@ -75,19 +75,19 @@
 
 
 def derive_union_boundary(shapes, boundary_type):
     """Create of a union based on the boundary type.
 
     Args:
         shapes (list): A list of shape objects.
-        boundary_type (str): this can be 'uniform' or 'unweighted'.
+        boundary_type (str): this can be ``'uniform'`` or ``'unweighted'``.
 
-            - 'uniform', the expected number of samples in each boundary is
+            - ``'uniform'``, the expected number of samples in each boundary is
               proportional to the area (length) of the boundary.
-            - 'unweighted', the expected number of samples in each boundary is
+            - ``'unweighted'``, the expected number of samples in each boundary is
               the same.
 
     Returns:
         Union, Union of the input shapes.
     """
     if boundary_type == 'none':
         boundary = None
```

## mindflow/geometry/shapes/simplex.py

```diff
@@ -5,45 +5,46 @@
 import numpy as np
 
 from .shapes import Shape, derive_union_boundary
 
 
 class Segment(Shape):
     """Segment sampler."""
+
     def __init__(self, vertices):
-        x0, y0, x1, y1 = np.ravel(vertices)
-        self._slope = (y1 - y0)/(x1 - x0)
-        self._intercpet = (y0*x1 - y1*x0)/(x1 - x0)
-        self._x_min = min(x0, x1)
-        self._x_max = max(x0, x1)
-        super(Segment, self).__init__(volume=math.sqrt((x0 - x1)*(x0 - x1) + (y0 - y1)*(y0 - y1)))
+        vertices = np.asarray(vertices)
+        self._vector = vertices[1] - vertices[0]
+        self._point = vertices[0]
+        self._x_min, self._x_max = np.sort(vertices[:, 0])
+        self._y_min, self._y_max = np.sort(vertices[:, 1])
+        super(Segment, self).__init__(volume=math.hypot(*self._vector))
 
     def is_inside(self, pts):
-        x = pts[:, 0]
-        return (x >= self._x_min) & (x <= self._x_max) & self.is_on(pts)
+        return (pts[:, 0] >= self._x_min) & (pts[:, 0] <= self._x_max) & \
+            (pts[:, 1] >= self._y_min) & (pts[:, 1] <= self._y_max) & \
+            self.is_on(pts)
 
     def is_on(self, pts):
         """Check if ``x`` is on the line defined by the segment."""
-        x, y = pts.T
-        return np.isclose(y, self.line_equation(x))
+        return np.cross(pts - self._point, self._vector) == 0
 
     def sample(self, num_samps):
-        x = self._x_min + (self._x_max - self._x_min)*np.random.rand(num_samps, 1)
-        return np.hstack([x, self.line_equation(x)])
-
-    def line_equation(self, x):
-        return self._intercpet + self._slope*x
+        samps = np.random.rand(num_samps, 1)
+        return self._point + samps*self._vector
 
 
 class Simplex(Shape):
     """Simplex (triangle in 2D and tetrahedron in 3D) sampler."""
+
     def __init__(self, vertices, boundary_type='none'):
         vertices = self._validate(vertices)
         # Compute volume
-        volume = .5*abs(np.linalg.det(np.hstack([np.ones([len(vertices), 1]), vertices])))
+        volume = .5 * \
+            abs(np.linalg.det(
+                np.hstack([np.ones([len(vertices), 1]), vertices])))
         # Prepare boundary
         num_vertices = len(vertices)
         if num_vertices == 3:
             cls = Segment
         elif num_vertices == 4:
             cls = Triangle3D
         else:
@@ -103,27 +104,29 @@
         else:
             raise ValueError
         return vertices
 
 
 class Triangle3D(Shape):
     """3D Triangle sampler."""
+
     def __init__(self, vertices):
         vertices = self._validate(vertices)
         # Check if the given triangle can be reduced into 2D.
         dim_reduced = None
         for i_col in range(vertices.shape[1]):
             if np.allclose(vertices[:, i_col], vertices[0, i_col]):
                 dim_reduced = i_col
                 val_reduced = vertices[0, i_col]
                 break
 
         if dim_reduced is None:
             # Compute area
-            cross_product = np.cross(vertices[1] - vertices[0], vertices[2] - vertices[0])
+            cross_product = np.cross(
+                vertices[1] - vertices[0], vertices[2] - vertices[0])
             volume = .5*abs(np.linalg.norm(cross_product, ord=2))
             super(Triangle3D, self).__init__(volume)
             # Prepare transform matrix
             matrix = vertices
             if np.linalg.det(matrix) < 0:
                 matrix = np.asarray([matrix[1], matrix[0], matrix[2]])
             self._matrix = matrix
@@ -147,15 +150,16 @@
             & np.isclose(pts[:, self._dim_reduced], self._val_reduced)
 
     def sample(self, num_samps):
         if self._tri_reduced is None:
             return self.transform(self.sample_unit_triangle(num_samps))
 
         samps_reduced = self._tri_reduced.sample(num_samps)
-        samps = np.insert(samps_reduced, self._dim_reduced, self._val_reduced, axis=1)
+        samps = np.insert(samps_reduced, self._dim_reduced,
+                          self._val_reduced, axis=1)
         return samps
 
     def sample_unit_triangle(self, num_samps):
         """Uniformly sample points in the plane defined by (0, 0, 1), (1, 0, 0)
         and (0, 1, 0).
 
         This is equivalent to sample from a flat dirichlet distribution.
@@ -171,9 +175,10 @@
     def inverse_transform(self, pts):
         """Transform the given triangle into the unit triangle."""
         return np.matmul(pts, self._matrix_inv)
 
     def _validate(self, vertices):
         vertices = np.asarray(vertices).copy()
         assert vertices.shape == (3, 3)
-        # TODO Check the cases that three points lie on a line
+        if np.linalg.det(vertices) == 0:
+            raise ValueError("Three points lie on a line.")
         return vertices
```

## mindflow/loss/losses.py

```diff
@@ -79,15 +79,16 @@
 
 class RegularizedLossCell(nn.Cell):
     r"""
     L1/L2 regularized loss.
 
     Args:
         reg_params (Parameter): Parameter type tensor used for regularization.
-        reg_mode (str): type to compute the regularized loss function. Only ["l1", "l2"] are supported. Default: "l2".
+        reg_mode (str): type to compute the regularized loss function. Only [``"l1"``, ``"l2"``] are supported.
+            Default: ``"l2"``.
 
     Inputs:
         None.
 
     Outputs:
         Tensor. a scalar tensor with shape :math:`()`.
 
@@ -216,18 +217,18 @@
 
 class WaveletTransformLoss(nn.LossBase):
     r"""
     The multi-level wavelet transformation losses.
 
     Args:
         wave_level (int): The number of the wavelet transformation levels, should be positive integer.
-        regroup (bool): The regroup error combination form of the wavelet transformation losses. Default: "False".
+        regroup (bool): The regroup error combination form of the wavelet transformation losses. Default: ``"False"``.
 
     Inputs:
-        - **input** - tuple of Tensors. Tensor of shape :math:`(B H*W/(P*P) P*P*C)`, where B denotes the batch size.
+        - **input** - tuple of Tensors. Tensor of shape :math:`(B*H*W/(P*P), P*P*C)`, where B denotes the batch size.
           H, W denotes the height and the width of the image, respectively.
           P denotes the patch size. C denots the feature channels.
 
     Outputs:
         Tensor.
 
     Raises:
@@ -335,19 +336,19 @@
     root-mean-square error between :math:`x` and :math:`y` element-wise,
     where :math:`x` is the prediction and :math:`y` is the labels.
 
     For simplicity, let :math:`x` and :math:`y` be 1-dimensional Tensor with length :math:`N`,
     the loss of :math:`x` and :math:`y` is given as:
 
     .. math::
-        loss = \sqrt{\frac{\sum_{i=1}^{N}{(x_i-y_i)^2}}{sum_{i=1}^{N}{(y_i)^2}}}
+        loss = \sqrt{\frac{\sum_{i=1}^{N}{(x_i-y_i)^2}}{\sum_{i=1}^{N}{(y_i)^2}}}
 
     Args:
-        reduction (str): Type of reduction to be applied to loss. The optional values are "mean", "sum", and "none".
-            Default: "sum".
+        reduction (str): Type of reduction to be applied to loss. The optional values are ``"mean"``,
+            ``"sum"``, and ``"none"``. Default: ``"sum"``.
 
     Inputs:
         - **prediction** (Tensor) - The prediction value of the network. Tensor of shape :math:`(N, *)` where :math:`*`
           means, any number of additional dimensions.
         - **labels** (Tensor) - True value of the samples. Tensor of shape :math:`(N, *)`,  where :math:`*`
           means, any number of additional dimensions, same shape as the `prediction` in common cases.
           However, it supports the shape of `labels` is different from the shape of `prediction` and they should be
```

## mindflow/pde/flow_with_loss.py

```diff
@@ -20,30 +20,30 @@
 
 class FlowWithLoss:
     """
     Base class of user-defined data-driven flow prediction problems.
 
     Args:
         model (mindspore.nn.Cell): A training or test model.
-        loss_fn (Union[str, Cell]): Loss function. Default: "mse".
+        loss_fn (Union[str, Cell]): Loss function. Default: ``"mse"``.
 
     Raises:
         TypeError: If `modle` or `loss_fn` is not mindspore.nn.Cell.
         NotImplementedError: If the member function `get_loss` is not implemented.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     """
 
     def __init__(self, model, loss_fn='mse'):
         self.model = model
         self.loss_fn = get_loss_metric(loss_fn) if isinstance(loss_fn, str) else loss_fn
         check_param_type(model, "model", data_type=nn.Cell, exclude_type=bool)
-        check_param_type(loss_fn, "loss_fn", data_type=nn.Cell, exclude_type=bool)
+        check_param_type(self.loss_fn, "loss_fn", data_type=nn.Cell, exclude_type=bool)
 
     def get_loss(self, inputs, labels):
         """
         Compute the loss of the model.
 
         Args:
             inputs (Tensor): The input data of model.
@@ -55,15 +55,15 @@
 @jit_class
 class SteadyFlowWithLoss(FlowWithLoss):
     """
     Base class of user-defined steady data-driven problems.
 
     Args:
         model (mindspore.nn.Cell): A training or test model.
-        loss_fn (Union[str, Cell]): Loss function. Default: "mse".
+        loss_fn (Union[str, Cell]): Loss function. Default: ``"mse"``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindspore import Tensor, nn
@@ -121,18 +121,18 @@
 @jit_class
 class UnsteadyFlowWithLoss(FlowWithLoss):
     """
     Base class of unsteady user-defined data-driven problems.
 
     Args:
         model (mindspore.nn.Cell): A training or test model.
-        t_in (int): Initial time steps. Default: 1.
-        t_out (int): Output time steps. Default: 1.
-        loss_fn (Union[str, Cell]): Loss function. Default: "mse".
-        data_format (str): Data format. Default: "NTCHW".
+        t_in (int): Initial time steps. Default: ``1``.
+        t_out (int): Output time steps. Default: ``1``.
+        loss_fn (Union[str, Cell]): Loss function. Default: ``"mse"``.
+        data_format (str): Data format. Default: ``"NTCHW"``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> import numpy as np
         >>> from mindspore import Tensor
```

## mindflow/pde/pde_with_loss.py

```diff
@@ -37,14 +37,16 @@
     the pde residual. The data(e.g. inputs) used to solve the residuals is passed to the parse_node, and the residuals
     of each equation can be automatically calculated.
 
     Args:
         model (mindspore.nn.Cell): Network for training.
         in_vars (List[sympy.core.Symbol]): Input variables of the `model`, represented by the sympy symbol.
         out_vars (List[sympy.core.Function]): Output variables of the `model`, represented by the sympy function.
+        params (List[sympy.core.Function]): Parameters of the `model`, represented by the sympy function.
+        params_val (List[sympy.core.Function]): Values of the Parameters from optimizer.
 
     Note:
         - The member function, "pde", must be overridden to define the symbolic derivative equqtions based on sympy.
         - The member function, "get_loss", must be overridden to caluate the loss of symbolic derivative equqtions.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
@@ -102,21 +104,22 @@
             Item numbers of current derivative formula nodes: 3
         bc_eq: Derivative(u(x, t), t) + Derivative(u(x, t), x) - 2.0
             Item numbers of current derivative formula nodes: 3
         {'my_eq': Derivative(u(x, t), (t, 2)) + Derivative(u(x, t), (x, 2)) - 4.0}
         {'bc_eq': Derivative(u(x, t), t) + Derivative(u(x, t), x) - 2.0}
     """
 
-    def __init__(self, model, in_vars, out_vars):
+    def __init__(self, model, in_vars, out_vars, params=None, params_val=None):
         self.model = model
         self.jacobian = batched_jacobian(self.model)
         self.hessian = batched_hessian(self.model)
+        self.param_val = params_val
         pde_nodes = self.pde() or dict()
         if isinstance(pde_nodes, dict) and pde_nodes:
-            self.pde_nodes = sympy_to_mindspore(pde_nodes, in_vars, out_vars)
+            self.pde_nodes = sympy_to_mindspore(pde_nodes, in_vars, out_vars, params)
 
     def pde(self):
         """
         Governing equation based on sympy, abstract method.
         This function must be overridden, if the corresponding constraint is governing equation.
         """
         return None
@@ -129,17 +132,17 @@
 
     def parse_node(self, formula_nodes, inputs=None, norm=None):
         """
         Calculate the results for each formula node.
 
         Args:
             formula_nodes (list[FormulaNode]): List of expressions node can be identified by mindspore.
-            inputs (Tensor): The input data of network. Default: None.
+            inputs (Tensor): The input data of network. Default: ``None``.
             norm (Tensor): The normal of the surface at a point P is a vector perpendicular to the tangent plane of the
-                point. Default: None.
+                point. Default: ``None``.
 
         Returns:
             List(Tensor), the results of the partial differential equations.
         """
         max_order = 0
         for formula_node in formula_nodes:
             max_order = max(formula_node.max_order, max_order)
@@ -150,29 +153,34 @@
             jacobian = self.jacobian(inputs)
         elif max_order == 1:
             hessian = None
             jacobian = self.jacobian(inputs)
         else:
             hessian = None
             jacobian = None
-        data_map = {"inputs": inputs, "outputs": outputs, "jacobian": jacobian, "hessian": hessian, "norm": norm}
+
+        if self.param_val is None:
+            data_map = {"inputs": inputs, "outputs": outputs, "jacobian": jacobian, "hessian": hessian, "norm": norm}
+        else:
+            data_map = {"inputs": inputs, "outputs": outputs, "jacobian": jacobian, "hessian": hessian,
+                        "norm": norm, "params": self.param_val}
         res = []
         for formula_node in formula_nodes:
             cur_eq_ret = formula_node.compute(data_map)
             res.append(cur_eq_ret)
         return res
 
 
 class Burgers(PDEWithLoss):
     r"""
     Base class for Burgers 1-D problem based on PDEWithLoss.
 
     Args:
         model (mindspore.nn.Cell): Network for training.
-        loss_fn (Union[str, Cell]): Define the loss function. Default: mse.
+        loss_fn (Union[str, Cell]): Define the loss function. Default: ``"mse"``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.pde import Burgers
         >>> from mindspore import nn, ops
@@ -227,16 +235,16 @@
 class NavierStokes(PDEWithLoss):
     r"""
     2D NavierStokes equation problem based on PDEWithLoss.
 
     Args:
         model (mindspore.nn.Cell): network for training.
         re (float): reynolds number is the ratio of inertia force to viscous force of a fluid. It is a dimensionless
-            quantity. Default: 100.0.
-        loss_fn (Union[str, Cell]): Define the loss function. Default: mse.
+            quantity. Default: ``100.0``.
+        loss_fn (Union[str, Cell]): Define the loss function. Default: ``"mse"``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.pde import NavierStokes
         >>> from mindspore import nn, ops
@@ -308,15 +316,15 @@
 
 class Poisson(PDEWithLoss):
     r"""
     Base class for Poisson 2-D problem based on PDEWithLoss.
 
     Args:
         model (mindspore.nn.Cell): network for training.
-        loss_fn (Union[str, Cell]): Define the loss function. Default: mse.
+        loss_fn (Union[str, Cell]): Define the loss function. Default: ``"mse"``.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
         >>> from mindflow.pde import Poisson
         >>> from mindspore import nn, ops
```

## mindflow/pde/sympy2mindspore/parse_sympy.py

```diff
@@ -42,35 +42,35 @@
         for node in self.nodes:
             cur_node_rst = node.compute(data)
             rst.append(cur_node_rst)
 
         return sum(rst)
 
 
-def _make_nodes(equations, in_vars, out_vars):
+def _make_nodes(equations, in_vars, out_vars, params=None):
     graph_nodes = list()
     for name, formula in equations.items():
         formula_node = FormulaNode(name)
-        SympyTranslation(sympy.expand(formula), formula_node, in_vars, out_vars)
+        SympyTranslation(sympy.expand(formula), formula_node, in_vars, out_vars, params)
         graph_nodes.append(formula_node)
 
     return graph_nodes
 
 
-def sympy_to_mindspore(equations, in_vars, out_vars):
+def sympy_to_mindspore(equations, in_vars, out_vars, params=None):
     """
     The sympy expression to create an identifier for mindspore.
 
     Args:
         equations (dict): the item in equations contains the key defined by user and the value is sympy expression.
         in_vars (list[sympy.core.Symbol]): list of all input variable symbols, consistent with the dimension of the
             input data.
         out_vars (list[sympy.core.Function]): list of all output variable symbols, consistent with the dimension of the
             output data.
-
+        params (list[sympy.core.Function]): list of all parameter variable symbols.
     Returns:
         List([FormulaNode]), list of expressions node can be identified by mindspore.
 
     Supported Platforms:
         ``Ascend`` ``GPU``
 
     Examples:
@@ -87,9 +87,9 @@
         >>> print(len(res))
         eq1: x + y
             Item numbers of current derivative formula nodes: 2
         eq2: Derivative(u(x, y), x) + Derivative(u(x, y), y)
             Item numbers of current derivative formula nodes: 2
         2
     """
-    converted_equations = _make_nodes(equations, in_vars, out_vars)
+    converted_equations = _make_nodes(equations, in_vars, out_vars, params)
     return converted_equations
```

## mindflow/pde/sympy2mindspore/pde_node.py

```diff
@@ -141,14 +141,28 @@
         """compute the result of symbol"""
         input_data = data.get("inputs")
         ret = self.input_split(input_data)[self.in_var_idx]
         return ret
 
 
 @jit_class
+class ParamNode:
+    """Compute parameter terms in sympy expression"""
+    def __init__(self, params, param_var_idx=None):
+        self.param_split = ops.Split(-1, len(params))
+        self.param_var_idx = param_var_idx
+
+    def compute(self, data):
+        """compute the result of parameter"""
+        params_data = data.get("params")
+        ret = self.param_split(params_data)[self.param_var_idx]
+        return ret
+
+
+@jit_class
 class NetOutputNode:
     """Compute network function terms in sympy expression"""
     def __init__(self, out_vars, out_var_idx=None):
         self.output_split = ops.Split(1, len(out_vars))
         self.out_var_idx = out_var_idx
 
     def compute(self, data):
```

## mindflow/pde/sympy2mindspore/sympy_translation.py

```diff
@@ -18,26 +18,27 @@
 from __future__ import absolute_import
 
 import numpy as np
 import sympy
 from mindspore import Tensor, jit_class
 from mindspore import dtype as mstype
 
-from .pde_node import MINDSPORE_SYMPY_TRANSLATIONS, MulNode, NumberNode, SymbolNode
+from .pde_node import MINDSPORE_SYMPY_TRANSLATIONS, MulNode, NumberNode, SymbolNode, ParamNode
 from .pde_node import MSFunctionNode, NetOutputNode, DerivativeNode, PowNode, AddNode
 
 
 @jit_class
 class SympyTranslation:
     '''translate sympy expressions'''
-    def __init__(self, formula, formula_node, in_vars, out_vars):
+    def __init__(self, formula, formula_node, in_vars, out_vars, params=None):
         self.formula = formula
         self.formula_node = formula_node
         self.in_vars = in_vars
         self.out_vars = out_vars
+        self.params = params
         print(f"{self.formula_node.name}: {self.formula}")
         self._parse_node()
         print(f"    Item numbers of current derivative formula nodes: {len(self.formula_node.nodes)}")
 
     @staticmethod
     def _check_item_args(item_args):
         """check item args"""
@@ -96,14 +97,21 @@
 
         elif item.is_NumberSymbol:
             node = self._parse_number_symbol(item)
 
         elif item.is_Pow:
             node = self._parse_pow(item)
 
+        elif item.is_Add:
+            nodes = []
+            for cur_item in item.args:
+                cur_node = self._parse_item(cur_item)
+                nodes.append(cur_node)
+            node = AddNode(nodes=nodes)
+
         else:
             raise ValueError("For parsing sympy expression: {} is not supported!".format(item))
 
         return node
 
     def _parse_derivative(self, item):
         """parses derivative expression"""
@@ -164,16 +172,22 @@
             fn_inside_node = self._parse_item(item.args[0])
         function_node = MSFunctionNode(nodes=[fn_inside_node], fn=fn)
 
         return function_node
 
     def _parse_symbol(self, item):
         """parse symbol"""
-        in_var_idx = self.in_vars.index(item)
-        symbol_node = SymbolNode(self.in_vars, in_var_idx=in_var_idx)
+        if item in self.in_vars:
+            in_var_idx = self.in_vars.index(item)
+            symbol_node = SymbolNode(self.in_vars, in_var_idx=in_var_idx)
+        elif item in self.params:
+            para_var_idx = self.params.index(item)
+            symbol_node = ParamNode(self.params, param_var_idx=para_var_idx)
+        else:
+            raise ValueError("Inputs and Parameters are supported, but got {}".format(item))
         return symbol_node
 
     def _parse_mul(self, item):
         """parse mul"""
         nodes = []
         for cur_item in item.args:
             cur_node = self._parse_item(cur_item)
```

## mindflow/utils/__init__.py

```diff
@@ -10,11 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
 """init"""
 from .load_config import load_yaml_config
+from .log_utils import print_log, log_config
+from .time_utils import log_timer
 
-__all__ = ['load_yaml_config']
+__all__ = ['load_yaml_config', 'print_log', 'log_config', 'log_timer']
 
 __all__.sort()
```

## mindflow/utils/load_config.py

```diff
@@ -56,9 +56,9 @@
 
     Supported Platforms:
         ``Ascend`` ``CPU`` ``GPU``
     """
     # Read YAML experiment definition file
     with open(file_path, 'r') as stream:
         config = yaml.safe_load(stream)
-    config = _make_paths_absolute(os.path.dirname(file_path), config)
+    config = _make_paths_absolute(os.path.abspath('.'), config)
     return config
```

## Comparing `mindflow_gpu-0.1.0rc1.dist-info/METADATA` & `mindflow_gpu-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: mindflow-gpu
-Version: 0.1.0rc1
+Version: 0.2.0
 Summary: An AI framework for simulations of fluid dynamics
 Home-page: https://www.mindspore.cn/
+Download-URL: https://gitee.com/mindspore/mindscience/tags
 Author: The MindSpore Authors
 Author-email: contact@mindspore.cn
 License: Apache 2.0
-Download-URL: https://gitee.com/mindspore/mindscience/tags
 Project-URL: Sources, https://gitee.com/mindspore/mindscience
 Project-URL: Issue Tracker, https://gitee.com/mindspore/mindscience/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: numpy (>=1.17.0)
 Requires-Dist: scipy (>=1.7.0)
 Requires-Dist: matplotlib (>=3.1.3)
 Requires-Dist: easydict (>=1.9)
 Requires-Dist: sympy (>=1.10.1)
 
-UNKNOWN
-
-
```

## Comparing `mindflow_gpu-0.1.0rc1.dist-info/RECORD` & `mindflow_gpu-0.2.0.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 mindflow/__init__.py,sha256=TXo-tv-1C3XBsTj_5ECkn0dAYkQy6G1w7meEwIfcTyk,2948
 mindflow/setup.py,sha256=gIgiwITWji7gZZ6V-tdkhFOHtRPWM_gUnfNL_C7WHzI,2239
-mindflow/cell/__init__.py,sha256=BrKWKG3gDg4SN0Ngc5FMTJlaqJ8o_o59eSs0i7HZaS0,1012
-mindflow/cell/activation.py,sha256=6jWLECYhPj5B4bdjjOjJlY-gmEeva8Kwq-XOUS9Hnpw,3492
-mindflow/cell/basic_block.py,sha256=dJImfLsrQLDsyDCMKhunep7zyqXCi256M7FMSnBRgd0,21416
-mindflow/cell/utils.py,sha256=8oBQoPeE2hr4N9KVFgcsAC4o7Fd1EWwwBAvnqY2YyME,5040
-mindflow/cell/neural_operators/__init__.py,sha256=nIx7bANZjxy4w5fkz04FvA367wG0thcpM6dWDHxpqaU,811
-mindflow/cell/neural_operators/dft.py,sha256=fxTzkpq1NK7vnVSzXGRuLTRsKGD7XZDfZXXPYtnl64o,14413
-mindflow/cell/neural_operators/fno1d.py,sha256=i7CERdnou7ly7YhNNqE-VjWUxTbvNBkZ0B_dPsnxMMs,7688
-mindflow/cell/neural_operators/fno2d.py,sha256=jwaPsCPG_0NlhjMF6o7ro4k4mI1dw7U77JQ6LDZUPHM,9511
+mindflow/cell/__init__.py,sha256=qMOtCEbPtvTk6Fr7Oy45GUMb7vh4VeqX-cnaeTlVK2I,1115
+mindflow/cell/activation.py,sha256=KxGUv5vecZBOOnEGxTQhY6Bhl7IC8Ngsdyb_0ioQlgc,3516
+mindflow/cell/basic_block.py,sha256=w_wXOu4B9pzdnCbe8tLkvWbYgZYvncWtPYvdB41qv6w,21680
+mindflow/cell/unet2d.py,sha256=QVi5a0EpsoUQd3qlr91sJdZuNqVcmXSP8VTAdVow5ko,7064
+mindflow/cell/utils.py,sha256=w-p7dt12LJBXeZkhaFtje6QvaGAaIb0paaZZZZtje_k,5355
+mindflow/cell/neural_operators/__init__.py,sha256=T9Z4dvaPctm9uV9ziaWKUuxUILsOcXg7mK5D_c749i4,936
+mindflow/cell/neural_operators/dft.py,sha256=hav4hOUyKi8QKaeybarhpphogppoSRN59sQS2BkSzeU,34318
+mindflow/cell/neural_operators/fno.py,sha256=TlCZ3JYuCub_G4hO0bE4xMRe3Cgf_ZI-tOxW_jurxHM,28824
+mindflow/cell/neural_operators/kno1d.py,sha256=doAJQX7JDPMkT20J9Ac16IgGssEdIoB4ckruG8za20o,4667
+mindflow/cell/neural_operators/kno2d.py,sha256=DIF_O9vlU7RtgihjdnOfa1w5n-I-nfTwOB4QgpRZxYQ,4867
 mindflow/cell/neural_operators/m2k.py,sha256=xSGAtK8Ug7FaENq2fzVLEcjPFOP3bSL5kkizDboy7qI,2357
-mindflow/cell/neural_operators/pdenet.py,sha256=ByH1VDTRUyF4e-Y2Jd1QceVS-IDqitTPVsM4p5y7OW8,9671
+mindflow/cell/neural_operators/pdenet.py,sha256=5b2O3zA14kowwF7rmJ4FTXmR4XkI9Tryn2AabcejeXo,9695
+mindflow/cell/neural_operators/percnn.py,sha256=LlSEW8horAIiwUaQ18cv1Qc1mmUQFDO8Ns9C5w9pXcc,12845
 mindflow/cell/transformer/__init__.py,sha256=LGRSUi4bn1v8mLdF4_BUIOHo7xAXxybwRw68TFdLoHk,699
-mindflow/cell/transformer/layer.py,sha256=TNjH59BvOI9ZGli8fPWPKxob9HJeC6_9fCqZPrg0xPs,14042
-mindflow/cell/transformer/vit.py,sha256=7kUmbbrv2MXyUO-l2w9PgjFFUb3qjhymc7YkvTcXmz8,6350
+mindflow/cell/transformer/layer.py,sha256=DRi7JQe-5YuFHOoFviRt4-srN9yUr0-4ThBtgxhosVg,14082
+mindflow/cell/transformer/vit.py,sha256=UFybKSSXh-CTMQvYhAomTFOmoyXy97GeZw9vPColEgE,6402
 mindflow/cfd/__init__.py,sha256=1axgHkUrFAm9ZaBA-eeKbrSzRuI2JlTcQM8r4OHG1sI,971
 mindflow/cfd/mesh_info.py,sha256=cXkXSY9R53ljIcVLDQI2RyFoYIc7EQlIeMm4G_sdihM,2531
-mindflow/cfd/runtime.py,sha256=XMmg8yuYKed0_TD8BexTn3ndRG5w1sJP2-EqpePIFaw,4168
-mindflow/cfd/simulator.py,sha256=wYvZ3DylFho_839ih1JjuTP1In2yQoWIFM7uifF6F20,3298
-mindflow/cfd/utils.py,sha256=PVeDzdxVXreivuXyT5npMDSs-ex0tuuR9-Pfh3nXaCs,4714
-mindflow/cfd/visualization.py,sha256=Rluz_qBoDy6tiA53sCo3WYlTVNhIGpOZrpTkoHQOuMk,2956
+mindflow/cfd/runtime.py,sha256=Cx_x07ngP2tbZWvxPWHnCapNLd6t15x8cwzvauqrvAY,4178
+mindflow/cfd/simulator.py,sha256=Sf1xlzGlEX149xQzc-U0pagg56HHUCC20JtVnUTli1M,3302
+mindflow/cfd/utils.py,sha256=T3A65koGb76QkVMgXgmn3VKt94HWCzEL39K40ub3_i0,4746
+mindflow/cfd/visualization.py,sha256=iGkz0JHkx33OYTmnkk41lsQKWTeaYuBkfdN98IbbwQU,3320
 mindflow/cfd/boundary_conditions/__init__.py,sha256=gSGDxSyCCMobelAsMfexgeLQ48g3ax5-gRPOEjqDwVE,749
 mindflow/cfd/boundary_conditions/base.py,sha256=h24TmJ6QMJYoJEMnWJbUPApcIULiRVAd75mRdgMt0Gw,1165
 mindflow/cfd/boundary_conditions/boundary_manager.py,sha256=kw0gXzj0fmB8Lv0eBwTvZwKwpclnknTCVd3WYb77Lpw,2752
 mindflow/cfd/boundary_conditions/neumann.py,sha256=Ivpbbr6zW6vIQf0K3IsPkzhWWI16nF9O6fc9ao6Tf1w,1247
 mindflow/cfd/boundary_conditions/periodic.py,sha256=XKh-P8SsMIl4OSuaBoIuKCO4pDsn0sVFh6JLVJmwTV8,1173
 mindflow/cfd/boundary_conditions/symmetry.py,sha256=Rc-Bp-N6AkZDWfhx-fJ3D6NT2j-P543WZVmj2c6G1ck,1319
 mindflow/cfd/boundary_conditions/wall.py,sha256=yAvY3eEF5hquiP7HpU_DYswbHBl6tCkX-VS1pMBwxoE,1836
@@ -40,57 +43,64 @@
 mindflow/cfd/space_solver/derivative_computer/__init__.py,sha256=3NEC_ajo8tSHiUjf_A23fgWlVv2peQdSy5um1yfjXWc,1348
 mindflow/cfd/space_solver/derivative_computer/base.py,sha256=JF6sXm5ez5YZ463zW_eZcPSuwKWBqnFiSIcMKrS7qQg,1090
 mindflow/cfd/space_solver/derivative_computer/forth_order_central_derivative_computer.py,sha256=VBxRIUYxH7jrxrEySOSxwmdTTm1XDx7m12RygXjq3z4,2675
 mindflow/cfd/space_solver/derivative_computer/forth_order_face_derivative_computer.py,sha256=maLUFOIKN5RbjJ4qNEcyYJQnqCyn1_8t2drdJfrFJcU,2624
 mindflow/cfd/space_solver/interpolator/__init__.py,sha256=_HkXLJ9Ui7hA0J_xghXHTEL1O_wTALzpSLDaswn4KIU,1142
 mindflow/cfd/space_solver/interpolator/base.py,sha256=nmxIcnPSEhzEwfIHrOiswkyvPAhoR1c4pgVCA-yLXxs,1031
 mindflow/cfd/space_solver/interpolator/central_forth_order_interpolator.py,sha256=3WswrAzeejq6Csard6RbFNSgtLwPqh-g71_79dqgZKs,2576
-mindflow/cfd/space_solver/reconstructor/__init__.py,sha256=rsPuoU46unBG2n69tbNNaE6euTOqYFVsh8VybtkQyqE,1045
+mindflow/cfd/space_solver/reconstructor/__init__.py,sha256=vZD8tiFLIv9W18AqS8ywMvWbi54sxbYb8cur-IonPco,1135
 mindflow/cfd/space_solver/reconstructor/base.py,sha256=kAjWtFLBfNU6i3flcSSYK-oUm1q3or7aPk4CKTxu72Q,2064
+mindflow/cfd/space_solver/reconstructor/weno3.py,sha256=VQUGFQsiskdI8gmoObUA9fmJS0xOo68P4UL3oCKE8aI,4739
 mindflow/cfd/space_solver/reconstructor/weno5.py,sha256=vb4zG1jkSnURXP0YO8zPOIjsFkelFpWHPwS33sZKPzw,6315
-mindflow/cfd/space_solver/riemann_computer/__init__.py,sha256=YpZX6jeg3QS-lANhtBfH-V62qGkeDPi4wflZlvyyuGc,1114
+mindflow/cfd/space_solver/reconstructor/weno7.py,sha256=SQ2wybtYrNtAS4PqBVDqI69HCgQhwdWvBjbVQdogHG0,8658
+mindflow/cfd/space_solver/riemann_computer/__init__.py,sha256=_-6FZnhZG65sh3-M1D-4JuMYzU_RXCmyWYfGuYedIx4,1174
 mindflow/cfd/space_solver/riemann_computer/base.py,sha256=ECb6fegQdaTWiMmGUctkH-A4E70lY-sWTS2DneSwd-U,1021
+mindflow/cfd/space_solver/riemann_computer/hllc.py,sha256=Tw0JaTL_UKrwMeLqWPcSdALLft3nPTLZSKWhEbY5Tbw,6303
+mindflow/cfd/space_solver/riemann_computer/roe.py,sha256=hB3HZ5wZ0igytL3So5EqhCWB6c5wGbUBkziP-ItbZDI,15258
 mindflow/cfd/space_solver/riemann_computer/rusanov.py,sha256=iXeSRFDCLUM2ZQugFIwtGsWmOHu4YHfmIYPuiVMoK60,2374
-mindflow/cfd/space_solver/riemann_computer/rusanov_net.py,sha256=1iySNWVTLdeejvsbaVwrkCk4OZuRcM-Zr9Sz91jx_cY,3636
+mindflow/cfd/space_solver/riemann_computer/rusanov_net.py,sha256=eKhI_Xkhd_IBDq07W_bPhH5RUMHJ4lK6fsrd7j5itE0,3638
 mindflow/common/__init__.py,sha256=upo0ynjSiiHktNRoUbU7NZWiqsssowphuGpXGphYWsg,884
-mindflow/common/lr_scheduler.py,sha256=an2oztoguFZGUaWjWCma9K5PqQRlU-k3Lj0Hit9Hvkg,9966
-mindflow/common/math.py,sha256=V1S2Wr-VKsrCgD3FAp9Szax7Yovztd51WHkNNCQFEsw,2014
+mindflow/common/lr_scheduler.py,sha256=stDrJ9G9WU_Ro82aDepsDWf9PQ2t-nhuRazpHC2IdDc,10167
+mindflow/common/math.py,sha256=ohlYFYyvhGYI-O6_vGKPnYYO9eiPbtqk1DQTy82G1Qw,2331
 mindflow/data/__init__.py,sha256=izQBltxrsBnCWLiRehjnDcbGt4CgtRRe3B3ZH1HCjNk,1145
-mindflow/data/boundary.py,sha256=hOId7ryYGia77FEImGE0FQwcGO-yrLjtZ6dmx_BoEho,8430
-mindflow/data/data_base.py,sha256=jdmNts0djeL2rCf9LhPKxKdvEBrFVf44hE8HXJusZEg,5624
-mindflow/data/dataset.py,sha256=61_FCtrBZck4lWS2RD5d-2qY2h7I1ky4NR_MT_7UnoI,18758
-mindflow/data/equation.py,sha256=PJY3F-mlFowUFf2vB0ETQby7YO5BEOHoYkYhfiUfzq0,5436
-mindflow/data/existed_data.py,sha256=hf34-RugoI6_CT8w1wqAkITz2c2TBGrjofBzF1Ty-LI,6960
-mindflow/data/mind_dataset.py,sha256=R0z0g7SqN2DLgoAiqutrt2SZn0vfaaRQ5EoPBCUEASk,12556
-mindflow/geometry/__init__.py,sha256=TE9Tbh8ZgMqVJXZh_Koy3seBResF_R-S8r_QOIy-s6Q,1542
-mindflow/geometry/csg.py,sha256=k8aP7Q6Vrv2itpkHTXWIAAEHrejNwJI3qjRFPoK_3Uk,29673
-mindflow/geometry/geom_utils.py,sha256=5yjXUC_OZyb1t73W7SuGdJoHRsnShOsqOwD-uT64AVc,5593
-mindflow/geometry/geometry_1d.py,sha256=LD_sKnO8kEYZPKlN7pgSDBR--prwUkjJNWchzJcp7X8,2355
-mindflow/geometry/geometry_2d.py,sha256=SgNw4-gExOT2rifjjRShQzzilXIxbQ5vJzEZek6_QQA,15747
-mindflow/geometry/geometry_3d.py,sha256=TAQorKspveIJLvOC_SNYBTvGhtEbSToqsDyixh7QZdg,9383
-mindflow/geometry/geometry_base.py,sha256=KrOFoUjT87fGICu2TIJo9kD1VqMgQKyqwBRF48yNer4,11153
-mindflow/geometry/geometry_nd.py,sha256=ESTDzrzAySqrDAVMT1AEqC90bpImq9t8eaqyWm42Zss,15732
-mindflow/geometry/geometry_td.py,sha256=FVsMI0l82r751h1vEEYn_Zxf-INrnJkglYFhCMS1rNU,13857
+mindflow/data/boundary.py,sha256=66Zpk5PhdEhMtvo24k6xoiZiLp8xmKi4qM6g1AFnoQY,8533
+mindflow/data/data_base.py,sha256=5d5KjPkPi830I84OJOARN5PgJGOYFqNex60SquT_iAA,5744
+mindflow/data/dataset.py,sha256=oLfOTOBSl_FhsCkY5OxPJG23nWnL5ntYCAo24QIjzVM,19200
+mindflow/data/equation.py,sha256=0oiw8DZVqS0s9ZdXFOLat5Q274wlkKiyna6V0oxsEU8,5450
+mindflow/data/existed_data.py,sha256=WFkwudEYI9_6kbmDctgye-hFM-VGcNKMreDZxkgFDlw,7040
+mindflow/data/mind_dataset.py,sha256=rTln8tlH1j2YNOr_-X6G6U4VgrIQe9P9q4IGA-4L7sA,12848
+mindflow/geometry/__init__.py,sha256=q2BnEOhAiwJL5jDP5qceM1anqX2hpcpNx_OSeiUrurU,1567
+mindflow/geometry/csg.py,sha256=Y3P6HMCd7_6IXwkW73GxoSkEzV_fHJYJhZKnpHWIs-0,29715
+mindflow/geometry/geom_utils.py,sha256=e0DREsctxTgqv_HJwIsgXetyA4blQmeQEbRwUODhdXw,5587
+mindflow/geometry/geometry_1d.py,sha256=r5plDiQXxJYigqGr_mYWx5xgSsh9YOKjyB-HdL1O8Jc,2363
+mindflow/geometry/geometry_2d.py,sha256=ND9RE3hCZISt7rLneS-76ZOE0ic8ofVA4q3cYi5vEnE,17748
+mindflow/geometry/geometry_3d.py,sha256=4gGhzVAGCWniGCOl8tDtqXCpfpmhppKcgTbCzIb5K18,9475
+mindflow/geometry/geometry_base.py,sha256=PN09zTBTj-ESHNqpitUADN-1BIcyASWi6BHr3-pjYOs,11185
+mindflow/geometry/geometry_nd.py,sha256=ikorBJi2ReeVNhDaj-58PhF2o1GR0avXRm0YBEmXRNM,15897
+mindflow/geometry/geometry_td.py,sha256=oGy2UA3wgAiz8QFVMooAeo2QaY2TSp8K3cllJsbF2-k,13955
 mindflow/geometry/shapes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mindflow/geometry/shapes/adapter.py,sha256=mTvKsSX5LEne6NlNN7S-niwagok8sT7l4iAL05f4xtc,2337
+mindflow/geometry/shapes/adapter.py,sha256=uH3_U9qhRNdznGfUgxymFCsAs05hFuOAd-UzhP-2hl4,2346
 mindflow/geometry/shapes/pentagon.py,sha256=gJPQYiLgFZG3gIMLvC7x1DMAMX5Adpw-KpaDxuMla2s,2708
+mindflow/geometry/shapes/polygon.py,sha256=o0nwmjvomU2dQ6ovGzTqkOdl1rSspksWAO8VMGvE3VM,2617
 mindflow/geometry/shapes/rotating.py,sha256=FGvyxb1zWB-rU5wX5AY89PZ9zGtKzdZvNNH7laFATQc,7023
-mindflow/geometry/shapes/shapes.py,sha256=MW9zwntlaXL1WO9FTzXwm4vVM5Zkvnc1Rrw03z_hQJE,3146
-mindflow/geometry/shapes/simplex.py,sha256=yOz2oV_I3w2K3vxeOSffSWl81DAl07t3WaNit6BtejQ,6579
+mindflow/geometry/shapes/shapes.py,sha256=YRkemwXEzdKY46_VA76orFR3WWdC2cRfBSW9rUEurAU,3162
+mindflow/geometry/shapes/simplex.py,sha256=a5UEZWxGzyBDLks9n9q7g4fbTwZv2VnQPOMtKDm12ME,6650
 mindflow/loss/__init__.py,sha256=Idwts_ZyyrfnW-fO4dKi5OB0tBZwY--eNa6eeCCiwic,926
-mindflow/loss/losses.py,sha256=U46koRQhdssYssWJssR5UxEScrIE84omafg-lew-ips,14215
+mindflow/loss/losses.py,sha256=UBklFUm-Jp8-TUNJo91Fxcn2Q235fnJ49WPpJj4L72Q,14261
 mindflow/operators/__init__.py,sha256=hy7KSjr2lYOphcDKWFsRC_dorg-hg1pN0rUU_Sry-P8,804
 mindflow/operators/derivatives.py,sha256=YIdY_7ATiu-yo4AVZEn_V-_-SO_XdO8stxLvqBVOq-8,4635
 mindflow/pde/__init__.py,sha256=YM8P1nzOg0iXeqrzwUO-xNS1xtY9HH2X-X8pEOreKns,1056
-mindflow/pde/flow_with_loss.py,sha256=APeJJ1LuubzU-kFsFuw4cc50mb7MQHKkXjkk7e6daKE,8517
-mindflow/pde/pde_with_loss.py,sha256=ZvqB4DpxbcJMcmYsg3oBBxERFBjMkdG5VjpzR8dQvS8,15750
+mindflow/pde/flow_with_loss.py,sha256=z2QvK92dG0e_LS0Q5G1Y2ieXUF3UXG8xICsiZszSkVU,8546
+mindflow/pde/pde_with_loss.py,sha256=lg8WAfI_Ukyx2sY2CZLOvUDncWcMNjHDAXpSMam6Z1I,16271
 mindflow/pde/sympy2mindspore/__init__.py,sha256=5RLE_PvndYTEVJuIlTW1ZTJx3WQt9xqZ5U3RYOtDj2A,788
-mindflow/pde/sympy2mindspore/parse_sympy.py,sha256=fseIp_54XDmuiHbZBAyWiSU0ZbZO_HzhEf6ArLVlkBU,3087
-mindflow/pde/sympy2mindspore/pde_node.py,sha256=bLhUZDoIPKLq-N6MsxOS0lWEI-xm4PZEecrExeMTsXI,6012
-mindflow/pde/sympy2mindspore/sympy_translation.py,sha256=wihRFY3sCxNbNRukcY22CPkE0W5bjgdv6bfhQZ_IRhc,7047
-mindflow/utils/__init__.py,sha256=wQ4qkN7hAGT7s40JNpARrtnvoUp8EKiDdIgQQBd4uW0,773
+mindflow/pde/sympy2mindspore/parse_sympy.py,sha256=y30iFqfDknLnLkeSYi9KYSnj5eiYrKzql1qs5o64qLY,3212
+mindflow/pde/sympy2mindspore/pde_node.py,sha256=TF6kdVqpHAHLL6BrHxlEbnDBvphbBVI9mV1YovPELAM,6445
+mindflow/pde/sympy2mindspore/sympy_translation.py,sha256=VBiRsK_VBt_agg0MWqEXUKGqtwMxw_U9EohHBUXagz0,7632
+mindflow/utils/__init__.py,sha256=Sh1tbXCkHjZTvPFebMiS7iQob4ufgpsMDifFldns-bg,892
 mindflow/utils/check_func.py,sha256=gBOmFPc4hck4HrInrm66pun7PV7F5fSJ0nUgX9DFr88,5419
-mindflow/utils/load_config.py,sha256=QYXMkwBv3OJfx5ad3dmrXA91CWDyN6D45zqIBAhJpEc,1898
-mindflow_gpu-0.1.0rc1.dist-info/METADATA,sha256=_x4OycYXTGQSkYcv_6Amj8Ea7DVho9o2vSJigtF_n4s,691
-mindflow_gpu-0.1.0rc1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mindflow_gpu-0.1.0rc1.dist-info/top_level.txt,sha256=8LhUMCPy-q-NkiERuIGgzn7NBIZloxP4HLIvF8LZ48E,9
-mindflow_gpu-0.1.0rc1.dist-info/RECORD,,
+mindflow/utils/load_config.py,sha256=ZXxopFVgxXOYyKrUvI38MZkARsNWjzQLQ2dos8FVYuY,1892
+mindflow/utils/log_utils.py,sha256=w2swiq8Z10Keo3RASFSZpn0ymRGc2_7FIOm_LB1NgpI,1503
+mindflow/utils/time_utils.py,sha256=FUqRYHvqIMIGjEVw2DkWwXfKKAkXF7r3YSe3lWiLh8k,392
+mindflow_gpu-0.2.0.dist-info/METADATA,sha256=RmH_3YfRfmWFY7q2P_GnJNFEJsKFfTtxGC5PEykN4ZQ,660
+mindflow_gpu-0.2.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mindflow_gpu-0.2.0.dist-info/top_level.txt,sha256=8LhUMCPy-q-NkiERuIGgzn7NBIZloxP4HLIvF8LZ48E,9
+mindflow_gpu-0.2.0.dist-info/RECORD,,
```

