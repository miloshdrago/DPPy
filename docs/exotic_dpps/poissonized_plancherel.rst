.. _poissonized_plancherel_measure:

Poissonized Plancherel measure
******************************

The poissonized Plancherel measure is a measure on partitions :math:`\lambda=(\lambda_1 \geq \lambda_2 \geq \cdots \geq 0)\in \mathbb{N}^{\mathbb{N}^*}`.
Samples from this measure can be obtained in the following way

- Sample :math:`N \sim \mathcal{P}(\theta)`
- Sample a uniform permutation :math:`\sigma\in \mathfrak{S}_N`
- Compute the sorting tableau :math:`P` associated to the RSK (`Robinson-Schensted-Knuth correspondence <https://en.wikipedia.org/wiki/Robinson%E2%80%93Schensted%E2%80%93Knuth_correspondence>`_) applied to :math:`\sigma`
- Consider only the shape :math:`\lambda` of :math:`P`.

Finally, the point process formed by :math:`\{\lambda_i - i + \frac12\}_{i\geq 1}` is a DPP on :math:`\mathbb{Z}+\frac12`.

.. :ref:`Fig. <poissonized_plancherel_plot>`

.. _poissonized_plancherel_plot:

.. plot:: plots/ex_plot_poissonized_plancherel.py

    Poissonized Plancherel measure

.. seealso::

    - :py:class:`~dppy.exotic_dpps.PoissonizedPlancherel`
    - :cite:`Bor09` Section 6
