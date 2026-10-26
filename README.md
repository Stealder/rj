# Roblox Multi

## Tải bản mới nhất

- [RobloxMulti portable v28.0.0](https://github.com/Stealder/rj/releases/download/v28.0.0/RobloxMulti-portable-v28.0.0.zip)
- [auto_update.exe](https://github.com/Stealder/rj/releases/download/v28.0.0/auto_update.exe)
- [Danh sách bản phát hành](https://github.com/Stealder/rj/releases)

Giải nén toàn bộ ZIP và chạy `tool.exe`. Giữ thư mục `_internal` cạnh EXE.
Điền tài khoản và cấu hình trong thư mục `input` trên máy của bạn.

Để cập nhật, đặt `auto_update.exe` cạnh `tool.exe`, đóng tool rồi chạy updater.
Updater chỉ tải gói EXE và giữ lại cấu hình, tài khoản, dữ liệu hiện có.

Repo chỉ cung cấp bản chạy và hướng dẫn tải. Không công bố mã nguồn ứng dụng.
Các file tài khoản, API key, proxy, cookie và log cá nhân không đi kèm bản tải.

Auto Change: `mode: "time"` checks conditions alongside the timer. `interval_minutes: 0` disables the timer only. Qualified accounts are saved to output before their input lines are removed.

V28: only accounts selected for an active slot authenticate. Confirmed unauthorized cookies are archived to output/deadck.txt before removing their exact input line; network/proxy errors are retried.
