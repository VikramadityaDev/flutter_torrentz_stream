
# Flutter Torrentz Stream

[![pub](https://img.shields.io/pub/v/flutter_torrentz_stream.svg)](https://pub.dev/packages/flutter_torrentz_stream)

A flutter plugin to stream videos directly from torrentz magnet links.

This plugin is still under development and pull requests to make it better are heavily appreciated

## Few Important points to note before using this plugin
- Has only android support for now. (Help to implement iOS support is highly appreciated)
- Is still under development and APIs may go through breaking changes.
- Supports streaming and seeking videos while still being downloaded but is still experimental and has been tested to work on MX Player but does not work with `video_player` plugin.

## Installation

Add below line to your `pubspec.yaml` and run `flutter packages get`
```  
flutter_torrentz_stream: ^0.0.1
```

## Using in release builds

If you are using proguard in your app then add the below 2 lines to your proguard rules:
```
-keep class com.frostwire.jlibtorrent.swig.libtorrent_jni {*;}
-keep class com.frostwire.jlibtorrent.swig.** { *; }
```
