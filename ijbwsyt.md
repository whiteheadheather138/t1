代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://3g.sjlbkw.cn/Article/details/gqdvjujgu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gijqoppip.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gvikmwwcl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/germmztbc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gtgspdzep.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.bbcook.cn/Article/details/gssmhxgfm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/gylyrehsw.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gxihvkzoh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gykcmvxzu.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/grmaheugr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.tarul.cn/Article/details/gzsgwoeko.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gbdybiury.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.vehdjk.com/Article/details/gytlmfhgt.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/glixpfubk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gryiakkvm.sHtML

[Q53] 按条件删除
来源：http://m.share.yfazqb.com/Article/details/gjwostjgi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gnrgdlvte.sHtML

[Q54] 清空表
来源：http://m.share.vehdjk.com/Article/details/ghyqloxxa.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gleuugmpf.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gffnxnart.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gvndstjhi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.epnwcf.com/Article/details/gvrstmjqn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gtejfhueg.sHtML

[Q57] 行号
来源：http://read.share.vehdjk.com/Article/details/gbpvosozl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpwdovhbx.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gjvnxhhzi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gbjumhmnk.sHtML

[Q59] 分组内累计
来源：http://wap.epnwcf.com/Article/details/gsnvsuqfc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gcdfmvhxc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/gexeikrgz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gdgmynyua.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.bbcook.cn/Article/details/gdawdwqtq.sHtML

[Q61] 移动平均
来源：http://read.share.vehdjk.com/Article/details/gwyherspm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gowazhskc.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/gvrozbgoy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/geyreuhst.sHtML

[Q63] 开启事务
来源：http://mobile.vehdjk.com/Article/details/gdcpodfkg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.bbcook.cn/Article/details/gqukvhqxx.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gjxrbooqj.sHtML

COMMIT;
来源：http://www.share.vehdjk.com/Article/details/gegimpcyi.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/gnckomnti.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gtotqnldr.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/ggpdkqycr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/gqvvzyiam.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/gtaoacbxu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/gxmibmdmu.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/ggqspvoph.sHtML

SAVEPOINT sp1;
来源：http://read.share.bbcook.cn/Article/details/goqfflgno.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gxnrfxubi.sHtML

[Q69] 查看执行计划
来源：http://www.share.vehdjk.com/Article/details/gyvstcbyg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/gmngvzocy.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gsunperek.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/grbisoehw.sHtML

[Q71] 查看建表语句
来源：http://www.share.epnwcf.com/Article/details/glplssbqf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.tarul.cn/Article/details/gxguvjcen.sHtML

[Q72] 查看索引
来源：http://www.blog.sjlbkw.cn/Article/details/ggdjdlrxd.sHtML

SHOW INDEX FROM users;
来源：http://read.share.epnwcf.com/Article/details/gjtiluapu.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gfccgmtif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gxgzkyejv.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/gjaucsnps.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fktsv.cn/Article/details/gffrjrpys.sHtML

[Q75] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/giaruxriy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gzilfsxpp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.vehdjk.com/Article/details/gjsanwthh.sHtML

[Q76] 按天统计
来源：http://blog.epnwcf.com/Article/details/gzcszwrmp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/glhgzabpz.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gbmtpbwhy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.vehdjk.com/Article/details/gsashdkjx.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gdzyhgdog.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.epnwcf.com/Article/details/gfvpilyvi.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gnzqmovuc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/gpulbfdoa.sHtML

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/gylfwowhb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gvnuvdkyt.sHtML

[Q81] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gmcelccrf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.tarul.cn/Article/details/gpmvqwmkd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gvwjwavtm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gugovpefy.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gvjeolyrh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/glcbsxcwe.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/ggcuhqtqj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gzxuzcqds.sHtML

[Q85] 数值取整
来源：http://www.blog.bbcook.cn/Article/details/glxgyxtas.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/ghhpfvegt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/gmigarhle.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/gcagxihsd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gcjwotfou.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/gbycbqwuu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/ghmvstvvz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.tarul.cn/Article/details/gtcjbxlaz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/ghukcsejq.sHtML

[Q89] 判断表是否存在
来源：http://3g.sjlbkw.cn/Article/details/gaosdynbl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gvcsesbod.sHtML

[Q90] 生成序号列
来源：http://baike.fktsv.cn/Article/details/gmoaonpnz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fktsv.cn/Article/details/glyvflumx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdxdkfhov.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/gmnmfohrd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvanknpwn.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gikqzzbjw.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gvkjzhmlu.sHtML

set -euo pipefail
来源：http://wap.sjlbkw.cn/Article/details/gvwhhbpav.sHtML

[R02] 变量赋值与使用
来源：http://3g.fktsv.cn/Article/details/gyilzolxb.sHtML

