代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.epnwcf.com/Article/details/gdmqltbgu.sHtML

[Q24] 去重
来源：http://www.blog.epnwcf.com/Article/details/gxzunizsv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gchtaitsy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.tarul.cn/Article/details/gjvtecsep.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.sjlbkw.cn/Article/details/gistdlmrg.sHtML

[Q26] 计数
来源：http://mobile.bbcook.cn/Article/details/gusrnambp.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gfyuffhgj.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gqlhdwfqq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gxskhfzzz.sHtML

[Q28] 求和与平均
来源：http://m.share.epnwcf.com/Article/details/gbnyrwxqt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gmelxqlxq.sHtML

[Q29] 最大最小值
来源：http://www.m.share.vehdjk.com/Article/details/genkoctyx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ggullepcx.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/ggbmvkskr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gybyqbiny.sHtML

[Q31] 分组后过滤
来源：http://blog.epnwcf.com/Article/details/giztqaihb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fktsv.cn/Article/details/gfxrlpsww.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/gqawvboae.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/guixpxkkg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/gucfmexen.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gkhflmbdz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.epnwcf.com/Article/details/govwqvvxn.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gqtknnmun.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/giuodymxl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.sjlbkw.cn/Article/details/gipgmaacw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.bbcook.cn/Article/details/geyihfxvy.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gltfvuepq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/ghcsisiew.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gpmmqwros.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gasvnoozx.sHtML

[Q37] 右连接
来源：http://blog.tarul.cn/Article/details/gtprypizc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.bbcook.cn/Article/details/grnnxdxoj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gmhgohukl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gnzwsusfw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/gazhuuzcy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gcodecnhi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/gxtxzwxzz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gvaganzvf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.epnwcf.com/Article/details/gndzkvesf.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/gjofbngux.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/gwaeuqeyb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/gkzfieomn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/geqyymman.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gnisfwpcv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.bbcook.cn/Article/details/gtficuhyc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/gdwacxchf.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/grfgzicss.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gownhkwpn.sHtML

[Q44] IN 子查询
来源：http://read.share.sjlbkw.cn/Article/details/gpaywctnu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fktsv.cn/Article/details/grtxqvnna.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/gatsqsynz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/ggivmtymh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/ggjvoajqs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gjlxsquoc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.epnwcf.com/Article/details/gntdxbbxm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/gtauslfts.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/grtflowrg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gzfnmhuxt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.yfazqb.com/Article/details/gzavuhdnt.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/gmnfkpvkr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gfgkuvrgx.sHtML

[Q50] 批量更新
来源：http://www.share.bbcook.cn/Article/details/guvnidwhi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gwirmlmmb.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/gsvtmcxgv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.tarul.cn/Article/details/gklneaogk.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/gbhubexgo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gxpnnsxdw.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/glpfejloc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/geqbdqhpd.sHtML

[Q54] 清空表
来源：http://wap.epnwcf.com/Article/details/ghultweli.sHtML

TRUNCATE TABLE logs;
来源：http://3g.epnwcf.com/Article/details/gkqddsnta.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/grydsmgro.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/ggijvsfpd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/gmefyykdx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/goowkbuxx.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/gdxparyjh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.yfazqb.com/Article/details/gsuiojqvf.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/glwcpettk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/giqekzwnk.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/gkzegonun.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gvqvpdswi.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.yfazqb.com/Article/details/gqbjqpqiz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.sjlbkw.cn/Article/details/gzpzkjnfk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gbedoqrqp.sHtML

[Q61] 移动平均
来源：http://www.m.share.epnwcf.com/Article/details/gbcibeyhc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gygmaltnx.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/ghvaezygl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gjoiogsja.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gewmzmnxq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fktsv.cn/Article/details/ghrnswsvc.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gdysioatm.sHtML

COMMIT;
来源：http://www.blog.epnwcf.com/Article/details/guccdwuny.sHtML

[Q65] 回滚事务
来源：http://www.blog.tarul.cn/Article/details/gwhujiveu.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gpoblmrir.sHtML

[Q66] 行锁查询
来源：http://mobile.vehdjk.com/Article/details/gzlcngodo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gfnpkctlq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.bbcook.cn/Article/details/gtfmjnwap.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/ghreuffzp.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/gjxmkpxoa.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gwfimbisz.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/glktaouyo.sHtML

[Q69] 查看执行计划
来源：http://baike.vehdjk.com/Article/details/gfcrjpcfy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.bbcook.cn/Article/details/gsttirgeo.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/gjfrmgdqi.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/gututozbq.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/goldjfdeh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gzgddbsxm.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/gxpqympuj.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/geuqpbgxm.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gavonkxeb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gqeqwngkh.sHtML

[Q74] 强制使用索引
来源：http://mobile.tarul.cn/Article/details/gpxakkazc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.yfazqb.com/Article/details/gkwoxyxnm.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gbnoodksk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.tarul.cn/Article/details/gawewbjiw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gbpmjinrm.sHtML

