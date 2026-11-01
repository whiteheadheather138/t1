代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/gtibvtzym.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gxyngmlwv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.vehdjk.com/Article/details/gikwbiths.sHtML

[Q21] 空值判断
来源：http://mobile.sjlbkw.cn/Article/details/gdmuycxrw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gocuhzyln.sHtML

[Q22] 排序
来源：http://baike.sjlbkw.cn/Article/details/gjpagnnzi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.vehdjk.com/Article/details/gejlchhll.sHtML

[Q23] 分页
来源：http://baike.yfazqb.com/Article/details/grhgxbrho.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.tarul.cn/Article/details/grqdoagcz.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gslmvjbwq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.bbcook.cn/Article/details/gyaflrhmd.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/ggtiybngm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/gcykfwwtb.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/ggvokjidt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gjlcwwxzq.sHtML

[Q27] 条件计数
来源：http://www.share.epnwcf.com/Article/details/gjxmgrrkk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gxgvxpvmh.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/gwgexkbzi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gqxutlhcx.sHtML

[Q29] 最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/gfgviukkd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gidivgtjg.sHtML

[Q30] 分组统计
来源：http://m.share.epnwcf.com/Article/details/glltqpdzi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gqixmocsf.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/gwyhjabfr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gdoudnysl.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/gnqkmbgpj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gcwfnezxf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gtcfznpll.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/glorvmfkf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.tarul.cn/Article/details/gaipbbwei.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.sjlbkw.cn/Article/details/giwbmwuzs.sHtML