name="Tom"; echo "$name"
来源：http://blog.yfazqb.com/Article/details/glwjnpepb.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/gplppupba.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gmealsshz.sHtML

[R04] 位置参数
来源：http://3g.yfazqb.com/Article/details/gbrmcihpo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/gajukjzun.sHtML

[R05] 参数默认值
来源：http://m.share.yfazqb.com/Article/details/gdilxaarj.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/gytardvjs.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gkltevwaw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gytlhrvdq.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/goblsycsp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/ggltommzv.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gtadegosz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fktsv.cn/Article/details/gqxgoogmj.sHtML

[R09] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gmmzunjvs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gwczvqvld.sHtML

[R10] 正则匹配
来源：http://blog.epnwcf.com/Article/details/gilffjumz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gxkmcqqwh.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/godpuoefw.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/geejiokgv.sHtML

start) echo "启动" ;;
来源：http://baike.fktsv.cn/Article/details/gkpwdgaay.sHtML

stop)  echo "停止" ;;
来源：http://m.share.epnwcf.com/Article/details/gljlwpfvb.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gehfbidhy.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/ghxhcfdlj.sHtML

[R12] for 遍历文件
来源：http://3g.yfazqb.com/Article/details/gijkdmsvj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fktsv.cn/Article/details/gxudbtteg.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/grijphemu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gakirmoiz.sHtML

[R14] C 风格 for
来源：http://baike.vehdjk.com/Article/details/guitikggf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gddcppuey.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gejljawob.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/gobuckalv.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gduguhter.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gsitionab.sHtML

[R17] 数组定义与取值
来源：http://baike.yfazqb.com/Article/details/gqgnofqwm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/gjujljpzl.sHtML

[R18] 遍历数组
来源：http://mobile.fktsv.cn/Article/details/gtxkcusqp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.tarul.cn/Article/details/gpqfyoxit.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/ghefucdkx.sHtML

echo "${#arr[@]}"
来源：http://m.share.sjlbkw.cn/Article/details/gptwcezaf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fktsv.cn/Article/details/gqwnnojes.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/gqouikena.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gzcudtufi.sHtML

echo "${#s}"
来源：http://baike.tarul.cn/Article/details/gwvnpwfzz.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/grdrurtex.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gqipuofqc.sHtML

[R23] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gcxxlzkto.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/geinnrfbg.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/genuwwhmn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.tarul.cn/Article/details/ganhkunfb.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gwpgjixhs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/ggaqzfiqs.sHtML

[R26] 命令替换
来源：http://m.share.yfazqb.com/Article/details/gqtoyjmpb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gvvwlmnjj.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gddylqoqr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.sjlbkw.cn/Article/details/ggqviosrn.sHtML

[R28] 浮点运算
来源：http://blog.bbcook.cn/Article/details/gwsfgslyd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.yfazqb.com/Article/details/gmjskicbi.sHtML

[R29] 定义函数
来源：http://baike.fktsv.cn/Article/details/gkyhrhmlj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/gtzukwxkk.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/ggwqikuca.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.tarul.cn/Article/details/gcladycts.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gzjeojtyy.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.yfazqb.com/Article/details/gzdtkwizt.sHtML

[R32] 参数个数校验
来源：http://mobile.sjlbkw.cn/Article/details/gktnnyxdd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gelswtisy.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/ggkoyzmry.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.tarul.cn/Article/details/goibyyfsp.sHtML

[R34] 退出时清理
来源：http://www.blog.bbcook.cn/Article/details/gnmetggbz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gzddjgmku.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gpejpsxtr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gdfoazzyg.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gqjhehecq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.vehdjk.com/Article/details/gekpcfpob.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gwnddiixg.sHtML

files=$(ls -1)
来源：http://read.share.yfazqb.com/Article/details/gzzxmozsg.sHtML

[R38] 管道串联
来源：http://m.share.epnwcf.com/Article/details/ggzwyzjmv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gjetdzfqe.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.vehdjk.com/Article/details/ghhwpwgfa.sHtML

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/gjrcayhwd.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/gooksexri.sHtML

echo "log" >> out.log
来源：http://www.m.share.epnwcf.com/Article/details/gtaghtboh.sHtML

[R41] 丢弃输出
来源：http://3g.vehdjk.com/Article/details/gtgotthru.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gcvepmrtk.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/glqydniiz.sHtML

wc -l < a.txt
来源：http://read.share.tarul.cn/Article/details/girudmntf.sHtML

[R43] 按名字查找文件
来源：http://www.share.yfazqb.com/Article/details/gotozezrs.sHtML

find . -name "*.log" -type f
来源：http://wap.yfazqb.com/Article/details/gpcwnukaz.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fktsv.cn/Article/details/gaszehbhk.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gknlaufpa.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/gmrrwzirb.sHtML

