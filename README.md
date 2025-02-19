# Sunnyscribe Audio Transcription Editor

[简体中文](./README.zh-CN.md)

## 1. Product Overview

### Introduction
Sunnyscribe is a professional offline audio transcription and text editing tool. Developed using the Electron framework and integrated with the advanced FunASR and Whisper speech recognition engine, it provides an efficient and secure audio transcription solution. This software is particularly suitable for users who need to convert audio content to text and perform professional text editing.

### Key Features
1. Audio Transcription
   - Supports multiple mainstream audio formats: MP3, WAV, M4A, OGG
   - Offline transcription for data security
   - Fast transcription speed: approximately 20 minutes for 4 hours of audio
   - Supports speaker diarization and automatic punctuation

2. Text Editing and Proofreading
   - Professional audio-video synchronized proofreading interface
   - Supports text highlighting, annotations, and marking features
   - Editing history with multi-level undo/redo

3. File Management
   - Smart series/collection management system
   - Comprehensive file status tracking
   - Secure recycle bin functionality

4. Import/Export
   - Support for importing existing subtitle files for proofreading
   - Export support for multiple formats: TXT, SRT, JSON, etc.

## 2. System Requirements

### Hardware Requirements
- Processor: Intel Core i3 8th gen or higher (i5/i7 recommended)
- Memory: Minimum 16GB RAM (32GB recommended)
- Storage: At least 10GB free space on system drive
  • Software core: ~300MB
  • Python environment: ~8GB
- Display: Minimum 1920x1080 resolution
- Audio: Sound card device supporting audio playback

### Operating System and Environment Requirements
- Operating System
  • Windows 10 64-bit (version 1909 or higher)
  • Windows 11 all versions supported
  • 32-bit systems not supported

- Required Components
  • FFmpeg (for audio processing, included)
  • Python 3.9+ (for transcription engine, included)
  • Node.js 14+ (runtime environment, included)

- Network Requirements
  • Completely offline operation for data security

## 3. User Guide

1. Software Installation

   a) Download Installation Files
      - Sunnyscribe installer:
        • Core software including main program and basic components
        • Installation package size: ~300MB
        • Supports Windows 10 and above
      
      - Python environment package: 
      [Download Link1](https://pan.baidu.com/s/1D9-otJsSt_DWciq5t9D-XQ?pwd=sunn)
      [Download Link2](https://drive.google.com/drive/folders/129V4UkZTwik1D-AroUJEXkkPV6meqmBF)
        • Includes FunASR transcription engine and necessary Python environment
        • Environment package size: ~8GB
        • Recommend 3GB+ free disk space

   b) Installation Steps
      1. Install Sunnyscribe
         - Run Sunnyscribe.exe installer
         - Choose installation path (can be installed on any drive)
         - Follow installation wizard
         - Avoid Chinese characters in installation path

      2. Configure Python Environment
         - Extract downloaded Python environment package
         - Move extracted python_funasr folder to Sunnyscribe installation directory
         - Ensure correct path structure, e.g.:
           C:\Program Files\Sunnyscribe\python_funasr\

   c) Post-Installation Configuration
      - Software automatically checks Python environment on first launch
      - Proceeds to main interface if environment is correctly configured
      - Follow prompts to reconfigure if environment issues occur

2. Transcription and Import

   a) Audio Transcription
      - Click "Start Transcription" button on main interface
      - Select audio file in file dialog (supports mp3, wav, m4a, ogg)
      - Select transcription parameters (optional): speaker diarization, punctuation
      - Monitor transcription progress in real-time
      - File appears in All Files page upon completion

   b) Text Import
      - Click "Import File" button on main interface
      - Select subtitle file (supports JSON format proofreading files)
      - Select corresponding audio file (ensure matching)
      - System automatically verifies file compatibility
      - Imported file appears in All Files page

   c) File Management
      - All transcribed or imported files displayed as cards in "All Files" page
      - Manage files through search, sort, filter functions
      - Organize files into series for batch management
      - Recycle bin feature prevents accidental deletion

3. File Card Management
   a) Play Audio
      - Click play button(🎵) to play audio file directly
      - Support progress bar drag and volume adjustment
      - View corresponding text content during playback
   b) View Text
      - Click view button(📄) to open text view interface
      - Support text search and location
      - View complete transcribed/imported text content
   c) Proofreading Edit
      - Click edit button(✏️) to enter proofreading interface
      - Support audio-synchronized proofreading
      - Provide text annotation and note features
      - Support editing history with undo/redo
   d) Add to Series
      - Click series button(📁) to add file to series
      - Create new series or add to existing ones
      - Batch operations available for series files
   e) Delete File
      - Click delete button(🗑️) to move file to recycle bin
      - Support restore from recycle bin or permanent deletion
      - Confirmation prompt prevents accidental deletion

