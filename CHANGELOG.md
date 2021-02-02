# Changelog

## [1.0.2] - 2021-02-02

### Added

- Created a change log

### Changed

- Performance improvement: Merged BrotliBitReader functions that read, peek, and skip bits from
the input buffer into a single read_bits function, reducing total number of calls and some 
redundancy in the inner loop processing
  
- Minor corrections in the README

## [1.0.1] - 2021-02-02

### Changed

- Removed all code that implemented use of intermediate streams and ringbuffers so that
decoding is just done as an in-memory transfer between the input and output buffers
  
- Streamlined the BroltliBitReader class and ensured that all access to it from other classes
happens via calls to a few functions that are intended to be parts of its API


## [1.0.0] - 2021-01-30

### Added

- Version number

### Changed

- Removed leading underscore from module name, as underscore is convention only for C/C++ modules

## 2021-01-29 - Initial implementation