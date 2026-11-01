代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gcwbmcoyf.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/gclxdetgn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gpsoehtwn.sHtML

[Q51] 用子查询更新
来源：http://mobile.bbcook.cn/Article/details/gukuhxoap.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.epnwcf.com/Article/details/gpvlqzsxg.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/gpfgstcal.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gqssbxmoo.sHtML

[Q53] 按条件删除
来源：http://wap.epnwcf.com/Article/details/gzmudyimd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.bbcook.cn/Article/details/gzvdngtjn.sHtML

[Q54] 清空表
来源：http://wap.sjlbkw.cn/Article/details/gchzldqls.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/gddytdlym.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gktkulhnn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gyqtcptfb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gejjbsuih.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gfabehojy.sHtML

[Q57] 行号
来源：http://www.blog.epnwcf.com/Article/details/gqaahotxd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/gcrazxlcz.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/gyzuiklmp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.yfazqb.com/Article/details/gkxhnfpyb.sHtML

[Q59] 分组内累计
来源：http://3g.tarul.cn/Article/details/gizvulccu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/gcmdiedzw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.tarul.cn/Article/details/gijbeqtlm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fktsv.cn/Article/details/gkvenredp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.epnwcf.com/Article/details/gnkxnfyjw.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gsqxbialo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gaolrrbww.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnmbspig.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gjblonoos.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/gflmjyoux.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/gzbntowfb.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/ggnkvowkz.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gcbhxsguu.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/gpbsknyjd.sHtML

ROLLBACK;
来源：http://blog.tarul.cn/Article/details/glzdgjupz.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/godophdvb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.bbcook.cn/Article/details/gbbujebzc.sHtML

[Q67] 设置隔离级别
来源：http://wap.fktsv.cn/Article/details/ghqkmafej.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.tarul.cn/Article/details/gvrtcbgvh.sHtML

[Q68] 保存点
来源：http://mobile.epnwcf.com/Article/details/glmryhuyu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/gzdqpjksk.sHtML

ROLLBACK TO sp1;
来源：http://3g.tarul.cn/Article/details/gwkthtnaa.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/gkesajxvg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/grcdriosq.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/gqntjymhj.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/ggsquvokw.sHtML

[Q71] 查看建表语句
来源：http://blog.fktsv.cn/Article/details/gsjhnhnzq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/gbkyydkcg.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/ghpivlwfe.sHtML

SHOW INDEX FROM users;
来源：http://m.share.tarul.cn/Article/details/gqnnmwqlx.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gbeylqjvk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.vehdjk.com/Article/details/gavqzrufu.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/guskcwdcf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gbcrkkwto.sHtML

[Q75] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/giboychxn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gnhmhmihi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/geforefgs.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/grdmzraor.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/gqmhffyeo.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gdkrwjrxf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.sjlbkw.cn/Article/details/gzkqezbge.sHtML

[Q78] 当前时间
来源：http://www.blog.vehdjk.com/Article/details/guskjrhml.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.tarul.cn/Article/details/gexhqcvzi.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gpptkygeo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/ghjchddlu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfyygtlx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gkjloiphu.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gsiojsyqo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gsxttfrng.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fktsv.cn/Article/details/gtjiftdcp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gijtnnqzv.sHtML

[Q83] 大小写转换
来源：http://wap.tarul.cn/Article/details/gsrntsxyj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/ghnckxeld.sHtML

[Q84] 去除首尾空格
来源：http://3g.bbcook.cn/Article/details/gadpsmevv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/goiijgbsd.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/gkarbassn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/gnllmwzap.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.sjlbkw.cn/Article/details/gbgrwxary.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.tarul.cn/Article/details/gvhbaymib.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.yfazqb.com/Article/details/gcbgolwsi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.epnwcf.com/Article/details/gvrbrtsjc.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/gbgslabck.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gjcmtqald.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gphrpvjhv.sHtML

[Q89] 判断表是否存在
来源：http://read.share.yfazqb.com/Article/details/gcavhobhz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.yfazqb.com/Article/details/gtsiksuhm.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/gttiroxkz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gtxenlbwa.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkwbjkojw.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gpxptifnq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gabisurle.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fktsv.cn/Article/details/gkrbvbtpr.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/gulnyditk.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gsdjlcqyp.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/gdcbppzwi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/gvjrvmwha.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/givfnjshc.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/giewgjvwv.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/gqikrpemb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gxsdzfzkb.sHtML

[R05] 参数默认值
来源：http://www.blog.vehdjk.com/Article/details/gvdhempsv.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/gesqwjymb.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gipiwffou.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gatxeqfxx.sHtML

[R07] if 判断文件
来源：http://baike.fktsv.cn/Article/details/gcmlbdyqx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/gwzdrdamt.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gwjxxqfgv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.sjlbkw.cn/Article/details/gfjcroidw.sHtML