SELECT * FROM (
来源：http://read.share.epnwcf.com/Article/details/gljcfbssk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnowxsqn.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gysrxyksu.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/gbztqtgwn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/guwbuxkdp.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/gqyqdoogt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gxgnjqwvi.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gxolbhxxi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.vehdjk.com/Article/details/gnlxntefj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.yfazqb.com/Article/details/gsjzdilwx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.epnwcf.com/Article/details/gyhacnmxr.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gtcixrugu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gmmknyilf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/ghgokuihn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/ggsdfegel.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/gwecrfkwp.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gsowyqfgm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/gsoerwcwj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/gxzclkgxi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.bbcook.cn/Article/details/gpgxnnzht.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fktsv.cn/Article/details/gnocflslo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gwmleirqw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fktsv.cn/Article/details/gkxfvfkep.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/gqvgtqayr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/guhgsjbjz.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/gkcmpouqz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.tarul.cn/Article/details/gbmdgxrxa.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/geyacvagl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gggpvjnld.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gophhyasj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gdtskcrxn.sHtML

[Q47] 与平均值比较
来源：http://www.share.bbcook.cn/Article/details/gihmxwxsr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.epnwcf.com/Article/details/gkgokykgn.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/gmhwcvijo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/gdixdafjw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.yfazqb.com/Article/details/gvnkybpog.sHtML

[Q49] 更新单行
来源：http://www.blog.yfazqb.com/Article/details/gojqacjbm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/glbxfojzs.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/ggdwddbra.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gijiefgsz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gqebpfley.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gnkaphxgd.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gvvovpchk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/guimppela.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gyeorrkmc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/gmiheliai.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/garlhwwwy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.yfazqb.com/Article/details/gqszjatvj.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/giuxswyqy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gdcfhlzjm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.vehdjk.com/Article/details/gtdvmvjog.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gghhqkznu.sHtML

[Q57] 行号
来源：http://wap.yfazqb.com/Article/details/ggckanfzv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gsqjeqgfl.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/gdhstvtlu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/giojturau.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gsdnrmdmm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gllwyvmvc.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/gjwttauft.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gdascveil.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gmgortygj.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gzqexznsa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/ganlshznf.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gjqjdivyn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gcmdzgfjr.sHtML

[Q63] 开启事务
来源：http://3g.vehdjk.com/Article/details/ggvydpadc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.sjlbkw.cn/Article/details/gnmrfqqhd.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/gmgwhbena.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/gzuublcax.sHtML

[Q65] 回滚事务
来源：http://www.share.bbcook.cn/Article/details/gyfnggnxn.sHtML

ROLLBACK;
来源：http://www.blog.vehdjk.com/Article/details/gyrodawvt.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/gxevubcwu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.sjlbkw.cn/Article/details/ggrjxlwkm.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/gqgwzapfd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.epnwcf.com/Article/details/gsqodcaen.sHtML

[Q68] 保存点
来源：http://www.share.sjlbkw.cn/Article/details/gkqoxeafe.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/gwqbsgezz.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gbohyatdv.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gjevycwob.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.yfazqb.com/Article/details/gkfhnyoen.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/gsgwkpixi.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/gucnisybc.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gzneiuzvu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/gkbcopzoy.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gqbrgdvbw.sHtML

SHOW INDEX FROM users;
来源：http://wap.epnwcf.com/Article/details/gebiytfas.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/gaspplrqy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.tarul.cn/Article/details/gblyscqgu.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gvuaznjal.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gflvffkwj.sHtML

[Q75] 日期格式化
来源：http://blog.tarul.cn/Article/details/gplkesxph.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gcualdoyg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/gxtkkqquf.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/gwifygdji.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gszufsbft.sHtML

[Q77] 时间加减
来源：http://wap.vehdjk.com/Article/details/gmrtrnyyp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.vehdjk.com/Article/details/gkccrhdnf.sHtML

[Q78] 当前时间
来源：http://mobile.yfazqb.com/Article/details/gmhxpadsm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.tarul.cn/Article/details/gavpvckgc.sHtML

[Q79] 字符串拼接
来源：http://wap.yfazqb.com/Article/details/gsxnnizam.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/grbztytos.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/giwrscrov.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fktsv.cn/Article/details/gfbwlpfvn.sHtML

[Q81] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gpofukjyp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/gskzplamj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gtttotdeu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gfdbpcpsx.sHtML

[Q83] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/guzxebhwn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gedlcalbg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/gzfxzdklr.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gtjknmfom.sHtML

[Q85] 数值取整
来源：http://www.blog.bbcook.cn/Article/details/gdobxjutp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gvcpwhsha.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gxophjvkb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fktsv.cn/Article/details/gglhhtzss.sHtML

[Q87] JSON 字段做条件
来源：http://3g.epnwcf.com/Article/details/gslnlfmcm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gkbounxax.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fktsv.cn/Article/details/govvbeyir.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/gpwtpsisi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.vehdjk.com/Article/details/gwlvdmchs.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/glhuifoio.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.sjlbkw.cn/Article/details/guvdmpojh.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/gorpjwyfs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/gkvhtunli.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/goyewmhyt.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gckoyfycd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfklhlxvx.sHtML

[R01] shebang 与严格模式
来源：http://www.share.bbcook.cn/Article/details/gafxbljvb.sHtML

#!/usr/bin/env bash
来源：http://wap.tarul.cn/Article/details/gtfcueioh.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gajjbnqbl.sHtML

[R02] 变量赋值与使用
来源：http://mobile.sjlbkw.cn/Article/details/gbolssnrr.sHtML

name="Tom"; echo "$name"
来源：http://3g.epnwcf.com/Article/details/gudtgvmam.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gemywdqil.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/geaigjnfr.sHtML

[R04] 位置参数
来源：http://baike.epnwcf.com/Article/details/gqgfhmjey.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/gabluxoir.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/glxodvrxh.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/gynfviimi.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/guwvulccw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gjkgypvyt.sHtML

[R07] if 判断文件
来源：http://www.share.epnwcf.com/Article/details/gikbqikep.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/gkiqxswuu.sHtML

[R08] 数值比较
来源：http://www.m.share.epnwcf.com/Article/details/gftgsefpf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.epnwcf.com/Article/details/gpzblgaho.sHtML

[R09] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/goexhjcen.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.bbcook.cn/Article/details/gpirgmxdl.sHtML

[R10] 正则匹配
来源：http://wap.fktsv.cn/Article/details/gstdcsani.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/gfoucljxd.sHtML

[R11] case 多分支
来源：http://m.share.bbcook.cn/Article/details/gxdtlebag.sHtML

case "$1" in
来源：http://www.m.share.vehdjk.com/Article/details/gbxyqbzlj.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxexlhujh.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/gueriovxs.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.vehdjk.com/Article/details/genpvxtfj.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/guzynjetw.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/ggjjeaikt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.bbcook.cn/Article/details/gxnjbhydx.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/grokuwrmj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gltfsbzwd.sHtML

[R14] C 风格 for
来源：http://3g.tarul.cn/Article/details/gncrdzgse.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/gsxqstegs.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/guxvhbprp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.bbcook.cn/Article/details/gumuhzepl.sHtML

[R16] until 等待条件
来源：http://blog.tarul.cn/Article/details/gqsfirafh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/govxwcdte.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gqztaxbua.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/gxkbwbqxg.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/gyzmxxucn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/gigudbsqj.sHtML

[R19] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gghyolmgz.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gaxbxgore.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.vehdjk.com/Article/details/gmianthjq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.epnwcf.com/Article/details/gnpgvghhx.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/gjehmfxdd.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gwkmtfbdl.sHtML

[R22] 截取子串
来源：http://wap.tarul.cn/Article/details/gdegejibz.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gzbnngqjb.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gdoyxetba.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/gyqjezunr.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/glklvfbaa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.epnwcf.com/Article/details/gfdoeiskr.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/gzxsbrofd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fktsv.cn/Article/details/gfvlqbybx.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/gmpxtsidf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/gwqcuepvh.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gtxhvhorv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/gilwybgja.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/ghkuepeqz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gcyjegrdi.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gmclvjnmq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gftiwjmvm.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/gfzdunpid.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gzxhwswnc.sHtML

[R31] 局部变量
来源：http://mobile.bbcook.cn/Article/details/gvmmefsne.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.sjlbkw.cn/Article/details/grrfykjpw.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/giisyvcsd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gcmcamqyr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/gdbmwnyue.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/gdlwnwmmy.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/gllnivjqj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gvjfrgquw.sHtML

[R35] 后台执行并等待
来源：http://www.share.epnwcf.com/Article/details/gymfovnxb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/gvftjlxqk.sHtML

[R36] 并发执行多个任务
来源：http://mobile.bbcook.cn/Article/details/gnryvomys.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gezkmxxnq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/grfutreog.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gofazpsqh.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gxwyvyhzi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gjwandqhc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.sjlbkw.cn/Article/details/glhbjeaha.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gaxftcchg.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gdoyqjpqq.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gbdyvaxck.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/gvklvirah.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gmmtwohzb.sHtML

[R42] 输入重定向
来源：http://mobile.bbcook.cn/Article/details/gmecrejkh.sHtML

wc -l < a.txt
来源：http://baike.bbcook.cn/Article/details/gshfwcdhg.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/goscsdhma.sHtML

find . -name "*.log" -type f
来源：http://read.share.fktsv.cn/Article/details/gcjazjert.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gnzoukkdw.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gtecxynvv.sHtML

[R45] 批量删除
来源：http://baike.fktsv.cn/Article/details/guxuczrvg.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gnqotyups.sHtML

[R46] 递归替换文件内容
来源：http://blog.epnwcf.com/Article/details/gsiqmyaew.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.yfazqb.com/Article/details/gyszlzsfo.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gqwjklyxz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gtwuiykbc.sHtML

[R48] awk 取指定列
来源：http://baike.sjlbkw.cn/Article/details/gchsnvvfg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gacveedcw.sHtML

[R49] awk 带条件
来源：http://wap.fktsv.cn/Article/details/gfhrizeuz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/gpgsemhrf.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gnibyluzt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/gxzhmvoms.sHtML

[R51] 排序去重取前几
来源：http://3g.fktsv.cn/Article/details/gqcnnqkde.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gfgjsvcjb.sHtML

[R52] 统计行数
来源：http://wap.bbcook.cn/Article/details/gnrbikjqd.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/gmupvvtwt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gttpcdemw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fktsv.cn/Article/details/giianjoee.sHtML

[R54] 比较两个文件
来源：http://blog.epnwcf.com/Article/details/ghbfwbvkl.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/gffogdlkh.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/gfqpqfjwt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/ghsdtocyk.sHtML

[R56] 远程拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gvvfvxfjc.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gfwrenshq.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gvmnnewxs.sHtML

ssh user@host 'uptime'
来源：http://wap.vehdjk.com/Article/details/gltornpbq.sHtML

[R58] 下载文件
来源：http://www.share.bbcook.cn/Article/details/gqxanoutn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/grpstguoz.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/glnszhasf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.epnwcf.com/Article/details/gpxavhckt.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gsllvnlnb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.tarul.cn/Article/details/gxogistni.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/gvdnhynvh.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/gpqrdzunt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fktsv.cn/Article/details/genhrssyu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.bbcook.cn/Article/details/greoqhrbv.sHtML

[R63] 内存与进程
来源：http://read.share.tarul.cn/Article/details/gdhffiobo.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.epnwcf.com/Article/details/gssjcfvuh.sHtML

[R64] 结束进程
来源：http://read.share.tarul.cn/Article/details/gifigxchh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fktsv.cn/Article/details/grmkumfuu.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gqtqxghvk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/gspocurca.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gowfvuypk.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/gxrvzyfay.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/gzhqbomuw.sHtML

openssl rand -hex 16
来源：http://mobile.fktsv.cn/Article/details/gznqbyzyt.sHtML

[R68] 计算文件校验值
来源：http://mobile.sjlbkw.cn/Article/details/gqjmupwah.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gaqtkkuda.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkmpkayx.sHtML


<!-- 参考信息 -->