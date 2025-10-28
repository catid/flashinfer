# Changelog

## [0.1.0](https://github.com/catid/flashinfer/compare/v0.0.4...v0.1.0) (2025-10-28)


### Features

* add group gemm operators ([#282](https://github.com/catid/flashinfer/issues/282)) ([e08ba42](https://github.com/catid/flashinfer/commit/e08ba4226f694d5469cce4233f1854c965f05197))
* add mma instructions for fp8 ([#179](https://github.com/catid/flashinfer/issues/179)) ([d305798](https://github.com/catid/flashinfer/commit/d3057983e6d47e857ec3956de94eb11f62d9d83e))
* adding `sm_scale` field for all attention APIs ([#145](https://github.com/catid/flashinfer/issues/145)) ([85d4018](https://github.com/catid/flashinfer/commit/85d4018de4766dafd1be60cf6d953cd9236a4058))
* enable `head_dim=256` for attention kernels ([#132](https://github.com/catid/flashinfer/issues/132)) ([0372acc](https://github.com/catid/flashinfer/commit/0372acc44d0d393af7fd9fb3dcef0ff25953d4e1))
* mma rowsum for fp8 ([#180](https://github.com/catid/flashinfer/issues/180)) ([5af935c](https://github.com/catid/flashinfer/commit/5af935ca783d3487034110902c6406089c31acbc))
* pytorch api of fp8 kv-cache ([#156](https://github.com/catid/flashinfer/issues/156)) ([66ee066](https://github.com/catid/flashinfer/commit/66ee06683eaea7efe724c46df528ae47aa75eca2))
* support ALiBi ([#146](https://github.com/catid/flashinfer/issues/146)) ([383518b](https://github.com/catid/flashinfer/commit/383518bdf1824f68d33a2eaafd72a780f195bdd4))
* support any num_heads for get_alibi_slope ([#200](https://github.com/catid/flashinfer/issues/200)) ([b217a6f](https://github.com/catid/flashinfer/commit/b217a6fefb7bd091469467d32b8aedde4a25cad7))
* support cuda graph for batched multi-query(prefill/append) attention ([#275](https://github.com/catid/flashinfer/issues/275)) ([83ceb67](https://github.com/catid/flashinfer/commit/83ceb67a5773b0447f5f0344411abfdbc53cf5f4))
* support cuda graph for batched multi-query(prefill/append) attention ([#277](https://github.com/catid/flashinfer/issues/277)) ([24cc583](https://github.com/catid/flashinfer/commit/24cc583cb6b1a205aa8aad53f56472305b73f5f4))
* support custom attention mask in prefill/append attention kernels ([#266](https://github.com/catid/flashinfer/issues/266)) ([7304282](https://github.com/catid/flashinfer/commit/7304282a8068942100f8e59adff533ce28f4d3e5))


### Bug Fixes

* add python 3.9 wheels to ci/cd ([#114](https://github.com/catid/flashinfer/issues/114)) ([2d8807d](https://github.com/catid/flashinfer/commit/2d8807d1fb3359ace8a03b73c92bd0679b9d4b33))
* bugfix to pr 135 ([#136](https://github.com/catid/flashinfer/issues/136)) ([3d55c71](https://github.com/catid/flashinfer/commit/3d55c71a62052c590c130897d3a3db49b14fcc34))
* fatal bugfix in batch decode operator ([#177](https://github.com/catid/flashinfer/issues/177)) ([238563f](https://github.com/catid/flashinfer/commit/238563fb8fa5f3e5906bb951c3ee84659ed9265a))
* fix bugs introduced in [#132](https://github.com/catid/flashinfer/issues/132) ([#135](https://github.com/catid/flashinfer/issues/135)) ([9b7b0b9](https://github.com/catid/flashinfer/commit/9b7b0b913e1fbef7aac6351109911c7ac08a8904))
* fix FindThrust.cmake ([#161](https://github.com/catid/flashinfer/issues/161)) ([30fa584](https://github.com/catid/flashinfer/commit/30fa5843aeb1ac48816967a63db140cff6044e13))
* fix macro to suppress compilation warning ([#231](https://github.com/catid/flashinfer/issues/231)) ([94bcf6f](https://github.com/catid/flashinfer/commit/94bcf6f27b0e92da8b9f8fc2dffd0af31756e1da))
* fix python package dispatch error message ([#182](https://github.com/catid/flashinfer/issues/182)) ([8eed01c](https://github.com/catid/flashinfer/commit/8eed01c094ceb47375a1d4da8748c43a2947e959))
* fix the re expression in build wheel scripts ([#119](https://github.com/catid/flashinfer/issues/119)) ([2e982ea](https://github.com/catid/flashinfer/commit/2e982ea99fc4132dbb94aae994742fdc2da81a34))
* remove 8 from default page size ([#233](https://github.com/catid/flashinfer/issues/233)) ([62343e6](https://github.com/catid/flashinfer/commit/62343e66039a25cd49e89c8fe11fac153dd4bfee))
* to fix the re used in matching wheel names ([#121](https://github.com/catid/flashinfer/issues/121)) ([2b3fcde](https://github.com/catid/flashinfer/commit/2b3fcde434a4a4b44552977484c2cfcc906f429d))
* version names cannot include multiple `+` ([#118](https://github.com/catid/flashinfer/issues/118)) ([af6bd10](https://github.com/catid/flashinfer/commit/af6bd10db03fa1353699631f6b31eee52d343569))
* version naming issue ([#117](https://github.com/catid/flashinfer/issues/117)) ([c849a90](https://github.com/catid/flashinfer/commit/c849a90e6b6756a2ca87733782607796d8c7b85a))


### Performance Improvements

* initial cuda graph support ([#256](https://github.com/catid/flashinfer/issues/256)) ([7e9cc7f](https://github.com/catid/flashinfer/commit/7e9cc7ff42ca283c317061a877305d09a395fad2))
* multiple q by sm_scale in decode kernels ([#144](https://github.com/catid/flashinfer/issues/144)) ([660c559](https://github.com/catid/flashinfer/commit/660c559348ba9710d0d81b53f710f7e4951eee2b))

## [0.0.4](https://github.com/flashinfer-ai/flashinfer/compare/v0.0.3...v0.1.0) (2024-05-01)


### Features

* pytorch 2.3 support
* gpu sampling kernels (top-p, top-k)
* more gqa group sizes
* add mma instructions for fp8 ([#179](https://github.com/flashinfer-ai/flashinfer/issues/179)) ([d305798](https://github.com/flashinfer-ai/flashinfer/commit/d3057983e6d47e857ec3956de94eb11f62d9d83e))
* mma rowsum for fp8 ([#180](https://github.com/flashinfer-ai/flashinfer/issues/180)) ([5af935c](https://github.com/flashinfer-ai/flashinfer/commit/5af935ca783d3487034110902c6406089c31acbc))
* support any num_heads for get_alibi_slope ([#200](https://github.com/flashinfer-ai/flashinfer/issues/200)) ([b217a6f](https://github.com/flashinfer-ai/flashinfer/commit/b217a6fefb7bd091469467d32b8aedde4a25cad7))

### Bug Fixes

* fix python package dispatch error message ([#182](https://github.com/flashinfer-ai/flashinfer/issues/182)) ([8eed01c](https://github.com/flashinfer-ai/flashinfer/commit/8eed01c094ceb47375a1d4da8748c43a2947e959))

## [0.0.3](https://github.com/flashinfer-ai/flashinfer/compare/v0.0.2...v0.0.3) (2024-03-08)


### Features

* adding `sm_scale` field for all attention APIs ([#145](https://github.com/flashinfer-ai/flashinfer/issues/145)) ([85d4018](https://github.com/flashinfer-ai/flashinfer/commit/85d4018de4766dafd1be60cf6d953cd9236a4058))
* enable `head_dim=256` for attention kernels ([#132](https://github.com/flashinfer-ai/flashinfer/issues/132)) ([0372acc](https://github.com/flashinfer-ai/flashinfer/commit/0372acc44d0d393af7fd9fb3dcef0ff25953d4e1))
* pytorch api of fp8 kv-cache ([#156](https://github.com/flashinfer-ai/flashinfer/issues/156)) ([66ee066](https://github.com/flashinfer-ai/flashinfer/commit/66ee06683eaea7efe724c46df528ae47aa75eca2))
* support ALiBi ([#146](https://github.com/flashinfer-ai/flashinfer/issues/146)) ([383518b](https://github.com/flashinfer-ai/flashinfer/commit/383518bdf1824f68d33a2eaafd72a780f195bdd4))


### Bug Fixes

* bugfix to pr 135 ([#136](https://github.com/flashinfer-ai/flashinfer/issues/136)) ([3d55c71](https://github.com/flashinfer-ai/flashinfer/commit/3d55c71a62052c590c130897d3a3db49b14fcc34))
* fix bugs introduced in [#132](https://github.com/flashinfer-ai/flashinfer/issues/132) ([#135](https://github.com/flashinfer-ai/flashinfer/issues/135)) ([9b7b0b9](https://github.com/flashinfer-ai/flashinfer/commit/9b7b0b913e1fbef7aac6351109911c7ac08a8904))
* fix FindThrust.cmake ([#161](https://github.com/flashinfer-ai/flashinfer/issues/161)) ([30fa584](https://github.com/flashinfer-ai/flashinfer/commit/30fa5843aeb1ac48816967a63db140cff6044e13))


### Misc
* add stream argument in BeginForwardFunction of TVMWrapper ([#164](https://github.com/flashinfer-ai/flashinfer/pull/164)) ([fabfcb5](https://github.com/flashinfer-ai/flashinfer/tree/fabfcb5751dcc003137a5a7d2d5514f3afe2e302))


### Performance Improvements

* multiple q by sm_scale in decode kernels ([#144](https://github.com/flashinfer-ai/flashinfer/issues/144)) ([660c559](https://github.com/flashinfer-ai/flashinfer/commit/660c559348ba9710d0d81b53f710f7e4951eee2b))

## [0.0.2](https://github.com/flashinfer-ai/flashinfer/compare/v0.0.1...v0.0.2) (2024-02-17)


### Bug Fixes

* add python 3.9 wheels to ci/cd ([#114](https://github.com/flashinfer-ai/flashinfer/issues/114)) ([2d8807d](https://github.com/flashinfer-ai/flashinfer/commit/2d8807d1fb3359ace8a03b73c92bd0679b9d4b33))
* version names cannot include multiple `+` ([#118](https://github.com/flashinfer-ai/flashinfer/issues/118)) ([af6bd10](https://github.com/flashinfer-ai/flashinfer/commit/af6bd10db03fa1353699631f6b31eee52d343569))
* version naming issue ([#117](https://github.com/flashinfer-ai/flashinfer/issues/117)) ([c849a90](https://github.com/flashinfer-ai/flashinfer/commit/c849a90e6b6756a2ca87733782607796d8c7b85a))
