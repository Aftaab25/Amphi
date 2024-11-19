Media-Player [https://github.com/Aftaab25/Media-Player]
    - Language: C++
    - Library: Qt
    - Minimum Viable Product (MVP):
        - Play audio (MP3, WAV, OGG) and video files (MP4, MKV, AVI)
        - Support Basic playback controls: Play, Pause, Stop, Seek, Volume control.
        - File Handling: Open files via file picker dialog
        - Display playback bar (progress slider)
        - FFmpeg for media decoding
        - OpenGL/DirectX (for video rendering) and a suitable Backend for audio (PortAudio/SDL2)
    - Intermediate
        - Playlist Management:
            - Create, save, and load playlists.
            - Display a list of tracks/videos for playback.
        - Keyboard Shortcuts:
            - Add shortcuts for playback controls, like spacebar for play/pause, arrows for seeking.
        - Customizable Settings:
            - Volume, playback speed, aspect ratio, and subtitle options.
        - Subtitles:
            - Load and display subtitle files (e.g., .srt).
        - Dark Mode:
            - Improve UI appearance for a modern look.
        - Audio/Video Format Support:
            - Expand supported formats using FFmpeg.
    - Advanced Features
        - Streaming Support:
            - Play media from URLs (HTTP, RTSP).
            - Add streaming protocols like HLS and DASH.
        - Audio/Video Filters:
            - Equalizer for audio.
            - Brightness, contrast, and color adjustments for video.
        - Advanced Subtitles:
            - Add support for subtitle styles (e.g., SSA/ASS)
        - Media Library:
            - Organize and manage a library of media files with metadata (e.g., ID3 tags for audio).
        - Cross-Device Sync:
            - Allow syncing playlists or playback positions across devices.
        - Customization:
            - Skins or themes for the UI.
        - Streaming and Casting:
            - Support for casting to devices like Chromecast or DLNA.
        - Codecs and Plugins:
            - Extend codec support using a plugin-based architecture.

Cross-Platform Considerations:
- Media Decoding: 
    - Use FFmpeg for decoding audio and video files. It’s cross-platform and supports almost all media formats.
- Audio Playback: Use a library like:
- PortAudio: Cross-platform audio library.
- SDL2: Provides robust multimedia features.
- Video Rendering:
    - Use OpenGL for cross-platform rendering.
    - Alternatively, use Vulkan or DirectX for specific platform optimizations.
- File Picker:
    - Use platform-specific libraries or a cross-platform GUI backend like ImGui File Dialog.
