# A1 提交清单（PROG2004 Assessment 1）

学号 25258567 ｜ 截止:2026-11-16 23:59

## 一、已经完成的部分

- [x] Java 项目全部源码（15 个类，`src/` 下），覆盖 Part 1–6
- [x] Javadoc 文档注释 + 行内注释（英文，与代码风格一致）
- [x] 编译验证:`javac -Xlint:all --release 11` 零警告；已实际运行并保存输出
- [x] `console-output.txt`：完整运行输出（261 行）
- [x] `README.md`：类职责表、各部分设计决策、四大支柱对应位置
- [x] `A1-25258567.zip`：整包（解压后是同名文件夹）

## 二、必须你自己完成的（作业硬性要求，不做会扣分）

1. **项目名 / zip 名**
   要求是 `A1-username`，username 是 **MySCU 用户名**，不是学号。
   如果你的 MySCU 用户名不是 `25258567`，把文件夹和 zip 都改名为 `A1-你的用户名`。
   同时把每个源文件头部的 `@author Dong Xinyang (25258567)` 改成你的名字和学号。

2. **GitHub 仓库（占 10% 评分，必须有提交历史）**
   - 新建 private 仓库，把整个项目推上去，邀请 tutor 和 unit assessor 作为 collaborator
   - 不要一次推完全部代码：按阶段拆分提交，建议 6–8 次，每次写清改了什么
     例：`Add Weekday enum and ClockTime value class` → `Add abstract HealthProfessional with validation`
     → `Add five specialised professional types with polymorphic service methods`
     → `Add Patient and Appointment with Comparable ordering`
     → `Add AppointmentManager with booking, filtering and cancellation`
     → `Add end-to-end demonstration in AssignmentOne`
     → `Add README with design rationale`
   - 提交时间要分布在评估期内（不要全部集中在同一天）

3. **WakaTime 报告**
   装 WakaTime 插件并真的编码，导出报告为 `A1-25258567-WakaTime.png/jpg/pdf` 一起提交。

4. **≤5 分钟视频**
   自己录、自己讲，禁止用 AI 生成。按下面顺序讲四大支柱，每条都做到:
   说出名字 → 用自己的话解释概念 → 指出代码里具体位置 → 说明为什么这里用它。

   | 支柱 | 建议讲的位置 |
   |---|---|
   | 封装 Encapsulation | `HealthProfessional.java`：private final 字段、构造器校验、`getWorkingDays()` 返回副本 |
   | 继承 Inheritance | `GeneralPractitioner/Nurse/Physiotherapist/Radiographer/Pharmacist extends HealthProfessional` |
   | 多态 Polymorphism | `AssignmentOne.printTeam()` 一个循环调 `deliverService()`；`Appointment` 只持有 `HealthProfessional` |
   | 抽象 Abstraction | `abstract class HealthProfessional` + 三个抽象方法；`Appointment implements Comparable` |

   时间分配建议:开场 30 秒 → 每个支柱 55–60 秒 → 结尾 20 秒演示一次运行结果。

5. **GenAI 声明（写在提交 comments 里）**
   Level 2 明确禁止 AI 写代码、写注释、做视频。请按实际情况如实填写；
   如果你用了 AI 辅助理解/调试，用这段:
   `I acknowledge that I have used Generative AI tools to complete this assessment in accordance with the conditions outlined in the Assessment Brief. I used [工具名] to [例如 explain OOP concepts / review my own code for bugs].`
   没用则用:
   `I acknowledge that I have not knowingly used GenAI to complete this assessment.`

6. **提交时还要附上**
   - `A1-username.zip`（Java 项目）
   - GitHub 仓库链接（写在 comments）
   - WakaTime 截图/报告
   - 视频链接（OneDrive 共享链接，写在 comments）

## 三、提交前最后自检（3 分钟）

- 解压 zip，用 IDE 打开，运行 `AssignmentOne`，确认输出与 `console-output.txt` 一致
- 确认所有类的 `@author` 是你的名字和学号
- 确认没有残留 `out/`、`.class`、`.idea/` 等无关文件（`out` 目录不要打进 zip）
- 视频长度 ≤ 5 分钟，能覆盖四大支柱各一处代码
- 截止前可多次提交，不要卡点
