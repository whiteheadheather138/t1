代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gsnedqzln.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/gclfspeeg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gcolgkvaz.sHtML

[Q51] 用子查询更新
来源：http://blog.sjlbkw.cn/Article/details/gvvxvlqzb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/ghkltcxxn.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/gawinlobp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gguflorjh.sHtML

[Q53] 按条件删除
来源：http://m.share.yfazqb.com/Article/details/gdybjfewn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gbthnutnh.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/glbnmhrmx.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gfamcytoh.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gbxiifmqt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/gheffzyde.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.yfazqb.com/Article/details/geepglcnn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/gchqycngp.sHtML

[Q57] 行号
来源：http://www.blog.epnwcf.com/Article/details/gutbsvjvj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/gaxnxbsyw.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/gkzbfkehk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/gdopfzpnj.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gzesufedf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gfpbbuufz.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.sjlbkw.cn/Article/details/gwaqkodiw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.tarul.cn/Article/details/gtkmtoqcq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gmsaahxbf.sHtML

[Q61] 移动平均
来源：http://read.share.fktsv.cn/Article/details/gqxpzzncx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/guivmdcpt.sHtML

[Q62] 分组占比
来源：http://www.share.sjlbkw.cn/Article/details/gyqrkgruz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gfvjlcsxt.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/gonbjewqw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gnijrbzvn.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/gmdvfsyyj.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gekuckbzz.sHtML

[Q65] 回滚事务
来源：http://mobile.yfazqb.com/Article/details/gcqbxtfca.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/gtvfnnixz.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/gerswawgg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/ghncyqtyw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.epnwcf.com/Article/details/gztyaeudr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gsulxmqid.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gllgrpexe.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gflelfapp.sHtML

ROLLBACK TO sp1;
来源：http://3g.bbcook.cn/Article/details/gmvwjdhyr.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/goirlaivi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.yfazqb.com/Article/details/gvjxzfjyk.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gkcwlwsif.sHtML

ANALYZE TABLE users;
来源：http://baike.vehdjk.com/Article/details/gbfiiloek.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/goremdfzx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gbqucgsau.sHtML

[Q72] 查看索引
来源：http://www.share.epnwcf.com/Article/details/gahqpniql.sHtML

SHOW INDEX FROM users;
来源：http://wap.vehdjk.com/Article/details/gyzxptsyk.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/glljlnhge.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gzimztscw.sHtML

[Q74] 强制使用索引
来源：http://blog.tarul.cn/Article/details/gjnifihjc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gomqkzvmj.sHtML

[Q75] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/ggfwfoesm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/ghshqunql.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gmeolcwvc.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gzunfbkvo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/genefvwou.sHtML

[Q77] 时间加减
来源：http://www.share.fktsv.cn/Article/details/gvqpbdjyr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.bbcook.cn/Article/details/gfxaaptgf.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/ggzvjrmlb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/gehycrjqq.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gopsjcilq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gcltzzrpv.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/ghxmubsyt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gjhxsowrs.sHtML

[Q81] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gzajrizxs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gdndpfzbp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/ghokfhcym.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gcfrohqnz.sHtML

[Q83] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gdxgpvxbx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gncaqldeu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gfqhjdnhu.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gbkyitckr.sHtML

[Q85] 数值取整
来源：http://wap.yfazqb.com/Article/details/gevclqwaq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/gxzarwvcg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fktsv.cn/Article/details/gtnornzyr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/gnutteniw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/gepfxmikj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.sjlbkw.cn/Article/details/gahzqcefo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gcowrxzzg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/gdfergshx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.yfazqb.com/Article/details/gfuxrtxlm.sHtML

[Q89] 判断表是否存在
来源：http://wap.epnwcf.com/Article/details/gwnhunpiw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gexhhogta.sHtML

[Q90] 生成序号列
来源：http://www.blog.sjlbkw.cn/Article/details/gmqvfskku.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fktsv.cn/Article/details/gbnylbwft.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvhptygtl.sHtML

R. Bash 专题
来源：http://wap.yfazqb.com/Article/details/gqegoyuhw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gawjrokiv.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.bbcook.cn/Article/details/grwbmgzcv.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gfuioghiu.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/gzbnyfjqb.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/glwdeflak.sHtML

name="Tom"; echo "$name"
来源：http://www.share.bbcook.cn/Article/details/gdtjfduho.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/glydsmwkl.sHtML

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/ghmycdbzp.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/gapmprfmg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.bbcook.cn/Article/details/gtnylmikd.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/guzuvmptq.sHtML

