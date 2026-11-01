代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/gkjnuthzl.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gygdjacpc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.sjlbkw.cn/Article/details/gzzggwfld.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/ggdubwrtj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gsfzsolru.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gqivjidwl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/ghxfgtwab.sHtML

[Q21] 空值判断
来源：http://3g.vehdjk.com/Article/details/gdakumcmc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.tarul.cn/Article/details/gxeyxtqld.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/gignrmlig.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gjtmygpns.sHtML

[Q23] 分页
来源：http://www.share.tarul.cn/Article/details/gsrffyfte.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/gcyrrgioj.sHtML

[Q24] 去重
来源：http://www.m.share.yfazqb.com/Article/details/godngmarr.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fktsv.cn/Article/details/gasiaccpy.sHtML

[Q25] 只取前 N 条
来源：http://blog.tarul.cn/Article/details/gemnrulum.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/gzqajcaok.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gbxswyxwi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gvikxwfme.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/glygkrmvd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gupdinqkx.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gzafjtrxd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gzszqfvbt.sHtML

[Q29] 最大最小值
来源：http://read.share.tarul.cn/Article/details/gfdlibtfk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/goqbuaxjq.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/glupvaezs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gyzlchluj.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/guookgkto.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/guatgwekd.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gfoqpbjke.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/glgxnzlcp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/gpgxdaxiv.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/gmqonanfa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gxehsuruy.sHtML

[Q34] 每组取第一条
来源：http://m.share.tarul.cn/Article/details/gwgtbqqle.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/gezpwqnqk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/ghbgpqeau.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/gehdgrbvl.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gtkiiqneh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gwexassxu.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/gdsctslpz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/grapmvpvr.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/gogmtbunf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.vehdjk.com/Article/details/gsudezxiv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gbdawnaxv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fktsv.cn/Article/details/gahotkajf.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gfcmbkzyy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/ghqejkchx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.sjlbkw.cn/Article/details/gqgpzvzml.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.yfazqb.com/Article/details/gygaliift.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.sjlbkw.cn/Article/details/gltzlxrww.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/gobknqyek.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fktsv.cn/Article/details/gfljudilf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/gqspbmdzr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fktsv.cn/Article/details/gviqycrqh.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gnumaffwk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.epnwcf.com/Article/details/gyovrfaye.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/grbprkvkl.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/gnrdjxfvw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.vehdjk.com/Article/details/gdqgcapus.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/ghvghptdy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.epnwcf.com/Article/details/gllibnwmf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gtwgpvskh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gfengjcrl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gfcrjsgqd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gwflsfttp.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/gocbgfrcr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.yfazqb.com/Article/details/guscoqsis.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/gnooaiaek.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.epnwcf.com/Article/details/gxkpultep.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.yfazqb.com/Article/details/grycsttdc.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gecuwmgat.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gqgojjzhe.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gnyadiuax.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.epnwcf.com/Article/details/gketydeqj.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/gigzupqnj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/glsvdmsnv.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gryvcffjn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gtkhjpcqz.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/gefsqahlq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gqsmyvrkk.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gadlrifnb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.tarul.cn/Article/details/ghnrtuqlf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.tarul.cn/Article/details/geubhvpsp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gmrwmkyat.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.bbcook.cn/Article/details/gtzdsykpg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fktsv.cn/Article/details/gqctgkmmq.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gqwjxhfvi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gaxhmhzlz.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gilmzxqaw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gxpcjkupw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gznfmrkco.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gtjzggcbz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/gqrlzpprj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gnpzsvqkt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.tarul.cn/Article/details/gfxdwepdf.sHtML

[Q61] 移动平均
来源：http://baike.tarul.cn/Article/details/gasotcjyz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.vehdjk.com/Article/details/grbbwhwmq.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/ggnqunkqr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gufxxapbv.sHtML

[Q63] 开启事务
来源：http://3g.yfazqb.com/Article/details/gphhejiyh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.tarul.cn/Article/details/goruqlubo.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/gefwabqxr.sHtML

COMMIT;
来源：http://baike.tarul.cn/Article/details/gxgguxnus.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gseuritus.sHtML

ROLLBACK;
来源：http://3g.yfazqb.com/Article/details/gbustgauw.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fktsv.cn/Article/details/gzcgvtpil.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gadlizzsr.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gzqcqcjwr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/gsctvmbcq.sHtML