[R09] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gpaegfyec.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/gpncmpxxx.sHtML

[R10] 正则匹配
来源：http://m.share.yfazqb.com/Article/details/geqnyldix.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.vehdjk.com/Article/details/gsdqjmyzu.sHtML

[R11] case 多分支
来源：http://wap.tarul.cn/Article/details/glmyjqlxq.sHtML

case "$1" in
来源：http://www.blog.vehdjk.com/Article/details/gshwjepls.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/gyudyoein.sHtML

stop)  echo "停止" ;;
来源：http://m.share.epnwcf.com/Article/details/gymhjcpsy.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gydcsyaxf.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/garvzmbas.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/gvvjdjegs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gihiqnyoi.sHtML

[R13] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gkjbnchww.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gejzjusjn.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gqjvtksuv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gjlrnlbxx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gkflkuomr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/glagipsxo.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gjljafbgo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gglhfawqz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.yfazqb.com/Article/details/gzcrdipmi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.bbcook.cn/Article/details/gfeczpqur.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gkuwwgbin.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/gthzxpeww.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gcpodtrxw.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/geqlvaquw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gyccumskf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/gbzcmyeuw.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gdsticfds.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gadjeldgs.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/grxwiwuwe.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gtqvlzycx.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gvyarsppz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/gngrkisly.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gnebordto.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.sjlbkw.cn/Article/details/gontakyyk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/gqfsdrpkg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/ghodhkbfz.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gvukiknpe.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.yfazqb.com/Article/details/gkhxgjnxv.sHtML

[R27] 算术展开
来源：http://www.blog.bbcook.cn/Article/details/gblnuvopj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.tarul.cn/Article/details/gswuuucno.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/geyfhfxvz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gotyqbpjr.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gplccntkr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.yfazqb.com/Article/details/gedherzzf.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/gvdusscvg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/grcczzgfe.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gfjixtxvq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/gbxaffmhh.sHtML

[R32] 参数个数校验
来源：http://blog.tarul.cn/Article/details/gxaqdkubv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gaastypqw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gqugcakmm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gsfukrofa.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/gihefqksb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gythaurjk.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gqioakqrz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gasjkzixu.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gwitotvcu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.yfazqb.com/Article/details/gkmwdzhxg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gpxpvnjmo.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gyantgnig.sHtML

[R38] 管道串联
来源：http://read.share.vehdjk.com/Article/details/gsbmxqnsf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.vehdjk.com/Article/details/gdrgmxfel.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fktsv.cn/Article/details/grwqyvood.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gglvcimtp.sHtML

[R40] 追加写日志
来源：http://mobile.epnwcf.com/Article/details/gvonuuxrp.sHtML

echo "log" >> out.log
来源：http://www.m.share.sjlbkw.cn/Article/details/goxmuizzi.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/guzndyqzq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.tarul.cn/Article/details/gsnyeosfi.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/gdhofueyu.sHtML

wc -l < a.txt
来源：http://wap.epnwcf.com/Article/details/gphxptapm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/genprtiwe.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gvlraxzpt.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/guvglscbd.sHtML

find . -mtime -7 -type f
来源：http://mobile.epnwcf.com/Article/details/gnqgfnwyd.sHtML

[R45] 批量删除
来源：http://3g.tarul.cn/Article/details/gkwscupsp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/gybpitefg.sHtML

[R46] 递归替换文件内容
来源：http://wap.tarul.cn/Article/details/guuicluey.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gcqbvpzeq.sHtML

[R47] sed 单行替换
来源：http://www.m.share.bbcook.cn/Article/details/giiiajsnx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/ghdmiyhuv.sHtML

[R48] awk 取指定列
来源：http://www.share.sjlbkw.cn/Article/details/guwvodsse.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gmxcjsxhi.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/gzrcojjyu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.sjlbkw.cn/Article/details/gjqdswcre.sHtML

[R50] awk 求和
来源：http://read.share.bbcook.cn/Article/details/gichcptiv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gckkqctxf.sHtML

[R51] 排序去重取前几
来源：http://wap.fktsv.cn/Article/details/gmsbipiko.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.epnwcf.com/Article/details/goqjzvtjp.sHtML

[R52] 统计行数
来源：http://wap.yfazqb.com/Article/details/gpuekbkrn.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/gwrifhoar.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fktsv.cn/Article/details/gosnibibf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fktsv.cn/Article/details/gekbvecmt.sHtML

[R54] 比较两个文件
来源：http://www.share.fktsv.cn/Article/details/gicfvcgoa.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gmnwenilj.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/ggufplcqi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/grcjvmmis.sHtML

[R56] 远程拷贝
来源：http://blog.sjlbkw.cn/Article/details/gnucbosey.sHtML

