.. _stationary_1-dependent_process:

Stationary 1-dependent process
******************************

A point process :math:`\mathcal{X}` on :math:`\mathbb{Z}` (resp. :math:`\mathbb{N}`) is called 1-dependent if for any :math:`A,B\subset \mathbb{Z}` (resp. :math:`\mathbb{N}`), such as the distance between :math:`A` and :math:`B` is greater than 1,

.. math::

    \mathbb{P}(A\cup B\subset \mathcal{X})
        =\mathbb{P}(A\subset \mathcal{X})
            \mathbb{P}(B\subset \mathcal{X}).

If :math:`\mathcal{X}` is stationary and 1-dependent then :math:`\mathcal{X}` forms a DPP.

The following 3 examples are stationary and 1-dependent process.

.. _carries_process:

Carries process
===============

The sequence of carries appearing when computing the cumulative sum (in base :math:`b`) of a sequence of i.i.d. digits forms a DPP on :math:`\mathbb{N}` with non symmetric kernel.

.. :ref:`Fig. <carries_process_plot>`

.. _carries_process_plot:

.. plot:: plots/ex_plot_carries_process.py

    Carries process

.. seealso::

    - :py:class:`~dppy.exotic_dpps.CarriesProcess`
    - :cite:`BoDiFu10`

.. _descent_process:

Descent process
===============

The descent process obtained from a uniformly chosen  permutation of  :math:`\{1,2,\dots,n\}` forms a DPP on :math:`\{1,2,\dots,n-1\}` with non symmetric kernel. It can be seen as the limit of the carries process as the base goes to infinity.

.. :ref:`Fig. <descent_process_plot>`

.. _descent_process_plot:

.. plot:: plots/ex_plot_descent_process.py

    Descent process

.. seealso::

    - :py:class:`~dppy.exotic_dpps.DescentProcess`
    - :cite:`BoDiFu10`

.. _limiting_descent_process:

Limiting Descent process for virtual permutations
==================================================

For non uniform permutations the descent process is not necessarily determinantal but in the particular case of virtual permutations with law stable under conjugation of the symmetric group the limiting descent process is a mixture of determinantal point processes.

.. :ref:`Fig. <virtual_descent_process_plot>`

.. _virtual_descent_process_plot:

.. plot:: plots/ex_plot_virtual_descent_process.py

    Virtual descent process

.. seealso::

    - :py:class:`~dppy.exotic_dpps.VirtualDescentProcess`
    - :cite:`Kam18`