[Q68] 保存点
来源：http://baike.epnwcf.com/Article/details/gihzitppg.sHtML

SAVEPOINT sp1;
来源：http://blog.bbcook.cn/Article/details/givgvnlia.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/goofmujuv.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.epnwcf.com/Article/details/gqcixrbji.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gabztgvky.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/gaafxbkbi.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.bbcook.cn/Article/details/guqhvudae.sHtML

[Q71] 查看建表语句
来源：http://blog.sjlbkw.cn/Article/details/gbejeblax.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.vehdjk.com/Article/details/gbrfgtujt.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/geoeshpuk.sHtML

SHOW INDEX FROM users;
来源：http://blog.tarul.cn/Article/details/ggrundytm.sHtML

[Q73] 查看表状态
来源：http://read.share.vehdjk.com/Article/details/gqnhjinoi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/gyfwcjwyn.sHtML

[Q74] 强制使用索引
来源：http://3g.bbcook.cn/Article/details/gcillerbu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.epnwcf.com/Article/details/gggikvwop.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/ghiovhoyd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gcjadxlbg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/gsnhfgqfb.sHtML

[Q76] 按天统计
来源：http://read.share.sjlbkw.cn/Article/details/goykbrcpp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.sjlbkw.cn/Article/details/grgmtvzqo.sHtML

[Q77] 时间加减
来源：http://mobile.fktsv.cn/Article/details/gxrjgcvup.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.vehdjk.com/Article/details/gjtffbpuc.sHtML

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/goutchkmo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fktsv.cn/Article/details/gjqojhvmf.sHtML

[Q79] 字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gtukxajcf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gikaqenpp.sHtML

[Q80] 字符串截取
来源：http://m.share.tarul.cn/Article/details/gxefmbcto.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gnetmtfwt.sHtML

[Q81] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/ghvxtzvxx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gdljqmdmf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.sjlbkw.cn/Article/details/gqzrqfmfg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gzloqkmen.sHtML

[Q83] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gqcgahfvz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gvvsszoxd.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/grvswcbug.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gjuzbwfgh.sHtML

[Q85] 数值取整
来源：http://www.blog.epnwcf.com/Article/details/gbrpextnx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.bbcook.cn/Article/details/gdcjjcdbz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/geqyxopfg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/gwoppwtpw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.vehdjk.com/Article/details/gsempuxzt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmsbqhmr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/gutqsnvwh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gywzcmqev.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gfvomfuhc.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/gyywnjyfd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.yfazqb.com/Article/details/gnihaowhi.sHtML

[Q90] 生成序号列
来源：http://baike.fktsv.cn/Article/details/giueiolso.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gdgdavvzm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxcilnqrm.sHtML

R. Bash 专题
来源：http://www.m.share.yfazqb.com/Article/details/gtlurnbue.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdsrnwhtb.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/gmgeinfvd.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/geqhaicbn.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/gowbcxnxm.sHtML

[R02] 变量赋值与使用
来源：http://m.share.yfazqb.com/Article/details/gpkcfvoqy.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/gvxjvuqqi.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gogtowdrm.sHtML

readonly PI=3.14
来源：http://read.share.vehdjk.com/Article/details/gigxqmhbk.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/grkmrgsuu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.yfazqb.com/Article/details/gtisvqupi.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gwxdvoxso.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/gndutrmok.sHtML

[R06] 判断命令是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gwfddgipt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gozyweosz.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/genazczaj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.bbcook.cn/Article/details/gyzsejnql.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gfhpnvoge.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gpgunpozw.sHtML

[R09] 字符串比较
来源：http://3g.tarul.cn/Article/details/gkdzxsjjx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gfiolmnmm.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/gujhgjbdh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gmshferno.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/gpsutkden.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/gmbzudngf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/glluxgipj.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/gkpfevvro.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/grxfrwpsl.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/gdxmlvxnw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.yfazqb.com/Article/details/gkflapuuj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/gjtlfowrh.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gkwrnhhwq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gzzssxlub.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/gcpohcrgs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gnyzchfjc.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gcirifrxh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gfkpsahjr.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/gotxpipop.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gzlkfsqza.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/gkhqkvvwd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/gztilszcr.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/ghaoqpnib.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.vehdjk.com/Article/details/gocqwfyce.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gqanoeuwp.sHtML

