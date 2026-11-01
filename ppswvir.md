代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gisliubyh.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/ggsegjiry.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gzqkozchg.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/ggxdrzujk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.tarul.cn/Article/details/gvesfnvln.sHtML

[Q24] 去重
来源：http://m.share.fktsv.cn/Article/details/ggzlobzlp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gysqeydig.sHtML

[Q25] 只取前 N 条
来源：http://www.share.tarul.cn/Article/details/gqwhhrrhy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gkykqhfxe.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/gudgmguxo.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gzzoztmbh.sHtML

[Q27] 条件计数
来源：http://read.share.epnwcf.com/Article/details/gzemhldec.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fktsv.cn/Article/details/gyjpglytc.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gwxcksejo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gtaktnkcc.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/glppechbw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gdxscmyue.sHtML

[Q30] 分组统计
来源：http://mobile.epnwcf.com/Article/details/gwbxzrwvu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gxbhosgxl.sHtML

[Q31] 分组后过滤
来源：http://baike.sjlbkw.cn/Article/details/gwwsbcepu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/gwlvxeblb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gaggndjdj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gwysicmwc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/grmbigwnx.sHtML

[Q33] 多列分组
来源：http://www.share.tarul.cn/Article/details/gqhodthts.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/gqdiojxle.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/gfrrwggmj.sHtML

