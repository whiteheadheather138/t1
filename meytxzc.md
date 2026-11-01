代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/gjgsztbzj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.sjlbkw.cn/Article/details/gxttcpgyg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/gxzwdwaem.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gjfnpyhpx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.tarul.cn/Article/details/glsshvuwb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.bbcook.cn/Article/details/gbxygyraq.sHtML

[Q43] 标量子查询
来源：http://3g.yfazqb.com/Article/details/gszsgrbom.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/giibzrsqa.sHtML

[Q44] IN 子查询
来源：http://3g.vehdjk.com/Article/details/ganvbmbzd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.vehdjk.com/Article/details/gemtmshhf.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fktsv.cn/Article/details/gnxjutxvu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gkbaviset.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.bbcook.cn/Article/details/gsmmjnqno.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gzxrjdqde.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/gfajsxjlh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gveokqywe.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gekmnhybo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gfnagvvqb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.sjlbkw.cn/Article/details/gtjkcsdfg.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/gaslngffr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gbacghqyp.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gssgsqpwv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gcejwoije.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gxecmggor.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fktsv.cn/Article/details/gqizlkdwm.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gileycryh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gobkysuag.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gaubsjpvv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fktsv.cn/Article/details/gqpyzvwgk.sHtML

[Q54] 清空表
来源：http://www.blog.fktsv.cn/Article/details/gcyiibauo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.yfazqb.com/Article/details/gxaqcfuhr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.vehdjk.com/Article/details/gfztqurbv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/grgmyjarv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fktsv.cn/Article/details/gpsslfnge.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fktsv.cn/Article/details/gdxjwxxae.sHtML

[Q57] 行号
来源：http://www.blog.sjlbkw.cn/Article/details/giytlaaxk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gdscvulpp.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/grvfbegkg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gkjrvwtje.sHtML

[Q59] 分组内累计
来源：http://wap.epnwcf.com/Article/details/gmicgcqmy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/ghppttuzv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/gvoyurkhl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.bbcook.cn/Article/details/gyayyohkw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.yfazqb.com/Article/details/ggowybecu.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gbspbjbfv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gjksfroqr.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gwoehzusa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gbdzjddmi.sHtML

[Q63] 开启事务
来源：http://www.share.vehdjk.com/Article/details/gdupniddc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/glbnxfmdm.sHtML

[Q64] 提交事务
来源：http://3g.bbcook.cn/Article/details/gmroyehnc.sHtML

COMMIT;
来源：http://www.blog.epnwcf.com/Article/details/ginxqhodp.sHtML

[Q65] 回滚事务
来源：http://3g.vehdjk.com/Article/details/gzhrhsgoo.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/glkynijim.sHtML

[Q66] 行锁查询
来源：http://baike.fktsv.cn/Article/details/glowedwjt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.vehdjk.com/Article/details/gusqyfyfl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/ghwjebbbu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.yfazqb.com/Article/details/glqfowder.sHtML

[Q68] 保存点
来源：http://blog.tarul.cn/Article/details/gmclatbtu.sHtML

SAVEPOINT sp1;
来源：http://wap.bbcook.cn/Article/details/ggwmguemy.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gwttktmvh.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/ghoaupjkc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.bbcook.cn/Article/details/guqayscxp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/garwbybjh.sHtML

ANALYZE TABLE users;
来源：http://mobile.fktsv.cn/Article/details/guiddtkkp.sHtML

[Q71] 查看建表语句
来源：http://m.share.epnwcf.com/Article/details/ghtrhrhca.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gazuyrute.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gieozdbbl.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gxrtjbxeh.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/ghyzkkdfm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/gebryqrir.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gdfpqmhrj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/gxknejuhp.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gnilyeoqi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gnpuovfzc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.bbcook.cn/Article/details/gzzuyknkb.sHtML

[Q76] 按天统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoisntqk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.vehdjk.com/Article/details/gloltcsux.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/gnwplakxd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fktsv.cn/Article/details/gxkoyijta.sHtML

[Q78] 当前时间
来源：http://read.share.fktsv.cn/Article/details/gtkjvgnua.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gkuzlhcfw.sHtML

[Q79] 字符串拼接
来源：http://read.share.fktsv.cn/Article/details/ggbwqhqwh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gxlzpxfhs.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gpxfyitbf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gxvlzofdr.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gcasvctqg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gbfntyzqm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.bbcook.cn/Article/details/gezgqgzvu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gundcsrib.sHtML

