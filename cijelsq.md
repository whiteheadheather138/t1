代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gxdhhcxwy.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/glyujnrlx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gdqbwhssh.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/gfrdthpsl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/gyuckfnmk.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/glonvijwq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.bbcook.cn/Article/details/ggmiyacnw.sHtML

[Q21] 空值判断
来源：http://baike.fktsv.cn/Article/details/gmcldegqf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gzsemsmxr.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/gyrjqyjui.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gppzrwjcj.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gwfoipmci.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.epnwcf.com/Article/details/gwgsycsbm.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/gnthfvpmq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.tarul.cn/Article/details/gxidhpclh.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/gjntbgghw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.epnwcf.com/Article/details/gsumqgdze.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/ggkjflngd.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.epnwcf.com/Article/details/gzowkvjio.sHtML

[Q27] 条件计数
来源：http://read.share.tarul.cn/Article/details/gklfkxbie.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/guzsfbybf.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gmrsircru.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gguhveguk.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/ghufiwffl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fktsv.cn/Article/details/gauhsurfy.sHtML

[Q30] 分组统计
来源：http://www.share.fktsv.cn/Article/details/gxjddlxwz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/ggdaiptrf.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gvjmcblrp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gpgwzbfkj.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gcevhvyqb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gxwwxrlvu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/gcuonfhrd.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gnxlbyrkm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gqwdvvwxb.sHtML

[Q34] 每组取第一条
来源：http://wap.fktsv.cn/Article/details/gwagqyvhl.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/glmoutzub.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gghqpeknd.sHtML

) t WHERE rn = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gkudvyjfw.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/gkqzmjzom.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gjjfnzihw.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/gaeanwajw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/grsoygefo.sHtML

[Q37] 右连接
来源：http://read.share.vehdjk.com/Article/details/geespmyqm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.epnwcf.com/Article/details/geddtckiq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/gdratihsv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.yfazqb.com/Article/details/gwadeqqwf.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gusbqjmoi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gfsbpxqtd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.yfazqb.com/Article/details/gtooqsqjq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fktsv.cn/Article/details/gakpwvfvr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/gihrvfvrj.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gpmbfpbok.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gkcionywe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.vehdjk.com/Article/details/girxknjmo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gaucfjomu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fktsv.cn/Article/details/gtbxoxmrv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.yfazqb.com/Article/details/gajccfwzd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.vehdjk.com/Article/details/gftxgotri.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gpopevkhj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.tarul.cn/Article/details/gqjvtndci.sHtML

[Q44] IN 子查询
来源：http://mobile.fktsv.cn/Article/details/gadpqalrp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.tarul.cn/Article/details/gjoapvcuf.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/gevsdwiak.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gycyjmkdn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/glmsxurkn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/gwdrzfrpw.sHtML

[Q47] 与平均值比较
来源：http://blog.vehdjk.com/Article/details/grtucgfmc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.tarul.cn/Article/details/gnndhwfpt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.bbcook.cn/Article/details/gumeivoee.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxdudarc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.yfazqb.com/Article/details/giqsuaflg.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gufhmshyh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gzowjvilb.sHtML

[Q50] 批量更新
来源：http://m.share.fktsv.cn/Article/details/gglrnvril.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.yfazqb.com/Article/details/gboskmjaa.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gwbytycpq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fktsv.cn/Article/details/gwilopwhr.sHtML

[Q52] 删除指定行
来源：http://wap.sjlbkw.cn/Article/details/gbjvicteu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gsidmvqal.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gbfjgxode.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.epnwcf.com/Article/details/gpuwvwbcq.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gxvotniho.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/geiazydqh.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/ghyuaswse.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gwjkicltl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gnwszbxik.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gguxqwjrm.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gxbtiwgvn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gixbdbtui.sHtML

[Q58] 累计求和
来源：http://m.share.sjlbkw.cn/Article/details/gqhtpfbpk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gbsyfhstf.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/gwdiiwpji.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gqcvytixm.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.sjlbkw.cn/Article/details/gwkiftdjo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.vehdjk.com/Article/details/gwbynzskt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gxdemshwg.sHtML

[Q61] 移动平均
来源：http://blog.epnwcf.com/Article/details/givtsprzj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gwufnpsrm.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/gofwqygte.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/goehzpqqs.sHtML

[Q63] 开启事务
来源：http://read.share.yfazqb.com/Article/details/gpwsckoys.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/gvutowugg.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gynawmkvz.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/godklxrvs.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gjjywquld.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/gismawlsr.sHtML