SELECT * FROM (
来源：http://mobile.epnwcf.com/Article/details/gbervatdg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/gcnvhpihy.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/girrzcayd.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gtlkxwjsy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gijunwlcx.sHtML

[Q36] 左连接
来源：http://www.m.share.bbcook.cn/Article/details/gabrizeyf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/grjbepmxv.sHtML

[Q37] 右连接
来源：http://www.share.tarul.cn/Article/details/gqxncmlpf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.bbcook.cn/Article/details/gbnyyeufe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gtxnwfpcp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/gdleryeyi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gemlgliaz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/gobsggrnv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gmlixstjz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gvpxtvzct.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gdvsjnbkv.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/gktllqwdn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.epnwcf.com/Article/details/gblbpkxpx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.epnwcf.com/Article/details/gtrwyxtci.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/gsmdzkwfv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/glpgwscrs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gsrqjoxeq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.tarul.cn/Article/details/gyljkypdg.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/gibrsftxy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.vehdjk.com/Article/details/gykksbyed.sHtML

[Q44] IN 子查询
来源：http://m.share.epnwcf.com/Article/details/gxejazxhz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/ghfmmdyln.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.epnwcf.com/Article/details/ggxnfqmvg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/glcyfiade.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.tarul.cn/Article/details/gliomcccq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/grmbuveqa.sHtML

[Q47] 与平均值比较
来源：http://mobile.bbcook.cn/Article/details/ggscdnvry.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gdjiwfalu.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/glvbipvbo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.tarul.cn/Article/details/geaqtzhjq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/grxauotax.sHtML

[Q49] 更新单行
来源：http://blog.fktsv.cn/Article/details/grrjbxops.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gtksnhdot.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/gesnpnmwe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gpjmacbjd.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/gjhquycxr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.yfazqb.com/Article/details/gdcqmbdjv.sHtML

[Q52] 删除指定行
来源：http://www.m.share.yfazqb.com/Article/details/gzrzeduzb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gekittuqb.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/glmzhhpln.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gxvpehqrj.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/glwzpnvxm.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.epnwcf.com/Article/details/gpmiqtfpv.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/gmpvjhdon.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gzxzldfqj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.yfazqb.com/Article/details/gnozjhqjg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gfzapzicn.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/gyazpppxq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gguegoyzr.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gdhmluhen.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gvlapsqlg.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/guovcmoga.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gwvvyvyax.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/grhppnwdb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.yfazqb.com/Article/details/gbqdhikat.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gsyoqkohx.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/gqwgvagyc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/gzdpcupie.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/gjptmhowz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gezmqyqta.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gdwirhihn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gsksueatj.sHtML

[Q64] 提交事务
来源：http://blog.bbcook.cn/Article/details/gwbangtix.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/galbrxplq.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gsqhcbbrb.sHtML

ROLLBACK;
来源：http://blog.tarul.cn/Article/details/gckhiuarc.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/gfalgmqzy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.tarul.cn/Article/details/gpewkyicy.sHtML

[Q67] 设置隔离级别
来源：http://wap.tarul.cn/Article/details/gurvcvtrh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/gnxzlafnu.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/ghkeomdsj.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gjxlbfdqt.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gajonxqli.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/grglmxrkp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.vehdjk.com/Article/details/gjgdaxdck.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gatqllyro.sHtML

ANALYZE TABLE users;
来源：http://m.share.sjlbkw.cn/Article/details/gyvhjvnut.sHtML

[Q71] 查看建表语句
来源：http://blog.fktsv.cn/Article/details/gouafozed.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/grgghphza.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/grzqaprzn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.bbcook.cn/Article/details/gcobbcekn.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gfixvfuri.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gvexpmfsp.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/glhgwcmkk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/geilgvufw.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gutxxbckx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gvofeqsrl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fktsv.cn/Article/details/gpxodfkdy.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gfchlkatv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gcuujsrqi.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/gufwizwia.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/gyitcovvk.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/gctfijysp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.bbcook.cn/Article/details/gcaqvaypw.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/gxgbdqjnz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.vehdjk.com/Article/details/geivawwpd.sHtML

[Q80] 字符串截取
来源：http://baike.vehdjk.com/Article/details/gktsoecsl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gaitvtlbg.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gkspegrpc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gzbtvkbem.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.bbcook.cn/Article/details/gstgdlgep.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gqcwfxili.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gnhormoqs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gvmlflhzc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/gcvhhptlm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gdjhhntzu.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gkqlntjet.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gdwxvkgcf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/gdcsomvai.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gefooqafy.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/gjaujqvhf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.yfazqb.com/Article/details/giwopbbot.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.vehdjk.com/Article/details/gpbvdvmgz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/glxqbgirf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.bbcook.cn/Article/details/gflfkufas.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fktsv.cn/Article/details/ghipdsxgp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gxhrlvcfc.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gqjxqweba.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.yfazqb.com/Article/details/gypaizuiy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpcymcttc.sHtML

R. Bash 专题
来源：http://www.m.share.yfazqb.com/Article/details/gouqejtyc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gicpbhuyw.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gfgyzqtkm.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/ghspyiipo.sHtML

set -euo pipefail
来源：http://www.share.bbcook.cn/Article/details/geysyuhaq.sHtML

[R02] 变量赋值与使用
来源：http://m.share.vehdjk.com/Article/details/guxigqian.sHtML

name="Tom"; echo "$name"
来源：http://read.share.vehdjk.com/Article/details/gnpjxuvyi.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/gnihhvlkx.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gpvqnjxmd.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/ghyhlfmvq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/gvtboursf.sHtML

[R05] 参数默认值
来源：http://mobile.epnwcf.com/Article/details/gnyubwybj.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gtdywnjdv.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gdbcofoos.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/ghqjvxqgg.sHtML

[R07] if 判断文件
来源：http://wap.epnwcf.com/Article/details/guwqtnrko.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.vehdjk.com/Article/details/ghbfrevdg.sHtML

[R08] 数值比较
来源：http://blog.sjlbkw.cn/Article/details/gggyqvcbb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gcudizjxs.sHtML

[R09] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/goauforrv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gcacvuwzn.sHtML

[R10] 正则匹配
来源：http://www.m.share.fktsv.cn/Article/details/gxmskotlw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/gktuiziue.sHtML

[R11] case 多分支
来源：http://www.m.share.tarul.cn/Article/details/goacwypel.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/gkmweonnw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gqkofybqp.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/ghbpdsstc.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/grsrdayuh.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/geecdibzb.sHtML

[R12] for 遍历文件
来源：http://read.share.fktsv.cn/Article/details/gxqunhzmr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.tarul.cn/Article/details/gkmghzibs.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gfzhctoab.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gjmkqvewe.sHtML

[R14] C 风格 for
来源：http://baike.sjlbkw.cn/Article/details/geisvjanj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/grnylgvco.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gltsbller.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/gphdcqoez.sHtML

[R16] until 等待条件
来源：http://www.blog.fktsv.cn/Article/details/gbcujubuk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gokthnamj.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/glqoykpxv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.bbcook.cn/Article/details/gulbqsknh.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gegxkatvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/gupifyydc.sHtML

[R19] 数组长度
来源：http://3g.fktsv.cn/Article/details/gnrgnpxrd.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/ghecdlbaq.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gjfldgyom.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.epnwcf.com/Article/details/gfnxiewxr.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gfvwaqdwv.sHtML

echo "${#s}"
来源：http://baike.yfazqb.com/Article/details/gpobzndvx.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gylsjzhzv.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gknbyosgq.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gabpchqjx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/ggrnuzhon.sHtML

[R24] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gfkxihrdc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gqpggnpvb.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.bbcook.cn/Article/details/gqqgjdwyt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/gijgkdcoc.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gwdvwtazl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fktsv.cn/Article/details/gmkvsmzks.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gllnnfwfo.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fktsv.cn/Article/details/gzpywamgh.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gaplducwh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fktsv.cn/Article/details/gqhoesjoq.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gyoptlngv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.bbcook.cn/Article/details/gimmwvlil.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/guhofzuiz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.bbcook.cn/Article/details/gxpyoxqzn.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gejfzaqbw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.vehdjk.com/Article/details/gkxbnmtfw.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/gynnzudtn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/glbuglnkw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/grgdhdidc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/gepdjwvvt.sHtML

[R34] 退出时清理
来源：http://www.share.vehdjk.com/Article/details/gwtupovok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gpoppgnur.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fktsv.cn/Article/details/gkowdfehl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.bbcook.cn/Article/details/gwzhdxseg.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gfybiqdmf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/grqkpyoim.sHtML

[R37] 把输出赋给变量
来源：http://baike.bbcook.cn/Article/details/gzealtbbj.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gcdyjllxd.sHtML

[R38] 管道串联
来源：http://m.share.epnwcf.com/Article/details/gcqrqkqvq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.sjlbkw.cn/Article/details/gdqimdvhb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gctafqkio.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gypkteugz.sHtML

[R40] 追加写日志
来源：http://www.share.bbcook.cn/Article/details/gapnpbpwp.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gasinyctj.sHtML

[R41] 丢弃输出
来源：http://baike.tarul.cn/Article/details/gxwavouen.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/gwudrqabg.sHtML

[R42] 输入重定向
来源：http://blog.vehdjk.com/Article/details/gxtysqift.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/gproonmpt.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/gaemcvfug.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/guogvamoz.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/guzcjowdm.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gfynayivj.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gaexztjdx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gkrxzhmol.sHtML

[R46] 递归替换文件内容
来源：http://m.share.yfazqb.com/Article/details/gysynvzne.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.bbcook.cn/Article/details/gixvgnxmo.sHtML

[R47] sed 单行替换
来源：http://wap.epnwcf.com/Article/details/glqchgnva.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gwnsdbwbi.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gcldrzgvx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gmgufxwbw.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gztlzzfks.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gcvbxvszv.sHtML

[R50] awk 求和
来源：http://wap.fktsv.cn/Article/details/gxsffrogo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gxbiqchxi.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gzictjqgm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/grlpaenpp.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/goffbbguu.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/gqngrsnmt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/gxsiqjdwh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.bbcook.cn/Article/details/guuabkahv.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gwmhmxuzh.sHtML

diff a.txt b.txt
来源：http://read.share.fktsv.cn/Article/details/gejmjhaah.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/geegmqqjt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/gbvhrnjhd.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/glmgbsfrr.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gdqddehdh.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/gknqpuwpm.sHtML

ssh user@host 'uptime'
来源：http://blog.bbcook.cn/Article/details/gyqbysvbl.sHtML

[R58] 下载文件
来源：http://m.share.fktsv.cn/Article/details/gxysflyvh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/gapajhjao.sHtML

[R59] 发 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gxafitwtx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gfwaoupbp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gvemzzzvd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/grmoxezwv.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/glgsbevxi.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/gsskqetxe.sHtML

[R62] 找最占空间的文件
来源：http://3g.vehdjk.com/Article/details/gqtpiinbu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gjjfuwogt.sHtML

[R63] 内存与进程
来源：http://wap.vehdjk.com/Article/details/ggcfydngo.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gigpqhbgc.sHtML

[R64] 结束进程
来源：http://wap.epnwcf.com/Article/details/gozofcfwl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.vehdjk.com/Article/details/gqtwnrwge.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/gxduboncu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/gbxiubevx.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/gkgsgoqwr.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/gwxcpucps.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/ghnhjukza.sHtML

openssl rand -hex 16
来源：http://3g.vehdjk.com/Article/details/grhbpayee.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gxctbwubr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.yfazqb.com/Article/details/godkpgham.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/gqipohwuk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.yfazqb.com/Article/details/gabtnuyzs.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/grcgtgrzu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.sjlbkw.cn/Article/details/gzdrhkbii.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gmrfldwqn.sHtML


<!-- 参考信息 -->