[Q83] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gidtuwdjm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gkvdlnscu.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/gkyipmhii.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gnamzdflb.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gupiusiot.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/gncgzmqjd.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fktsv.cn/Article/details/gzmziycpa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.sjlbkw.cn/Article/details/ggdwdkjev.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gsnpscrxe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/gjvzudlpa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gznamczya.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/gudlcgize.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/gaadopykn.sHtML

[Q89] 判断表是否存在
来源：http://3g.yfazqb.com/Article/details/gnmxayhch.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.epnwcf.com/Article/details/gwvcgirwv.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gzpyjsjmj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/glwhrqsjr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gqnlehdte.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gqcbljvmz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxwdkzjun.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gwwjnvpnq.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/gqkokezoa.sHtML

set -euo pipefail
来源：http://www.blog.epnwcf.com/Article/details/gbivggjss.sHtML

[R02] 变量赋值与使用
来源：http://m.share.vehdjk.com/Article/details/gspkrkhje.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gucnjzshs.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/getudlakl.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gtwibcbgo.sHtML

[R04] 位置参数
来源：http://wap.yfazqb.com/Article/details/glnpkucuj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/gimxnyqdh.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gtmzdozjv.sHtML

name="${1:-default}"
来源：http://www.blog.epnwcf.com/Article/details/gwgidvdhl.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/gudyhlocf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gzdfbupye.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gyjjmmyut.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/goaapgthj.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/gdgnocnab.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gobkeywmh.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gnhwqkppi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gjtwsczeo.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/graxueaii.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/gzoatejgq.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/ghuvvsbnm.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gbamrymxv.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/glangqmvh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fktsv.cn/Article/details/ghykkuzcs.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gvxqwvscn.sHtML

esac
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvzjugzs.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fktsv.cn/Article/details/gynzwrxez.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.vehdjk.com/Article/details/gjhjjmyrt.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gocirhtuo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gzwzboyzh.sHtML

[R14] C 风格 for
来源：http://3g.fktsv.cn/Article/details/gcdwblzlm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gyfpvefwm.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gggazhmvf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/gjytmuzwf.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gelkbbvjm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gtwzpjaup.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gbeblthdx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gwzsasmwm.sHtML

[R18] 遍历数组
来源：http://www.share.sjlbkw.cn/Article/details/gwrtdykzt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/ggtkmhtvk.sHtML

[R19] 数组长度
来源：http://blog.vehdjk.com/Article/details/gazjdzton.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.epnwcf.com/Article/details/gzezzvukd.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/grwbvbdek.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.bbcook.cn/Article/details/glwdtierq.sHtML

[R21] 字符串长度
来源：http://blog.fktsv.cn/Article/details/gamaokngx.sHtML

echo "${#s}"
来源：http://3g.bbcook.cn/Article/details/gwdixhyfq.sHtML

[R22] 截取子串
来源：http://blog.yfazqb.com/Article/details/ghgbtnzzs.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/glfohbubx.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gthhvtfna.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gtdpwvsmq.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/grxycgzgh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fktsv.cn/Article/details/gaawhnemm.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/gzwlqsenp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gwupfcbxg.sHtML

[R26] 命令替换
来源：http://www.m.share.sjlbkw.cn/Article/details/glkhnupic.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/gorzvzitx.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gqhqngtme.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/ginvmtoga.sHtML

[R28] 浮点运算
来源：http://read.share.tarul.cn/Article/details/gophmhviz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gszvgunex.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gyctrslbv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gfebxmgbv.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/ggzgmkpix.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gchyzzjao.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/gpalsrmxd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/ggbxlevdo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/gclqclxtm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gnyavytfc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gebsvidbz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/gijxurgbt.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/gfxneragh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gupfinwzj.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/ghjywjfea.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/ghttofduv.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/glceyzaep.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/gumshfyty.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.vehdjk.com/Article/details/glgazinip.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gqnsajtdw.sHtML

[R38] 管道串联
来源：http://read.share.fktsv.cn/Article/details/gbklvtpcu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gykccpujl.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gezxsbwol.sHtML

cmd > out.log 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gpddohgdd.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/geclncsez.sHtML

echo "log" >> out.log
来源：http://mobile.yfazqb.com/Article/details/gryylolrw.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gwpkvrfim.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/gttfisqdj.sHtML

[R42] 输入重定向
来源：http://read.share.bbcook.cn/Article/details/gnkxgznet.sHtML

wc -l < a.txt
来源：http://wap.fktsv.cn/Article/details/gwxckdnxx.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/gbjqpwcbz.sHtML

find . -name "*.log" -type f
来源：http://blog.fktsv.cn/Article/details/gwletkesf.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/gomysjpio.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gppdasmrt.sHtML

