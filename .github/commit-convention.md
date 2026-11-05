# Commit Convention

Format: `<type>(<scope>): <subject>`

## Type
- feat: tính năng mới
- fix: sửa lỗi
- refactor: thay đổi code, không đổi hành vi
- test: thêm/sửa test
- docs: tài liệu, ADR
- chore: cấu hình, build, CI, dependency

## Scope
Tên module: order, payment, ledger, notification, reconciliation, shared.
Bỏ scope nếu thay đổi không thuộc module nào.

## Rules
- Subject bằng tiếng Anh, dạng mệnh lệnh ("add", không "added"), không viết hoa chữ đầu, không dấu chấm cuối, tối đa 50 ký tự
- Body (nếu có): cách subject 1 dòng trống, giải thích WHY, không lặp lại WHAT
- Tham chiếu issue ở cuối body: `Refs #12` hoặc `Closes #12`

## Examples
feat(payment): verify SePay webhook signature
fix(order): prevent expired order from being marked paid
docs(adr): add ADR-0001 use PostgreSQL