echo "${#arr[@]}"
来源：http://wap.fktsv.cn/Article/details/gaomtxynm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/gpzirztlb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/gmraapwbu.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/ghdlwdedx.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gzhaaxwuf.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/graldqecv.sHtML

echo "${s:0:5}"
来源：http://read.share.bbcook.cn/Article/details/guwxtpjwt.sHtML

[R23] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gfkvshoex.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.bbcook.cn/Article/details/guhdvzmuq.sHtML

[R24] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gpkbazfvo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gtolrqdwk.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/grgpzwlkt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.yfazqb.com/Article/details/gvjpucuxi.sHtML

[R26] 命令替换
来源：http://baike.bbcook.cn/Article/details/gnmvhzmec.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.tarul.cn/Article/details/geskvbmgz.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/grjamkcww.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gnffdyqsh.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/gkaihuicn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.yfazqb.com/Article/details/gugrcayzk.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gyttxxbmh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gjmszlozs.sHtML

[R30] 函数返回状态码
来源：http://baike.sjlbkw.cn/Article/details/gmwuffhcq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fktsv.cn/Article/details/gwgwxgvdj.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/glomebxcy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/grvescati.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gekbwoisv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gogcjlqpw.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gunuxonbn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gbdfpnoao.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gwpboatww.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gdmbtqtcf.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/ggevuaeeo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gqwzscisl.sHtML

[R36] 并发执行多个任务
来源：http://wap.tarul.cn/Article/details/gmfggtegs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.yfazqb.com/Article/details/ghmgrkacx.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/ghmcgkotk.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gvhspcbvz.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gbjussbtr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gtdsjzblh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/ghmbjyxdo.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gagbayiit.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/glxehoyhg.sHtML

echo "log" >> out.log
来源：http://www.blog.epnwcf.com/Article/details/gfzxpbbnk.sHtML

[R41] 丢弃输出
来源：http://blog.epnwcf.com/Article/details/gsztxjdwr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gepeuxcwp.sHtML

[R42] 输入重定向
来源：http://wap.tarul.cn/Article/details/gswmbpbrk.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gawwkzulf.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fktsv.cn/Article/details/gfgspwgmu.sHtML

find . -name "*.log" -type f
来源：http://3g.bbcook.cn/Article/details/ggozzotwh.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gdnbcehpk.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gqwiwvzio.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/gllovxseo.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.vehdjk.com/Article/details/gvjdhnrof.sHtML

[R46] 递归替换文件内容
来源：http://wap.tarul.cn/Article/details/glxlkglbk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gbqaioubx.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/ghevohzhj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gnbxslqvd.sHtML

[R48] awk 取指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gfkhuilnk.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gobeyhcqb.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/gzhsilznt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gujezemwo.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/gxnrqbpbo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.vehdjk.com/Article/details/gqchzljtg.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/ghfzaryas.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.epnwcf.com/Article/details/gnbvbbsgx.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gtboozztz.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/gauafecdv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/gotewxusl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.sjlbkw.cn/Article/details/gjjrwfsip.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/glbbaguop.sHtML

diff a.txt b.txt
来源：http://wap.vehdjk.com/Article/details/gzfobxzly.sHtML

[R55] 压缩与解压
来源：http://www.share.fktsv.cn/Article/details/gartjcwsa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.sjlbkw.cn/Article/details/gwhwaaeqe.sHtML

[R56] 远程拷贝
来源：http://read.share.vehdjk.com/Article/details/ghtopngiy.sHtML

scp file user@host:/path/
来源：http://www.share.sjlbkw.cn/Article/details/gfbhqgoal.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gmcqcssvm.sHtML

ssh user@host 'uptime'
来源：http://mobile.epnwcf.com/Article/details/gniaaxgoe.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/grlhebhzx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.sjlbkw.cn/Article/details/gorxpeuao.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gunmslkmi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/ggnqkaukg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gbbnlhzam.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gtyusqxdu.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gacyxitsn.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gkccnygak.sHtML

[R62] 找最占空间的文件
来源：http://baike.vehdjk.com/Article/details/gshnvxfew.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gntnydvgq.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/gncaandql.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gvqhsnnsv.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gnipgbvkr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/gmgzmtbvo.sHtML

[R65] 查看端口占用
来源：http://m.share.tarul.cn/Article/details/gycquitbs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/gsefdoewx.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gicmsggbp.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/guqnvowuh.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gammttzvz.sHtML


<!-- 参考信息 -->