name="${1:-default}"
来源：http://www.blog.vehdjk.com/Article/details/gsfhieisq.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/gnggfubzc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gghovjrkg.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gbunezpnf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/guybpsilv.sHtML

[R08] 数值比较
来源：http://www.blog.bbcook.cn/Article/details/gaetfxbfj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/gvddblhqq.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gbiarwgxg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/grxwqqpid.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/grpuiyhmc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.tarul.cn/Article/details/gjyqnbvks.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/ghtgywpvf.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gpeaayypv.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gedilpekv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.tarul.cn/Article/details/gbjszbcqi.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gulwqpmrk.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gtmuqhvcm.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gpdlcmxcy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.bbcook.cn/Article/details/gusttyegy.sHtML

[R13] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gxaxzncst.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/geewddacg.sHtML

[R14] C 风格 for
来源：http://www.share.fktsv.cn/Article/details/gzldqmbod.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/ggwbfeqgp.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gzlescwip.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/gxhdagdkl.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gowiqbmfh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gycukxzsn.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/goyrpzspc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gsraukuxm.sHtML

[R18] 遍历数组
来源：http://baike.bbcook.cn/Article/details/gioqocnjz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.epnwcf.com/Article/details/gupfswrap.sHtML

[R19] 数组长度
来源：http://www.share.tarul.cn/Article/details/gbtefqvtd.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gipoqkeue.sHtML

[R20] 关联数组（字典）
来源：http://www.share.yfazqb.com/Article/details/gnohfakls.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.vehdjk.com/Article/details/gczcxneey.sHtML

[R21] 字符串长度
来源：http://blog.fktsv.cn/Article/details/gmkpjftgj.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gyzqqytxv.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gibfeghub.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/gelyrgfiu.sHtML

[R23] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/glcidsxxl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gcnvvewma.sHtML

[R24] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gssddqzso.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.yfazqb.com/Article/details/gpzvoeeii.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.yfazqb.com/Article/details/glwzyaqux.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.sjlbkw.cn/Article/details/ghwjbmsgs.sHtML

[R26] 命令替换
来源：http://www.blog.tarul.cn/Article/details/gdudxcxji.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/gtsslhlmf.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gwlonsfdc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/ggpvkkalg.sHtML

[R28] 浮点运算
来源：http://www.m.share.tarul.cn/Article/details/gioqvzqgp.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gjzmenitb.sHtML

[R29] 定义函数
来源：http://mobile.bbcook.cn/Article/details/giwmwyduz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.yfazqb.com/Article/details/gsieyhcxn.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gjqxvhqwk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/gvkdysgjt.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/gnpyaakxo.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gusiuihyw.sHtML

[R32] 参数个数校验
来源：http://3g.tarul.cn/Article/details/ghinopmcz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gacsbktek.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gictfltru.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gqtbwurzs.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gasqvohef.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gzgbvsomj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gqnkbkfdr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/grttfvxxp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.tarul.cn/Article/details/gbrrzcbxs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/gmzcwzrda.sHtML

[R37] 把输出赋给变量
来源：http://baike.vehdjk.com/Article/details/gchebfsay.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/gcncfbptd.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/gzviexqoo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gvqssjqej.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/ggvzlynwn.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/grmbjvvge.sHtML

[R40] 追加写日志
来源：http://3g.vehdjk.com/Article/details/gmybcyimd.sHtML

echo "log" >> out.log
来源：http://blog.sjlbkw.cn/Article/details/gecokqnuv.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/gppmppxgy.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gbmccugrw.sHtML

[R42] 输入重定向
来源：http://m.share.fktsv.cn/Article/details/gqpqcamfz.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/gfblbvaxo.sHtML

[R43] 按名字查找文件
来源：http://read.share.tarul.cn/Article/details/glrlilmkr.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gfkznjwra.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/giaiecsqq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gobbmnkyk.sHtML

[R45] 批量删除
来源：http://3g.sjlbkw.cn/Article/details/gfkeqipak.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/goahqujtu.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/gdjlusztz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gnaiggeox.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gkunqaxzj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.bbcook.cn/Article/details/glemqcsnu.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gywedxnln.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gqdtjvwff.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/gxtefgbhv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gambyqbhg.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gimglkdvg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gmnohctyp.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fktsv.cn/Article/details/gjbmbbfjx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.bbcook.cn/Article/details/goyedddra.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/gmvcsvksl.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/gjlotvars.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/gslfgzlkt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/gsfommohf.sHtML