find . -name "*.tmp" -delete
来源：http://wap.sjlbkw.cn/Article/details/gtlqhizbj.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gjyskbagh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gfpecgnud.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/ghtbjkrsi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gztjflycd.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/ggpaintca.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.tarul.cn/Article/details/gbrzkggfn.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/gkataeoyb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/gykdxnslb.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gxbptewrf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.bbcook.cn/Article/details/garrlzuor.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gvaqsjpil.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gntkgwfms.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/gbqsulpjc.sHtML

wc -l a.txt
来源：http://www.share.tarul.cn/Article/details/gsngcjtht.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.epnwcf.com/Article/details/gvzlzxjrc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.vehdjk.com/Article/details/gyksdnqqy.sHtML

[R54] 比较两个文件
来源：http://baike.bbcook.cn/Article/details/gdktpopyz.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gzyjeoxbr.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/gzuqguwjh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/gvrrguiuc.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/gqmcrwxxl.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/glugnwbba.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gsejgiixg.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gnvxxvyfs.sHtML

[R58] 下载文件
来源：http://mobile.epnwcf.com/Article/details/gebxsspmr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.tarul.cn/Article/details/ghqsmytsq.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gjjqadmsa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gsajwqarh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/ghtrrqovn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyayeebe.sHtML

[R61] 磁盘占用
来源：http://mobile.sjlbkw.cn/Article/details/ghmtlarfc.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gxfbymlpc.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gdgewfsww.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/gvdqfirob.sHtML

[R63] 内存与进程
来源：http://blog.bbcook.cn/Article/details/gtohozcil.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gwtmhudda.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gmisewkwq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gkdajlmoa.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/glrwgcgtp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.yfazqb.com/Article/details/gjcyrfuhz.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gebtgxuem.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/ggpwoiyec.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/gvtjctgdy.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gkunlqien.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gexiujgli.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.yfazqb.com/Article/details/gcdiwglrr.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gykfrhppc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fktsv.cn/Article/details/gcwvldauy.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/gylvqcqwx.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gtnlyjddo.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gmpkjafos.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/genkwpsuu.sHtML

[R72] 等待端口就绪
来源：http://www.blog.vehdjk.com/Article/details/gwawcwrdj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gpykzsdao.sHtML

[R73] 分割大日志
来源：http://3g.fktsv.cn/Article/details/gdfsoxdda.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/gnsyegpcu.sHtML

[R74] 批量重命名
来源：http://read.share.vehdjk.com/Article/details/gqvdmfirw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/gloxuynvr.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gvvkotaag.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/gizrxmwdo.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/gptowizst.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gfswhopln.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gzlfuraez.sHtML

read -rp "请输入: " ans
来源：http://m.share.fktsv.cn/Article/details/gggxjejgj.sHtML

[R78] 交互式菜单
来源：http://baike.fktsv.cn/Article/details/gbmiiyuxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gfbqghizl.sHtML

[R79] 解析命令行选项
来源：http://www.blog.epnwcf.com/Article/details/gufwfrjnf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gsuslbbee.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gscvawmrf.sHtML

time ./run.sh
来源：http://baike.fktsv.cn/Article/details/gqnjyevok.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggwroznkl.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gvhadkprw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpodqkqsm.sHtML

[S01] C：Hello World
来源：http://blog.vehdjk.com/Article/details/gngvrpdpn.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/gvjdvpmtq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/giowqovao.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.yfazqb.com/Article/details/gpocvrsuv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.tarul.cn/Article/details/glwvrfnio.sHtML

[S03] C：读入整数
来源：http://blog.vehdjk.com/Article/details/ghmdrzkhv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.tarul.cn/Article/details/gufxmnyqw.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/gmukclvmn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/gmfbigkiy.sHtML

[S05] C：字符串长度
来源：http://www.share.fktsv.cn/Article/details/gpasekhgb.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/gdolekalj.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gnwwbwklv.sHtML

strcmp(a, b) == 0
来源：http://wap.tarul.cn/Article/details/gxyggosqv.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/grxyxrfkz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/glbrggzfg.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gdpkvgqvm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gxdrdyloh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpmhcyzm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/gcthjkxau.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gztprwgvm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gxczxuhyp.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gqzjcwunl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gqflxpuvk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gpoismidl.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gcyswlyuw.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/geoshdfhd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gpnafslnn.sHtML

[S13] C：宏定义
来源：http://wap.fktsv.cn/Article/details/givifjomc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gstuapady.sHtML

[S14] C：枚举
来源：http://read.share.yfazqb.com/Article/details/gadzivyiw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.sjlbkw.cn/Article/details/gkqurwcpy.sHtML

[S15] C：类型转换
来源：http://read.share.vehdjk.com/Article/details/gjgobapku.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/grxkwvcpv.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gniwtjbil.sHtML


<!-- 参考信息 -->