4. Proofreading and Editing
   a) Basic Functions
      - Click edit button(✏️) to enter proofreading interface
      - Support audio-synchronized proofreading
      - Text editing features:
        • Select and modify text
        • Copy, paste, delete functions
      - Annotation features:
        • Add, edit, delete notes
        • Text highlighting
        • Add comments and tags
      - History:
        • Multi-level undo and redo
        • Save editing records
      - Export features:
        • JSON format (with marked transcription data)
        • SRT format (subtitle file)
        • TXT format (text with timestamps)
        • CSV format (AU marked file)
        • DOCX format (word document with marks)
        • Export by filter conditions

   b) Audio-Synchronized Proofreading
      - Audio control:
        • Play/pause control
        • Volume adjustment
      - Progress control:
        • Drag progress bar to locate
        • Click progress bar for quick positioning
        • Click subtitle for quick positioning
        • Click speaker timeline for quick positioning
      - Text synchronization:
        • Auto-highlight current character during playback
        • Auto-scroll following playback progress
        • Click text to position audio

   c) Editing Assistance
      - Search function:
        • Text content search
        • Regular expression search
      - Filter function:
        • Filter by speaker
        • Filter by annotation type
      - Merge subtitles:
        • Custom character count for sentence merging
        • Support merge and undo
      - Modify speaker:
        • Double-click speaker for batch modification
        • Single-click subtitle mark to modify speaker

5. Recycle Bin Management
   a) Basic Functions
      - Click recycle bin button(🗑️) to enter management interface
      - List view of all deleted files
      - Display deletion time and original path information

   b) File Operations
      - Restore: Return file to original location
      - Permanent delete: Complete file removal
      - Batch operations: Support empty recycle bin

6. Software Settings
   a) Basic Settings
      - Interface settings
        • Language selection: Simplified Chinese
        • Font settings: type, size adjustment
      - Performance settings
        • Hardware acceleration toggle
        • Cache size adjustment (default 1GB)
        • Maximum concurrent tasks (default 3)

   b) Audio Settings
      - Audio input device selection
      - Audio output device selection
      - Audio device format

   c) Transcription Settings
      - Model configuration:
        • Acceleration device selection (CPU/GPU)
        • Concurrent threads (1-8)
      - Transcription parameters:
        • Batch size: 5-300 (default 300)
        • Sentence split interval: 300-1500ms (default 600ms)
        • Sentence merge interval: 300-2000ms (default 400ms)
        • Merge content length limit: 10-100 characters (default 24)
        • Punctuation list: customizable
      - One-click reset:
        • Quick restore default configuration

7. Licensing
   a) Software License Information
      - Software nature:
        • Sunnyscribe is commercially licensed software
        • Authorization code required for full functionality
      - Usage restrictions:
        • Unactivated version allows basic transcription and proofreading
        • Import/export features require activation
        • Each license supports one device
      - Trial version:
        • 1-month free trial activation code
        • Full software functionality during trial
        • Email sunnytranscribe@gmail.com for trial code
        • Purchase formal license after trial period

   b) License Acquisition Process
      1. Get machine code:
         • Open software, click "About" page
         • Click "Enter activation code" button
         • Copy displayed machine code
      2. Contact support:
         • Send machine code to: sunnytranscribe@gmail.com
         • Choose trial or purchase permanent license
         • Receive payment information (if purchasing)
      3. Activate software:
         • Enter received activation code
         • Click confirm to complete activation

   c) License Policy
      - License types:
        • Trial license: 1-month validity
        • Permanent license: lifetime validity
      - License scope: Single device
      - After-sales service:
        • Free version updates
        • Priority technical support
        • Dedicated customer service

8. Help and Support
   a) Online Support
      - Official email: sunnytranscribe@gmail.com
      - Response time: Within 24 hours on working days
      - Support content:
        • Purchase inquiries
        • Activation issues
        • Technical support
        • Feature suggestions

   b) FAQ
      - Installation related:
        • Python environment configuration
        • Software startup failure
        • Environment detection errors
      - Transcription related:
        • Transcription speed optimization
        • Audio format support
        • Transcription quality improvement
      - Activation related:
        • Activation code usage
        • Device change process
        • License renewal method