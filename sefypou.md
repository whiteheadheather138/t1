代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.bbcook.cn/Article/details/gddypxuxf.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/guslpgscb.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gkrxmhqws.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/gpedhuyqj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gaeabjpoc.sHtML

[Q28] 求和与平均
来源：http://m.share.tarul.cn/Article/details/gijlgjjip.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gdprfcnyo.sHtML

[Q29] 最大最小值
来源：http://www.blog.fktsv.cn/Article/details/gdvikbqns.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqtkwouee.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gwrxseeeq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gmqsbfqok.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/ggsbxfnph.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/glybrzbep.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gdjehojnp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gytbwtrsq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/ghdjjvgve.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gavehafzk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/glqsmrrvl.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gdkhwbcjb.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/gypdoyhln.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/gwfutkuyd.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gblqjajnp.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/gczlciplf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gmctrgkbd.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gepldcwrl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gwaxnhmmk.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gtrkxbust.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/guurilabe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.sjlbkw.cn/Article/details/gyyytsmkn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/grzkhhokc.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gdyhnogkf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gpketfhzg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fktsv.cn/Article/details/gzbksobxz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/gxjzducnf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.vehdjk.com/Article/details/gftgtrlam.sHtML

[Q41] 多表连接
来源：http://m.share.yfazqb.com/Article/details/gplrheeiw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fktsv.cn/Article/details/gzesekreh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gmjrlzjdg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.epnwcf.com/Article/details/gockejsjs.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.vehdjk.com/Article/details/ggwfcydhz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/geruuowed.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/gakrezrit.sHtML

[Q43] 标量子查询
来源：http://www.share.bbcook.cn/Article/details/gjcpyjmah.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gwzqqzvoj.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/gbebgqdde.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.vehdjk.com/Article/details/gikxjitmk.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gkfxturom.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gekpypdzb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gxruuonhf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gxuejjdjo.sHtML

[Q47] 与平均值比较
来源：http://baike.yfazqb.com/Article/details/gatfaxlra.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.sjlbkw.cn/Article/details/gqqljkqie.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/gkihctlyc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.vehdjk.com/Article/details/ggbdnbyim.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gdzoidxrr.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gqnlwnrvj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gzigrrdts.sHtML

[Q50] 批量更新
来源：http://read.share.sjlbkw.cn/Article/details/gjydmgjsf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.epnwcf.com/Article/details/ghjuptxwp.sHtML

[Q51] 用子查询更新
来源：http://wap.sjlbkw.cn/Article/details/gyhrcaodv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gsqqohdcw.sHtML

[Q52] 删除指定行
来源：http://m.share.fktsv.cn/Article/details/ghhqbiqao.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gfqbeidyg.sHtML

[Q53] 按条件删除
来源：http://mobile.bbcook.cn/Article/details/gtspcuqjd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gzbzihlvb.sHtML

[Q54] 清空表
来源：http://www.share.tarul.cn/Article/details/gansvejyq.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.yfazqb.com/Article/details/gixavprmj.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/glupltvto.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gcfpynizp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gzyhujzlx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gmlxfscyx.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/gyodhimyh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.epnwcf.com/Article/details/gkoaftkqz.sHtML

[Q58] 累计求和
来源：http://blog.vehdjk.com/Article/details/grbymhzqb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gvpmfamhn.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/gywobqjin.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gaemeeoxx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.sjlbkw.cn/Article/details/gsizhvbcq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gqtdhfuwn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.tarul.cn/Article/details/gmyftcgcq.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/gcccbwwck.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gslnvirkd.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/gxbyhmgsy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/ggbjjkhnn.sHtML

[Q63] 开启事务
来源：http://wap.sjlbkw.cn/Article/details/gqnivblru.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gubkeaalt.sHtML

[Q64] 提交事务
来源：http://blog.epnwcf.com/Article/details/gtanfslwe.sHtML

COMMIT;
来源：http://wap.sjlbkw.cn/Article/details/gbpnoarga.sHtML

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/gxrylcscs.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gavbegaug.sHtML

[Q66] 行锁查询
来源：http://www.share.epnwcf.com/Article/details/gvgymwxpd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.epnwcf.com/Article/details/gclejcyaz.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gcwdblrrj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.bbcook.cn/Article/details/gldcpdksy.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gdwpnzvop.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gbfpmtnxx.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gfagmfrzk.sHtML

[Q69] 查看执行计划
来源：http://blog.bbcook.cn/Article/details/goljfoxhw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.yfazqb.com/Article/details/gfafjwcvt.sHtML