[Q76] 按天统计
来源：http://baike.epnwcf.com/Article/details/gxejvhazc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/gcauvkqkd.sHtML

[Q77] 时间加减
来源：http://wap.bbcook.cn/Article/details/gbkffkcpx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.epnwcf.com/Article/details/gpcepoldj.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/gqrfbyqol.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.vehdjk.com/Article/details/ghhvlkqny.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gjhnzeumn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.vehdjk.com/Article/details/golgdcajf.sHtML

[Q80] 字符串截取
来源：http://baike.yfazqb.com/Article/details/gccsaoili.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/grwfvyriq.sHtML

[Q81] 字符串替换
来源：http://blog.bbcook.cn/Article/details/ghuiooqee.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.bbcook.cn/Article/details/gdafvpaxd.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/grmmleqjs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gmpptqsyz.sHtML

[Q83] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gfgmogtgx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gcyaybwir.sHtML

[Q84] 去除首尾空格
来源：http://baike.yfazqb.com/Article/details/gxdahqtic.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gvjokafaf.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gkudjtyjv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.sjlbkw.cn/Article/details/gcwbbzykn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/gdtxqifxx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.yfazqb.com/Article/details/gtcshbbgn.sHtML

[Q87] JSON 字段做条件
来源：http://3g.sjlbkw.cn/Article/details/gqsnlrltr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gwfbhpwcy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/gkvdziimx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/glhebyfjc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.bbcook.cn/Article/details/grdotmxch.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gcmechxtj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.vehdjk.com/Article/details/gfdtxwkoa.sHtML

[Q90] 生成序号列
来源：http://3g.yfazqb.com/Article/details/ggsdffqsa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/gfecqdwla.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdpuojpss.sHtML

R. Bash 专题
来源：http://3g.tarul.cn/Article/details/gyenydnwh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glqgdneif.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gvbzzpkst.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gsdicdvdk.sHtML

set -euo pipefail
来源：http://read.share.tarul.cn/Article/details/gtzadkfzu.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/gzqhcyatg.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gruxfkiia.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/gdamckotq.sHtML

readonly PI=3.14
来源：http://read.share.vehdjk.com/Article/details/ggbsktdql.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gucztvevb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/gmdnhiseq.sHtML

[R05] 参数默认值
来源：http://read.share.vehdjk.com/Article/details/gqixigmpv.sHtML

name="${1:-default}"
来源：http://read.share.vehdjk.com/Article/details/gugrvpdfo.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gxtruvyzm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gqpbjunil.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/gcrpravom.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/gctqugbqv.sHtML

[R08] 数值比较
来源：http://baike.tarul.cn/Article/details/gnblnrcue.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.yfazqb.com/Article/details/gdagdtszd.sHtML

[R09] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gayqgblao.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.bbcook.cn/Article/details/gmhkmdmkd.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gheuoaqwa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.yfazqb.com/Article/details/gjrsouysx.sHtML

[R11] case 多分支
来源：http://m.share.fktsv.cn/Article/details/grjpsnudj.sHtML

case "$1" in
来源：http://www.m.share.yfazqb.com/Article/details/gngyyzmlt.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gyfpukskc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/gjvfqsmtf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/grwgzaitd.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gkbfjqopl.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gajieeylc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fktsv.cn/Article/details/gbtdcewdl.sHtML

[R13] for 计数循环
来源：http://wap.fktsv.cn/Article/details/glaeaijhc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gzokabyve.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/gkapqrgeg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gqokqutov.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gardqyqhw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/gxkpwoeoq.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/gxpqoliqd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gjwfpoeql.sHtML

[R17] 数组定义与取值
来源：http://read.share.tarul.cn/Article/details/gsezxfgvj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/gkycpjrpa.sHtML

[R18] 遍历数组
来源：http://www.blog.epnwcf.com/Article/details/gehicetmk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.sjlbkw.cn/Article/details/gpsjjezcf.sHtML

[R19] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gdkxiwgic.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gevnqoeul.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/gsbsqghlt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gueyhwtwz.sHtML

[R21] 字符串长度
来源：http://wap.tarul.cn/Article/details/gaclvkryj.sHtML

echo "${#s}"
来源：http://3g.vehdjk.com/Article/details/gcmwgtgsi.sHtML

[R22] 截取子串
来源：http://3g.vehdjk.com/Article/details/gghzcyllp.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gfofktnln.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gmgkmvcwp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gmuckytsr.sHtML

[R24] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gxfamicwp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gyijdwdpr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fktsv.cn/Article/details/grmfnkqkt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/gdosdrquv.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gbcnyjnum.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/giyvgpvqh.sHtML

[R27] 算术展开
来源：http://m.share.vehdjk.com/Article/details/gsrcquyhu.sHtML

echo $((1 + 2 * 3))
来源：http://wap.tarul.cn/Article/details/gciwqrdke.sHtML

[R28] 浮点运算
来源：http://www.m.share.fktsv.cn/Article/details/gusgeidtg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.epnwcf.com/Article/details/gfrefrzqr.sHtML