[Q66] 行锁查询
来源：http://mobile.sjlbkw.cn/Article/details/gdlpgqxsa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.tarul.cn/Article/details/gdiwclnck.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/gfxdzvzcj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gmdicorux.sHtML

[Q68] 保存点
来源：http://baike.vehdjk.com/Article/details/gvfnxkepk.sHtML

SAVEPOINT sp1;
来源：http://wap.yfazqb.com/Article/details/gbykbtjik.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gdglptzpa.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/gmpclrguq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.bbcook.cn/Article/details/gjrooudng.sHtML

[Q70] 更新统计信息
来源：http://wap.yfazqb.com/Article/details/gkkclzgbp.sHtML

ANALYZE TABLE users;
来源：http://3g.epnwcf.com/Article/details/gaxirrqto.sHtML

[Q71] 查看建表语句
来源：http://3g.epnwcf.com/Article/details/grhdbtnwf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gliyxufdf.sHtML

[Q72] 查看索引
来源：http://mobile.sjlbkw.cn/Article/details/gstdqhwmy.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gnviolocn.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/ggvkiuvpf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.bbcook.cn/Article/details/gyagbbvqp.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/godviaxdx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gxlyduluw.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gyaqknvxz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.vehdjk.com/Article/details/gmheeyriq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gomrogtyv.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/gpeulzfqc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/gtzdtttqq.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gyocgcexx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.yfazqb.com/Article/details/gxgudyqvc.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/guuvdbnaq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/gaastkptx.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/goxcwgaac.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fktsv.cn/Article/details/glquuxste.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/gqxgvfoer.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gcnrggqxh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gwglhmgav.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.tarul.cn/Article/details/ggfyslwry.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gxohkgjlw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/geyfdbbng.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gkwewcmxa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gcyowivxo.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/gvrwavmhe.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gunzvzrgd.sHtML

[Q85] 数值取整
来源：http://blog.fktsv.cn/Article/details/gyijrlwzx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/guvaczmch.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/gpvkatuhk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gbcqlckll.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.epnwcf.com/Article/details/gjmbqbjtv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.vehdjk.com/Article/details/gccpqantv.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gbyihgvcj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gtqetxsox.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gylnupiro.sHtML

[Q89] 判断表是否存在
来源：http://read.share.bbcook.cn/Article/details/gukmpitrb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gqqoprfza.sHtML

[Q90] 生成序号列
来源：http://www.share.epnwcf.com/Article/details/ggwmtijfg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gxblojaqc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkmsnvjle.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gczdkyocl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gsfvyjbpn.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.tarul.cn/Article/details/gxahdbdkf.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/gwumuiepw.sHtML

set -euo pipefail
来源：http://www.m.share.tarul.cn/Article/details/gfxzflpak.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/ggzgillxj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gkbgcdhjy.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gkqqxgdlp.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/gidgnvrlf.sHtML

[R04] 位置参数
来源：http://www.blog.epnwcf.com/Article/details/gmdhhfety.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpfvonby.sHtML

[R05] 参数默认值
来源：http://read.share.vehdjk.com/Article/details/gykqoepzw.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gwsvqkdgh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.yfazqb.com/Article/details/gqpkqixzq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gqjwbvyuv.sHtML

[R07] if 判断文件
来源：http://blog.vehdjk.com/Article/details/gmgwkxqyw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gxqjgwqay.sHtML

[R08] 数值比较
来源：http://www.share.bbcook.cn/Article/details/gndmbqemo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gufpcadpg.sHtML

[R09] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gztqpvcda.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gicwgxjgu.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/geikvvmpf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/genmrdzvk.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/gpsqbgjso.sHtML

case "$1" in
来源：http://www.m.share.epnwcf.com/Article/details/guumxzzxn.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gjykjqrxe.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gnzuhzzib.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/goslhahpp.sHtML

esac
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnkxlztw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gyhdcjemm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/gxoogrsnt.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnkgdfkw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gueugunlx.sHtML

[R14] C 风格 for
来源：http://mobile.fktsv.cn/Article/details/gomogjnyq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/grbsozski.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gipcasfjy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/gnauwypyx.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gzdaamoof.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gjanoehlk.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gyaiezolm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.sjlbkw.cn/Article/details/grgdszrdr.sHtML

[R18] 遍历数组
来源：http://blog.tarul.cn/Article/details/gjoucufcw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.epnwcf.com/Article/details/gntfmmkal.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/ggrqkydwg.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gixutahcp.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fktsv.cn/Article/details/grbkspybm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.epnwcf.com/Article/details/grxuypfwf.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gzgknauqz.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gfxgegxgh.sHtML

