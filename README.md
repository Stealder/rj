# Roblox Multi

## Tải bản mới nhất

- [RobloxMulti portable v36.0.0](https://github.com/Stealder/rj/releases/download/v36.0.0/RobloxMulti-portable-v36.0.0.zip)
- [auto_update.exe](https://github.com/Stealder/rj/releases/download/v36.0.0/auto_update.exe)
- [Danh sách bản phát hành](https://github.com/Stealder/rj/releases)

Giải nén toàn bộ ZIP và chạy `tool.exe`. Giữ thư mục `_internal` cạnh EXE.
Điền tài khoản và cấu hình trong thư mục `input` trên máy của bạn.

Để cập nhật, đặt `auto_update.exe` cạnh `tool.exe`, đóng tool rồi chạy updater.
Updater chỉ tải gói EXE và giữ lại cấu hình, tài khoản, dữ liệu hiện có.

Repo chỉ cung cấp bản chạy và hướng dẫn tải. Không công bố mã nguồn ứng dụng.
Các file tài khoản, API key, proxy, cookie và log cá nhân không đi kèm bản tải.

Auto Change: `mode: "time"` checks conditions alongside the timer. `interval_minutes: 0` disables the timer only. Qualified accounts are saved to output before their input lines are removed.

V28: only accounts selected for an active slot authenticate. Confirmed unauthorized cookies are archived to output/deadck.txt before removing their exact input line; network/proxy errors are retried.

V30: prevent console QuickEdit pauses, check every account timer before launches, and share launch attempts fairly within each proxy. After timed IP changes, wait 60 seconds then require HTTPS and UDP probes before account login; failed probes retry without another IP rotation.

V31: log stable process exit codes and other Roblox PIDs when a client disappears. This diagnostic release retains the v30 proxy readiness and timer fixes.

V32: verify copied client files against the installed Roblox version and restore missing or changed files. Use tool.exe --crash-report or menu [6] for Windows crash-module metadata. Does not claim to fix every cause of native access violations.

V33: pause new client launches when RobloxPlayerInstaller is running; do not multiply overlapping installers. Finish one official Roblox update with the tool closed before restarting multi-client mode. Debug reports now collect Installer/Bootstrapper logs as well as Windows crash metadata.

V34: honor an existing explicit Roblox EXE/version directory in roblox_exe. A sibling timestamp no longer overrides that selected path. Fallback discovery only applies when the selected player is missing; debug logs record the selected source EXE.

V35: optional roblox_version_lock requires a specific existing player and refuses version fallback. Locked rejoin uses private copies without RobloxPlayerInstaller.exe; the installed original is preserved. Default false; set true with your exact roblox_exe path. This does not override Roblox server version requirements.

V36: verify the selected build native files against its official installation manifest. Recover mismatched files into tool-owned runtime copies without altering the installed source. Check native bytes before every launch/rejoin; recover idle runtimes or select a new clean generation while live clients continue. Native recovery does not promise to fix unrelated access violations.