[Q70] 更新统计信息
来源：http://mobile.bbcook.cn/Article/details/gqzeicaus.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/givwzsjrn.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gkavglivk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/ggkqzgtaq.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/gsuralahm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gpsroaxbz.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/geozfszmg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.vehdjk.com/Article/details/gdlbkatxx.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/gjhzsgbgi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/glnaggzga.sHtML

[Q75] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/giabbnzhh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gshgugmmd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gparfnzga.sHtML

[Q76] 按天统计
来源：http://baike.bbcook.cn/Article/details/gxugobriw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.tarul.cn/Article/details/gfxwqhzlo.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/ghttmcher.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.vehdjk.com/Article/details/gxpnqcpzu.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gdetpwvit.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/gqpxyasfn.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gyujiifcc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.yfazqb.com/Article/details/gfqnmhkuh.sHtML

[Q80] 字符串截取
来源：http://www.blog.bbcook.cn/Article/details/gbenotqna.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gwnklfwlp.sHtML

[Q81] 字符串替换
来源：http://www.share.tarul.cn/Article/details/gkmgaytnz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gzehmenne.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.epnwcf.com/Article/details/ghjumicnj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gzyqqokse.sHtML

[Q83] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gatdnjbtk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gemsqqdtk.sHtML

[Q84] 去除首尾空格
来源：http://baike.yfazqb.com/Article/details/gxxaypyep.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gbjrrfzji.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gzwgcbnxj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gjwojoaed.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/goekkwqht.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/gicrgttoy.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gluwblipo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gutjxbost.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.sjlbkw.cn/Article/details/gkxeysdmu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gfvxodsgt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gufvlhxwd.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gpkdosygn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.yfazqb.com/Article/details/giuhnbfgy.sHtML

[Q90] 生成序号列
来源：http://baike.fktsv.cn/Article/details/ghcbgwijq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gkwrklceb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gldxpmxci.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/guvwzrqjv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdrzgdkof.sHtML

[R01] shebang 与严格模式
来源：http://m.share.bbcook.cn/Article/details/ghfkrxoda.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/gywzkmapc.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/gdkvnektt.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gqrvzqgdc.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/gfqajbfch.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/gwjdepjol.sHtML

readonly PI=3.14
来源：http://www.m.share.vehdjk.com/Article/details/gsonnkfwc.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/gazmvlosd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.epnwcf.com/Article/details/gpivrfmmm.sHtML

[R05] 参数默认值
来源：http://wap.tarul.cn/Article/details/gxejzjgvw.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gbgkkjmjs.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gutnxqacd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gpdgyvxfk.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gwmedojzo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/gckfwgnye.sHtML

[R08] 数值比较
来源：http://mobile.epnwcf.com/Article/details/gysvvdllp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.sjlbkw.cn/Article/details/gwespwigm.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gmemqnzmf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gyudxjdly.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/grsnsairm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gquywvgiu.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gmonqvjvk.sHtML

case "$1" in
来源：http://www.m.share.epnwcf.com/Article/details/gqudepqxt.sHtML

start) echo "启动" ;;
来源：http://www.blog.yfazqb.com/Article/details/gwzhglytu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/glszcwqqh.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gwqamkdbm.sHtML

esac
来源：http://www.blog.fktsv.cn/Article/details/gccbpbkkc.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/grhcswixs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.tarul.cn/Article/details/gszterwlo.sHtML

[R13] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gitsyzqyt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gweegelgv.sHtML

[R14] C 风格 for
来源：http://www.share.fktsv.cn/Article/details/gzcdjukyt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gaystvqbe.sHtML

[R15] while 逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gaxkmzjsd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.yfazqb.com/Article/details/gskggxchk.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gusdhvaty.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/ghoeivcwv.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gebptjzoq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gbkurapgr.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/guirygkso.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gsojztdic.sHtML

[R19] 数组长度
来源：http://3g.bbcook.cn/Article/details/gmvzkwucf.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gwkfrgyqa.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlnpewif.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gbvrbmkfs.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gitunerre.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gjrhlkosz.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/goyoaagvh.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gzsihvjnx.sHtML

[R23] 字符串替换
来源：http://blog.bbcook.cn/Article/details/grfhuhvrp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gsxrhwquv.sHtML

[R24] 大小写转换
来源：http://wap.tarul.cn/Article/details/gskcotvnj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gslvjqvny.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gwsqtftiq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gaiivokcn.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/galvecykp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fktsv.cn/Article/details/ggskredaz.sHtML