[R22] 截取子串
来源：http://3g.tarul.cn/Article/details/gjbnwxvro.sHtML

echo "${s:0:5}"
来源：http://m.share.vehdjk.com/Article/details/glajqlvua.sHtML

[R23] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gnceoqfgc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxbcacsg.sHtML

[R24] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gmtozrxhu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gapmxucpm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.bbcook.cn/Article/details/gbqgnngoc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/gpvdfvobn.sHtML

[R26] 命令替换
来源：http://www.share.fktsv.cn/Article/details/glzzbgurh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.epnwcf.com/Article/details/gevmgcruk.sHtML

[R27] 算术展开
来源：http://www.share.sjlbkw.cn/Article/details/gygrfgazj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gvologfoi.sHtML

[R28] 浮点运算
来源：http://baike.sjlbkw.cn/Article/details/gksywhvhn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gyyxhvxbb.sHtML

[R29] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gruatxqyk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gfgeedluv.sHtML

[R30] 函数返回状态码
来源：http://baike.tarul.cn/Article/details/galrhqpwq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.vehdjk.com/Article/details/gdhuqutrq.sHtML

[R31] 局部变量
来源：http://read.share.epnwcf.com/Article/details/gdgotslqf.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.sjlbkw.cn/Article/details/gzwwczmpo.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/giihumkxp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/gaauwikux.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.sjlbkw.cn/Article/details/gtcepivkv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/gitvakkfk.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/gmhotiqnx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/gdmllgzti.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/gqhmxmnof.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/gyugaofks.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/geslygtuo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.yfazqb.com/Article/details/gsxzjvopx.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/geuqyolrx.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/graybbwsf.sHtML

[R38] 管道串联
来源：http://read.share.epnwcf.com/Article/details/gtlramubi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.yfazqb.com/Article/details/gzwfwpuum.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/gbxwinlde.sHtML

cmd > out.log 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gakaupyue.sHtML

[R40] 追加写日志
来源：http://www.share.fktsv.cn/Article/details/gnizgkbax.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gufldrcgr.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gpgavhtru.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/gzldvjlyh.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/grppfyrni.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/gffqqmorj.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/grhmazlxi.sHtML

find . -name "*.log" -type f
来源：http://blog.tarul.cn/Article/details/gltiwsmsl.sHtML

[R44] 按修改时间查找
来源：http://wap.fktsv.cn/Article/details/gdqkzkhvj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.tarul.cn/Article/details/guwkyutjh.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gatonuslr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.yfazqb.com/Article/details/gxcqphsiu.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.bbcook.cn/Article/details/gaeaukawd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.vehdjk.com/Article/details/gfazfqliy.sHtML

[R47] sed 单行替换
来源：http://mobile.epnwcf.com/Article/details/ggvvkfpai.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/gtgtworsm.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/ggkqqekrz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gtceiclhp.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gnlmdlaua.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/gsszxoczu.sHtML

[R50] awk 求和
来源：http://www.blog.tarul.cn/Article/details/gewlnmxpw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/ggtxgwfgs.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gdgvwnfxl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fktsv.cn/Article/details/gelytemqz.sHtML

[R52] 统计行数
来源：http://www.blog.epnwcf.com/Article/details/gdxmuzeyx.sHtML

wc -l a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqbubric.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gkknfozor.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.bbcook.cn/Article/details/gwqnehplt.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gmlzhcfmu.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/glbbhpbdq.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/guymkjvew.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.bbcook.cn/Article/details/goqomdenj.sHtML

[R56] 远程拷贝
来源：http://blog.epnwcf.com/Article/details/gyylytomj.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gcstoiulq.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/guarthusb.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/geaoamitn.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gtrijxpvq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.epnwcf.com/Article/details/gswhyhjgm.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gmwshrvcb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gjpceynfd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/grjchrszk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gymbxmpsl.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gdejhmhgv.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/godgnbgtg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.sjlbkw.cn/Article/details/gprkswhan.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gopvajfev.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/giwtmhfcj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.tarul.cn/Article/details/gtoayjljj.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gbupnnwwk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpktpyotq.sHtML

[R65] 查看端口占用
来源：http://mobile.bbcook.cn/Article/details/gexxelmos.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/ggkozkqvs.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gacdmftdg.sHtML

crontab -e;  crontab -l
来源：http://wap.vehdjk.com/Article/details/gwrmdxarw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.vehdjk.com/Article/details/gqagpyaiz.sHtML


<!-- 参考信息 -->