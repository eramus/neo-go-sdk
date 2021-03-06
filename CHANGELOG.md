# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this 
project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## 1.1.0 - 2017-08-19

### Added

- New `neo.WIF` struct.
- New `neo.PrivateKey` struct.
- Ability to convert a WIF into a PrivateKey, see example below.

```golang
wif := neo.NewWIF("L1QqQJnpBwbsPGAuutuzPTac8piqvbR1HRjrY5qHup48TBCBFe4g")

privateKey, err := wif.ToPrivateKey()
if err != nil {
  log.Fatal(err)
}

log.Println(privateKey.Value)
```

## 1.0.1 - 2017-08-19

### Added

- Link to GoDoc documentation.

### Changed

- Logo in README to new CoZ logo.

## 1.0.0 - 2017-08-16

### Changed

- Added badges to README.

## 0.2.0 - 2017-08-16

### Added

- Existing code from original repo.
- Full CI job.

## 0.1.0 - 2017-08-16

### Added

- Setup repo.