[R27] 算术展开
来源：http://blog.fktsv.cn/Article/details/gvtanljgf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gbadysuwu.sHtML

[R28] 浮点运算
来源：http://blog.epnwcf.com/Article/details/gfvycbdwh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.vehdjk.com/Article/details/gxnqasouv.sHtML

[R29] 定义函数
来源：http://wap.yfazqb.com/Article/details/glvvsodhz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.yfazqb.com/Article/details/gehqhdwuv.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gkcugzmmx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.tarul.cn/Article/details/gvkpmjdgo.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/ghlhctiuy.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/gmoedcrog.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/gwxylkzix.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/giackszmq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gupoxkzpj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/grgbkaugb.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/ggvhlcldx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gvqdezwqf.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gbktiuopo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gfswoqpcf.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gljkoxbxd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gizazshbc.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gsuibrrnh.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gvkorfqru.sHtML

[R38] 管道串联
来源：http://www.m.share.epnwcf.com/Article/details/gyixhxydh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.vehdjk.com/Article/details/gntfvuvnp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.bbcook.cn/Article/details/guarmskmv.sHtML

cmd > out.log 2>&1
来源：http://blog.yfazqb.com/Article/details/gfwmgjbhl.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gwitulsnn.sHtML

echo "log" >> out.log
来源：http://mobile.sjlbkw.cn/Article/details/gszooxjyv.sHtML

[R41] 丢弃输出
来源：http://3g.vehdjk.com/Article/details/gperyrsph.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gbovdacig.sHtML

[R42] 输入重定向
来源：http://www.blog.fktsv.cn/Article/details/gfiaflvzn.sHtML

wc -l < a.txt
来源：http://3g.bbcook.cn/Article/details/gucgoefjj.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gtbfofaqi.sHtML

find . -name "*.log" -type f
来源：http://www.share.bbcook.cn/Article/details/gtrnvocrp.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gbzkgdvid.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gqbdqzzym.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/ggjshwozr.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/gelzyotbv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/gsnvstgwl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gztpjkjph.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/gtxpruncu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gpursicwf.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gymtjumqm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gwlozjokc.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/gsyppvvoc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gmhgjmioh.sHtML

[R50] awk 求和
来源：http://baike.vehdjk.com/Article/details/gnendfpas.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/ggnsplfph.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gvokvpyje.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gifibljyb.sHtML

[R52] 统计行数
来源：http://www.share.epnwcf.com/Article/details/gpqatcnkn.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gmeyykcyo.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.bbcook.cn/Article/details/gxpwmyayz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gutorjnig.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gvicidfsc.sHtML

diff a.txt b.txt
来源：http://mobile.bbcook.cn/Article/details/gcmsxemeh.sHtML

[R55] 压缩与解压
来源：http://www.m.share.vehdjk.com/Article/details/gwremminw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/glxizhkev.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/ghjsgwxaq.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gwuphgyca.sHtML

[R57] 远程执行命令
来源：http://3g.fktsv.cn/Article/details/gtdvqugmp.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gjkpoibzb.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gikgsfqdh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fktsv.cn/Article/details/gfsbbthfx.sHtML

[R59] 发 POST JSON
来源：http://baike.tarul.cn/Article/details/gvykpacia.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gzodyeemm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gynulqiil.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/giijnxrmj.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gutfvzcvy.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/gkblzqecp.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/gfvdxycdi.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gmhtaonpg.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gdjczzbed.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.vehdjk.com/Article/details/gmrqfllrw.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gnytglumg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/goohqwwbs.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/gaectnsds.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fktsv.cn/Article/details/gyhpnbkzd.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gjocwxpta.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gtvisbgjr.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.sjlbkw.cn/Article/details/giuhpcggr.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/griuyzoip.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gbrhltpye.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gxzoizwoj.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/gpiolypva.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.vehdjk.com/Article/details/gnjneatlc.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/guxeyjuke.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gjrqmbufk.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gvhaonxty.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gkynnmkzo.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/ghpgvprlx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gklznmlyv.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/gaswdmhhr.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gctccazcl.sHtML

[R74] 批量重命名
来源：http://baike.vehdjk.com/Article/details/gdscdroxc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gstjllcri.sHtML

[R75] 导出环境变量
来源：http://m.share.vehdjk.com/Article/details/gywyfvyee.sHtML


<!-- 参考信息 -->