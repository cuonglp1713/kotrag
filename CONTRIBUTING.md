## Note for Commit Message Convention

### Cấu trúc commit

```
<type>: <description> (REQUIRED)

[optional body] (OPTIONAL)

[optional footer] (OPTIONAL)
```

### Các loại commit (`type`)
- **feat**: Thêm tính năng mới
- **fix**: Sửa lỗi
- **docs**: Thay đổi tài liệu
- **refactor**: Tối ưu code, dọn dẹp code (không thêm tính năng, không sửa bug)
- **perf**: Cải thiện hiệu năng
- **test**: Thêm/sửa test case
- **build**: Thay đổi build system hoặc thư viện bên ngoài
- **ci**: Thay đổi liên quan CI/CD
- **chore**: Việc vặt, không ảnh hưởng trực tiếp code (vd: update `.gitignore`)
- **BREAKING_CHANGE**: Thay đổi lớn, gây ảnh hưởng ngược tới source code

### Description
- Ngắn gọn, súc tích, mô tả hành động (imperative form).  
  Ví dụ:
    - `feat: add RAG service interface`
    - `fix: prevent null pointer in embedding service`

### Body (tuỳ chọn)
- Dùng khi cần mô tả chi tiết hơn về commit.
- Tách với description bằng **một dòng trống**.

### Footer (tuỳ chọn)
- Dùng để tham chiếu issue, PR, hoặc giải thích giải pháp thay thế.
- Tách với body bằng **một dòng trống**.

---

## Ví dụ commit chuẩn

```
feat: add initial RAG pipeline structure

Introduce RagService interface and a basic implementation
with document loading and embedding functions. (OPTIONAL)

Future work: integrate Qdrant as vector store backend. (OPTIONAL)
```