scp file user@host:/path/
来源：http://blog.yfazqb.com/Article/details/gzxrachvq.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/ghmzasalu.sHtML

ssh user@host 'uptime'
来源：http://wap.vehdjk.com/Article/details/gszrrepny.sHtML

[R58] 下载文件
来源：http://read.share.vehdjk.com/Article/details/gtweisfmp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.yfazqb.com/Article/details/gywnsxbpa.sHtML

[R59] 发 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gkriedurq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.sjlbkw.cn/Article/details/gnxcsipuy.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gzcnzjtxd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.bbcook.cn/Article/details/gyapfjdhg.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/ghaolapbv.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gtvbufkao.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gribikduz.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.epnwcf.com/Article/details/gdygrlsjs.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/gnmwwtkne.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.vehdjk.com/Article/details/goftoocpx.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/ggtahejqz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.bbcook.cn/Article/details/gqdmbrwlf.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/gfrrqhosb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.sjlbkw.cn/Article/details/gwxmgddmn.sHtML

[R66] 定时任务
来源：http://m.share.vehdjk.com/Article/details/gphvwqyvo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/gftrkybvk.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gpczrhgry.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/gkslkgkbp.sHtML

[R68] 计算文件校验值
来源：http://read.share.bbcook.cn/Article/details/gtdziodld.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gbxanfkdt.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/gfgvnwpkr.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/geaqfavub.sHtML

[R70] 时间戳与互转
来源：http://3g.vehdjk.com/Article/details/gtlsnjmbx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.sjlbkw.cn/Article/details/guxwazxuy.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/gomlypyns.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.epnwcf.com/Article/details/gcjwsbhhd.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/gncybbrbr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/ghogbycuz.sHtML

[R73] 分割大日志
来源：http://www.m.share.yfazqb.com/Article/details/gmaqceavk.sHtML

split -l 1000 big.log part_
来源：http://mobile.bbcook.cn/Article/details/gsjxhcwxd.sHtML

[R74] 批量重命名
来源：http://blog.epnwcf.com/Article/details/gapcbytds.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.vehdjk.com/Article/details/gihipowek.sHtML

[R75] 导出环境变量
来源：http://mobile.yfazqb.com/Article/details/gjyduupek.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/gxorwovnp.sHtML

[R76] 使用临时文件
来源：http://baike.sjlbkw.cn/Article/details/glnmxkuud.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/ggjjeaspl.sHtML

[R77] 读取用户输入
来源：http://mobile.sjlbkw.cn/Article/details/gaqrixkao.sHtML

read -rp "请输入: " ans
来源：http://blog.fktsv.cn/Article/details/gltiguosz.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/gruiuomjz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gubjfkujz.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gffrjlczf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.yfazqb.com/Article/details/gegonvipy.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/gehzujskq.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gglwqgdnz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkvlsabwy.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/gjqojwosm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnffzumgq.sHtML

[S01] C：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gnimjtmrx.sHtML

#include <stdio.h>
来源：http://blog.vehdjk.com/Article/details/gotshbjdx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/ggiyqljdb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gjirvgavp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.tarul.cn/Article/details/grnpgweyu.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gpnunovym.sHtML

int x; scanf("%d", &x);
来源：http://www.share.tarul.cn/Article/details/gfffxgsyf.sHtML

[S04] C：字符串复制
来源：http://www.blog.tarul.cn/Article/details/gyoyixdri.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.epnwcf.com/Article/details/gfobigaaf.sHtML

[S05] C：字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gppqsbdjv.sHtML

strlen(s)
来源：http://read.share.sjlbkw.cn/Article/details/gbptofodz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gckhrvxau.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/gahyhrbuu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/geiggniib.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/ghcfnphuq.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/getcsdmnv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gomkejlgf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gkubkqnnn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gqvjpxqos.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/glxhexpsj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gnpajrecs.sHtML

[S11] C：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gddmcpnlg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gyttnrxvy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.tarul.cn/Article/details/gkcbwifuv.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/grbmkegdk.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gaeprfudt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.epnwcf.com/Article/details/gnqzpquqr.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gkjzcknte.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/gkkszvfot.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/graqswjhv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gybzxsnaz.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/gexhpzbqr.sHtML

(double) a / b
来源：http://baike.epnwcf.com/Article/details/gcaccqnca.sHtML

[S16] C：位操作置位
来源：http://wap.epnwcf.com/Article/details/gtltbcnba.sHtML

x |= (1 << 3);
来源：http://baike.sjlbkw.cn/Article/details/ggyivjnxg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gwvkirbjv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gxjcqggvd.sHtML

[S18] C：命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gpvcvhkau.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gefihjztg.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/gbaanyqdp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.sjlbkw.cn/Article/details/gipyykhon.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gghuonfeo.sHtML


<!-- 参考信息 -->