[R54] 比较两个文件
来源：http://m.share.yfazqb.com/Article/details/gfnislmem.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gnogonzni.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/grljwykuy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.sjlbkw.cn/Article/details/gqsoapkcc.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gyfxeboof.sHtML

scp file user@host:/path/
来源：http://mobile.epnwcf.com/Article/details/gdteyvcet.sHtML

[R57] 远程执行命令
来源：http://www.m.share.yfazqb.com/Article/details/gscqqvfhg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gwzpfxrjm.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/gknsezvnh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/gfcklbeua.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/gowqwmlyt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gygyoqvwc.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gryuhikni.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.vehdjk.com/Article/details/gynkhmlif.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gtnunzkvy.sHtML

df -h;  du -sh *
来源：http://mobile.bbcook.cn/Article/details/gmodggojf.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gsrhgdxwn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gfgqskfks.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gegwiipml.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fktsv.cn/Article/details/gdcetdcgw.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/guqwzfhxk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gkkywduag.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/glyfamgqs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.bbcook.cn/Article/details/ghprpaeyn.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gxtbdmexw.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/gpmemtjrk.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/goxyhfrwe.sHtML

openssl rand -hex 16
来源：http://www.blog.sjlbkw.cn/Article/details/gfosuschc.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gdfhovfsb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gekhozulx.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/gfvfkphhn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/gnxqvrrfy.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/grmhbzxqc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.bbcook.cn/Article/details/gljcdoyxm.sHtML

[R71] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gwescfawl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/ggszaiymf.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/gibgulvpp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gkchwpdks.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/gmxyklgvl.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/gbgkqdhiq.sHtML

[R74] 批量重命名
来源：http://mobile.yfazqb.com/Article/details/grqqogunq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gsrwifouu.sHtML

[R75] 导出环境变量
来源：http://read.share.fktsv.cn/Article/details/gnoxnlstf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.yfazqb.com/Article/details/ggqikbstw.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/grlqtflnx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gmiomqgos.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gcyiqgjsl.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gfbqwmdwo.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gvgqxmics.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.sjlbkw.cn/Article/details/gikhmhlyv.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gvrsjzsoo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/gvqxceslw.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.yfazqb.com/Article/details/gmwojbgps.sHtML

time ./run.sh
来源：http://mobile.fktsv.cn/Article/details/gmrnoravs.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbnntflya.sHtML

S. C / C++ 专题
来源：http://baike.epnwcf.com/Article/details/gpmbduftk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glmgmvazv.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/goerbtkvr.sHtML

#include <stdio.h>
来源：http://read.share.fktsv.cn/Article/details/gismhmbxd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gqvauxbjl.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/glnaltwjq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.vehdjk.com/Article/details/gkbiwccsl.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/grafqmzft.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/gsnvlqvql.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/gxecwxrgn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.tarul.cn/Article/details/gajtdifzb.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/glthljhwt.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gpxinhysa.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gfjdzbtog.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/gsedyzzhn.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gnbvrurzd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/gftjyrhvh.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/gbefnkbyo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/gbhhtramd.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gdocqgddj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gkybvnvdg.sHtML

[S10] C：指针与解引用
来源：http://www.blog.bbcook.cn/Article/details/godpxhyxk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gkiiozctk.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gxivtsbyx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gzhttrxhs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fktsv.cn/Article/details/gooceptun.sHtML

fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gvfxujbbg.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/guxthrukb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gkbqbtuol.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/grxukslxn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fktsv.cn/Article/details/gaqlikuon.sHtML

[S14] C：枚举
来源：http://baike.yfazqb.com/Article/details/ggpkzobgu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.epnwcf.com/Article/details/gfbgkevpq.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gzlyyrauu.sHtML

(double) a / b
来源：http://www.share.bbcook.cn/Article/details/gozubbsec.sHtML

[S16] C：位操作置位
来源：http://www.blog.tarul.cn/Article/details/gkegiwvkc.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gqpgbwwpo.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gjbecaonw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/gctdcbtxw.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmhkbcde.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.tarul.cn/Article/details/gewyhcbtx.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/gfdbtohia.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/ghapzdvjx.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/gxuicilrl.sHtML


<!-- 参考信息 -->