[R45] 批量删除
来源：http://3g.yfazqb.com/Article/details/gabjuchdy.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.vehdjk.com/Article/details/gvjgzziss.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gbfwxbvlv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.tarul.cn/Article/details/gufhszktj.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gbstspkmf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.bbcook.cn/Article/details/glcxkehhr.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gxzqoquul.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/grqnupgvf.sHtML

[R49] awk 带条件
来源：http://mobile.tarul.cn/Article/details/grnqueoux.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fktsv.cn/Article/details/gxnbhhogf.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gjemaplnq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gidkbovwt.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/gstybffoi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gfkhbuszu.sHtML

[R52] 统计行数
来源：http://3g.sjlbkw.cn/Article/details/gapwaxmwt.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gvfeeuhru.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/glpphlpjz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.vehdjk.com/Article/details/gqdtfcuzx.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gouhstpiv.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gmuoscwwq.sHtML

[R55] 压缩与解压
来源：http://www.share.tarul.cn/Article/details/gkztuxuea.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.epnwcf.com/Article/details/gtsyywfcv.sHtML

[R56] 远程拷贝
来源：http://www.share.tarul.cn/Article/details/glueyxmxf.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/gjrpfqmdo.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/grlderufq.sHtML

ssh user@host 'uptime'
来源：http://read.share.fktsv.cn/Article/details/gyveygfyw.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/gzymdetkr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.vehdjk.com/Article/details/glhjjyike.sHtML

[R59] 发 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gkkgnnzih.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gvnaonloa.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/gqsihfash.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/gccnokvoo.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/gdrginyjb.sHtML

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/gnepxxqlc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.epnwcf.com/Article/details/gxxqdkida.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fktsv.cn/Article/details/gigptofqu.sHtML

[R63] 内存与进程
来源：http://www.blog.fktsv.cn/Article/details/gosfjanbe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.epnwcf.com/Article/details/gchsvkyvz.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/glmglumtj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/gfoyvogrv.sHtML

[R65] 查看端口占用
来源：http://wap.fktsv.cn/Article/details/gtrxsoafp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.yfazqb.com/Article/details/gzrkglarw.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/glgbohqpm.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/gufluzxyt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gzronrmme.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gdcnnlmqa.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gfxxsltxg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/gcabrttrf.sHtML

[R69] 生成随机密码
来源：http://wap.yfazqb.com/Article/details/gdnzvgewq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.sjlbkw.cn/Article/details/gdmttktnn.sHtML

[R70] 时间戳与互转
来源：http://wap.yfazqb.com/Article/details/gilfplcjo.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.tarul.cn/Article/details/gctlfracy.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/ggjxuneho.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gjzgcpyva.sHtML

[R72] 等待端口就绪
来源：http://www.share.epnwcf.com/Article/details/gbxbzqnlj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gfrdharxw.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/gdmauaboq.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gzwrwbtve.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/gdjsxkxdy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gycgrfbgl.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gbdpfeypo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.bbcook.cn/Article/details/gkrgvzqmr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.tarul.cn/Article/details/grsyxagqm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gqvtvqvrn.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gywdljiso.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/gcfavekpj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.vehdjk.com/Article/details/gwvyoklym.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.epnwcf.com/Article/details/glgajwdan.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/gqzrgwsjf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.yfazqb.com/Article/details/gxzrmyqds.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/ggxxbxqtl.sHtML

time ./run.sh
来源：http://read.share.fktsv.cn/Article/details/gumunziiw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grqwpbpwv.sHtML

S. C / C++ 专题
来源：http://baike.bbcook.cn/Article/details/gbgwrylki.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkxvhnnvd.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/govkajvrd.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gvdueqyei.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.vehdjk.com/Article/details/gkzgqefef.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.epnwcf.com/Article/details/gsdoisoqc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.yfazqb.com/Article/details/gioqipauo.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gfxsqxbfw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fktsv.cn/Article/details/ghzqdwlok.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/ghsovcemh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/gvqjqwxxh.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/gwvxhrhkb.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gwzdghcge.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/giftrmyag.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gwnzulkqt.sHtML

[S07] C：数组遍历求和
来源：http://blog.sjlbkw.cn/Article/details/gjynovgod.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gwmcbwaml.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/glmlmnmba.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/ghldummvf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gxzeigbeu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gfvoxeljf.sHtML

[S10] C：指针与解引用
来源：http://m.share.yfazqb.com/Article/details/gklinfita.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/gmjkjwnhy.sHtML

[S11] C：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gbbbbqosb.sHtML


<!-- 参考信息 -->