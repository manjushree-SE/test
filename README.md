(shree_zarr) administrator-se@administrator-se:~$ pip install numpy==1.22.4 xarray==2023.1.0 zarr==2.13.3
Collecting numpy==1.22.4
  Downloading numpy-1.22.4.zip (11.5 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 11.5/11.5 MB 13.1 MB/s eta 0:00:00
  Installing build dependencies ... done
  Getting requirements to build wheel ... done
ERROR: Exception:
Traceback (most recent call last):
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/cli/base_command.py", line 106, in _run_wrapper
    status = _inner_run()
             ^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/cli/base_command.py", line 97, in _inner_run
    return self.run(options, args)
           ^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/cli/req_command.py", line 67, in wrapper
    return func(self, options, args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/commands/install.py", line 386, in run
    requirement_set = resolver.resolve(
                      ^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/resolver.py", line 95, in resolve
    result = self._result = resolver.resolve(
                            ^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py", line 546, in resolve
    state = resolution.resolve(requirements, max_rounds=max_rounds)
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py", line 397, in resolve
    self._add_to_criteria(self.state.criteria, r, parent=None)
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_vendor/resolvelib/resolvers.py", line 173, in _add_to_criteria
    if not criterion.candidates:
           ^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_vendor/resolvelib/structs.py", line 156, in __bool__
    return bool(self._sequence)
           ^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py", line 174, in __bool__
    return any(self)
           ^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py", line 162, in <genexpr>
    return (c for c in iterator if id(c) not in self._incompatible_ids)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py", line 53, in _iter_built
    candidate = func()
                ^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py", line 187, in _make_candidate_from_link
    base: Optional[BaseCandidate] = self._make_base_candidate_from_link(
                                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/factory.py", line 233, in _make_base_candidate_from_link
    self._link_candidate_cache[link] = LinkCandidate(
                                       ^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py", line 304, in __init__
    super().__init__(
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py", line 159, in __init__
    self.dist = self._prepare()
                ^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py", line 236, in _prepare
    dist = self._prepare_distribution()
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/resolution/resolvelib/candidates.py", line 315, in _prepare_distribution
    return preparer.prepare_linked_requirement(self._ireq, parallel_builds=True)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/operations/prepare.py", line 527, in prepare_linked_requirement
    return self._prepare_linked_requirement(req, parallel_builds)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/operations/prepare.py", line 642, in _prepare_linked_requirement
    dist = _get_prepared_distribution(
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/operations/prepare.py", line 72, in _get_prepared_distribution
    abstract_dist.prepare_distribution_metadata(
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/distributions/sdist.py", line 56, in prepare_distribution_metadata
    self._install_build_reqs(finder)
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/distributions/sdist.py", line 126, in _install_build_reqs
    build_reqs = self._get_build_requires_wheel()
                 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/distributions/sdist.py", line 103, in _get_build_requires_wheel
    return backend.get_requires_for_build_wheel()
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_internal/utils/misc.py", line 702, in get_requires_for_build_wheel
    return super().get_requires_for_build_wheel(config_settings=cs)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py", line 196, in get_requires_for_build_wheel
    return self._call_hook(
           ^^^^^^^^^^^^^^^^
  File "/home/administrator-se/shree_zarr/lib/python3.12/site-packages/pip/_vendor/pyproject_hooks/_impl.py", line 402, in _call_hook
    raise BackendUnavailable(
pip._vendor.pyproject_hooks._impl.BackendUnavailable: Cannot import 'setuptools.build_meta'
(shree_zarr) administrator-se@administrator-se:~$ ^C
(shree_zarr) administrator-se@administrator-se:~$ ^C
(shree_zarr) administrator-se@administrator-se:~$ 

