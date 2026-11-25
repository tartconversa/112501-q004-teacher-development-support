# 教师培训与名师支持资料基线

CSV 使用 UTF-8 编码，首行为字段名。资料仅提供项目所需的合成事实，空值代表来源尚未提供。

- `teachers.csv`：基线资料，首行为 `teacher,school,subject,valid_from,qualification`。
- `gaps.csv`：基线资料，首行为 `request,school,subject,students,priority,submitted_on`。
- `sessions.csv`：基线资料，首行为 `session,mentor,mode,date,minutes,capacity`。
- `history.csv`：基线资料，首行为 `teacher,session,attendance,completed_on`。

## 基线检查

运行 `python3 -m unittest discover -s tests -v` 可检查资料可读性、主键唯一性和版本锚点。该检查不实现业务分析能力。
