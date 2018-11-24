# flac-converter

This is a Ruby command line application that can convert flac files to another format such as mp3, using ffmpeg

## Dependencies

- Ruby (developed using Ruby 2.5.1)
- ffmpeg (developed using ffmpeg 4.1)

This application requires that your system has both [Ruby](https://www.ruby-lang.org/en/) and [ffmpeg](https://ffmpeg.org/) installed.

Ruby offers [installers](https://www.ruby-lang.org/en/downloads/), as does [ffmpeg](https://ffmpeg.org/download.html#build-mac)

ffmpeg can also be installed using homebrew:

```bash
brew install ffmpeg
```

## Usage

```bash
./flac-converter [options]
```

Or place in an executable path such as /usr/local/bin and:

```bash
flac-converter [options]
```

### Optional arguments

* -s, --source-dir=SOURCE_DIR      Source directory (default: current directory)
* -t, --target-dir=TARGET_DIR      Target directory (default: current directory + /converted_files)
* -c, --codec=CODEC                Specify the codec (default: mp3)
* -r, --sample-rate=SAMPLE_RATE    Specify the sample rate (default: 44100)
* -b, --bit-rate=BIT_RATE          Specify the bit rate (default: 320k)
* -a, --channels=AUDIO_CHANNELS    Specify the audio channels (default: 2)
* -d, --delete                     Delete source file after conversion (defaut: false)