[R29] 定义函数
来源：http://wap.yfazqb.com/Article/details/giigujfrs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gwdgrsgwm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gjdlkicgp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gcdajgbqq.sHtML

[R31] 局部变量
来源：http://wap.fktsv.cn/Article/details/gtbwrbjur.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/gfnhdqbha.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gwwzvvucg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gwzzgfpok.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.tarul.cn/Article/details/ggukgopnj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gztxbcpcq.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gprspreqy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrswsoqo.sHtML

[R35] 后台执行并等待
来源：http://baike.fktsv.cn/Article/details/giqjegnpc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gsatbqjgd.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.sjlbkw.cn/Article/details/gjfxmqejc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.sjlbkw.cn/Article/details/gswzlpyta.sHtML

[R37] 把输出赋给变量
来源：http://blog.epnwcf.com/Article/details/giklbkciu.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/goscjkfbc.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/glegpnasz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/gmtlljout.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gcuhixaxo.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/glixthnwx.sHtML

[R40] 追加写日志
来源：http://www.share.vehdjk.com/Article/details/gncreksyr.sHtML

echo "log" >> out.log
来源：http://www.blog.yfazqb.com/Article/details/guyhkyxsj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/ghufyabfo.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/gotpawplv.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/giwubsvid.sHtML

wc -l < a.txt
来源：http://www.share.fktsv.cn/Article/details/gvjqlydpg.sHtML

[R43] 按名字查找文件
来源：http://blog.bbcook.cn/Article/details/gjwqkhijw.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gmszqvlew.sHtML

[R44] 按修改时间查找
来源：http://m.share.sjlbkw.cn/Article/details/gdhlmahrz.sHtML

find . -mtime -7 -type f
来源：http://read.share.yfazqb.com/Article/details/gcjpinttj.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/gurrctwbu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/gkezdnjlj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gbaldskby.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.yfazqb.com/Article/details/gkwmsqdid.sHtML

[R47] sed 单行替换
来源：http://3g.epnwcf.com/Article/details/gawkvnckz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gnsrdkrax.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/gpdgusawa.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gpnsjtljb.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/gpcyrfzhj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gecehfrin.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/gudmpvkpn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gcpfoqmio.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gkwritmea.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gtdtreqdk.sHtML

[R52] 统计行数
来源：http://3g.fktsv.cn/Article/details/gndasfbvt.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/gafeedtlf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.sjlbkw.cn/Article/details/gelbhcavw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/gawjuxjhg.sHtML

[R54] 比较两个文件
来源：http://3g.vehdjk.com/Article/details/gmswqkuph.sHtML

diff a.txt b.txt
来源：http://read.share.sjlbkw.cn/Article/details/guvdbbjtt.sHtML

[R55] 压缩与解压
来源：http://wap.bbcook.cn/Article/details/gaqncngcf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gowcxohjc.sHtML

[R56] 远程拷贝
来源：http://www.blog.yfazqb.com/Article/details/grukdrhbo.sHtML

scp file user@host:/path/
来源：http://m.share.epnwcf.com/Article/details/gpcudbvrh.sHtML

[R57] 远程执行命令
来源：http://www.share.epnwcf.com/Article/details/gpbqwugrb.sHtML

ssh user@host 'uptime'
来源：http://www.share.tarul.cn/Article/details/gjieqqbjz.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/gnbuznejg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gaprharpn.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gdlbhdsiv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gyajjheso.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gawhaynqt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gskpfxckg.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gvtodsmch.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/ggujljmof.sHtML

[R62] 找最占空间的文件
来源：http://read.share.epnwcf.com/Article/details/gmmwlsxsz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/ggzfqnkih.sHtML

[R63] 内存与进程
来源：http://m.share.sjlbkw.cn/Article/details/gbftarewm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fktsv.cn/Article/details/gvyjtjefa.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/galjbkach.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gaflnnjlr.sHtML

[R65] 查看端口占用
来源：http://baike.epnwcf.com/Article/details/gkncdmoyp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.epnwcf.com/Article/details/gxnwnwrig.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gdizpmiaf.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gapsiijre.sHtML

[R67] 生成随机十六进制串
来源：http://blog.sjlbkw.cn/Article/details/gpnyqmcgo.sHtML

openssl rand -hex 16
来源：http://www.blog.bbcook.cn/Article/details/gxlfcjkgg.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gmwjibqfd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.epnwcf.com/Article/details/gtipjfuxb.sHtML

[R69] 生成随机密码
来源：http://mobile.vehdjk.com/Article/details/gwwfforox.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fktsv.cn/Article/details/gyigwlvsy.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/glszsamuf.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gehfqohqq.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gnoyyklap.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaiyogtw.sHtML

[R72] 等待端口就绪
来源：http://m.share.tarul.cn/Article/details/gcpqpndld.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/glwvfujrp.sHtML

[R73] 分割大日志
来源：http://blog.sjlbkw.cn/Article/details/gjryibynw.sHtML


<!-- 参考信息 -->