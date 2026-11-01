代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/ggwedwctf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/gejnzbmoh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/gpxmudqdu.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/gmswqjjuz.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/gixytsvmx.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/gbwlxqitg.sHtML

SELECT id, name FROM users;
来源：http://mobile.fktsv.cn/Article/details/glirirhtc.sHtML

[Q17] 条件查询
来源：http://baike.yfazqb.com/Article/details/gnhytlfxt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.vehdjk.com/Article/details/geeluyrhu.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/glkccuxrm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.bbcook.cn/Article/details/gfqyhpryy.sHtML

[Q19] 范围查询
来源：http://m.share.tarul.cn/Article/details/guamnakls.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/gvedyrqoh.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gvecfhzef.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gplyawtek.sHtML

[Q21] 空值判断
来源：http://www.m.share.yfazqb.com/Article/details/galfqtvnt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gpbexshuy.sHtML

[Q22] 排序
来源：http://mobile.sjlbkw.cn/Article/details/gfqyglinx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/gdiqpxyyp.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gcvebyypg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.tarul.cn/Article/details/gcrbfzqnn.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gicfygaeq.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gfsmuxruj.sHtML

[Q25] 只取前 N 条
来源：http://wap.fktsv.cn/Article/details/gkpzjrggi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/ggjdlbczl.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/grjdyibnf.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/gxtesazpd.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gduzpmaev.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gvswohrma.sHtML

[Q28] 求和与平均
来源：http://www.share.yfazqb.com/Article/details/geohxsnty.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gaesjbeno.sHtML

[Q29] 最大最小值
来源：http://wap.fktsv.cn/Article/details/gayilpbiz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gcujwxncm.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gnsktkhyb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gyruyfknk.sHtML

[Q31] 分组后过滤
来源：http://mobile.fktsv.cn/Article/details/gbgrookqd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.bbcook.cn/Article/details/gwymijelg.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gmbmjdzjj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gkbmdtece.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gqqgypbun.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/glbgaihvt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.vehdjk.com/Article/details/gaxbnvhjq.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/ggmxnoaah.sHtML

SELECT * FROM (
来源：http://3g.bbcook.cn/Article/details/gtnhxqtub.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.bbcook.cn/Article/details/gbgyfzkhd.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/gxwtddoqh.sHtML

[Q35] 内连接
来源：http://read.share.fktsv.cn/Article/details/gquslumih.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gpvekjjhf.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gohiavspz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gzqgkqetp.sHtML

[Q37] 右连接
来源：http://m.share.bbcook.cn/Article/details/gxpksjwjc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/gtvoorsyy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/ghxzpxlkx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.tarul.cn/Article/details/grgoxchhp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.vehdjk.com/Article/details/gubiogjlb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/gspcidbji.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/ghleiftnp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.yfazqb.com/Article/details/gutceupls.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gfqwseram.sHtML

[Q41] 多表连接
来源：http://www.m.share.vehdjk.com/Article/details/gsnwoorap.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gonaqzuyt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.bbcook.cn/Article/details/goeeqiowf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/grkvrlmmw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.tarul.cn/Article/details/gjyvzvuso.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gpwyyjrmf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.vehdjk.com/Article/details/gsbvtzexu.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gfzobxgst.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/gewlpieep.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/guerfycvd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fktsv.cn/Article/details/glyksiotb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.vehdjk.com/Article/details/gabtwqkvu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gamgpgbqu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fktsv.cn/Article/details/ghgoysemt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gpeytqccp.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/gfsjsziqt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.epnwcf.com/Article/details/guitcsvrv.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.sjlbkw.cn/Article/details/gzvfkntpn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gdriszaeu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gcxarfpok.sHtML

[Q49] 更新单行
来源：http://m.share.fktsv.cn/Article/details/ghconoyem.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gjrcvsmlh.sHtML

[Q50] 批量更新
来源：http://baike.sjlbkw.cn/Article/details/gbxgtclbc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gloijtkwt.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gxteunool.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.yfazqb.com/Article/details/gecrpurdy.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/gjnzoxtzk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gokxioyxx.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/gugqjjczo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.bbcook.cn/Article/details/gwuyloagq.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/gxbfellha.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fktsv.cn/Article/details/grwiscdan.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.yfazqb.com/Article/details/gxxhltrlq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fktsv.cn/Article/details/gsauabobq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/gagjrjzxq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gbsapbtwj.sHtML

[Q57] 行号
来源：http://mobile.fktsv.cn/Article/details/gcljxxcfq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/glivmhxks.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/gzkflsmsq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gicmikaxz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gkbweyfnw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gdhhwkjvs.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.yfazqb.com/Article/details/glkbtectq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gcjhhvsdh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.bbcook.cn/Article/details/gbxymlotg.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gamddkfhr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gftldflwt.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gpqqcuoxq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gndyipdqp.sHtML

[Q63] 开启事务
来源：http://www.blog.fktsv.cn/Article/details/geirtpflj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gdbjvwcvr.sHtML

[Q64] 提交事务
来源：http://3g.yfazqb.com/Article/details/gglomhnis.sHtML

COMMIT;
来源：http://wap.epnwcf.com/Article/details/giyagykax.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/ggdcajhbb.sHtML

ROLLBACK;
来源：http://mobile.tarul.cn/Article/details/gpyrmxcdl.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/gobbhkwrl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.bbcook.cn/Article/details/gzyqvoebv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.yfazqb.com/Article/details/goullhigg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.epnwcf.com/Article/details/gdijjjnjp.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gafkcsnja.sHtML

SAVEPOINT sp1;
来源：http://baike.sjlbkw.cn/Article/details/gpjkidpdc.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gciuablrh.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gqqjpmasi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.bbcook.cn/Article/details/gfgyffuah.sHtML

[Q70] 更新统计信息
来源：http://blog.yfazqb.com/Article/details/gtmajxeto.sHtML

ANALYZE TABLE users;
来源：http://www.blog.sjlbkw.cn/Article/details/gxhlaujhu.sHtML

[Q71] 查看建表语句
来源：http://blog.yfazqb.com/Article/details/gejqivurp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/gpwzhgeuv.sHtML

[Q72] 查看索引
来源：http://read.share.fktsv.cn/Article/details/gstnwopbx.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gwajwgybs.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/gpdzdxsiu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gfmrqjthe.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/gzojbkowm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.tarul.cn/Article/details/gexpdklbn.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gccxxnonu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gqekukcqf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/gjrkzrjnn.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/ghiiioote.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.yfazqb.com/Article/details/ghciltvxa.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gainsduzx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gyhtdlhhz.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/gckqczhfr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gipjbdvzv.sHtML

[Q79] 字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gjbcimone.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/gmzyphgov.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/gcmduaodf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/glgynqfbx.sHtML

[Q81] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/goptkvgjt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/gpojrmhlt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gwzkpwmhy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gvvpvixzm.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gzeittiee.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.tarul.cn/Article/details/grqyrkxos.sHtML

[Q84] 去除首尾空格
来源：http://mobile.epnwcf.com/Article/details/gbokkwqye.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gkbsajmku.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gwwwjutkn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.epnwcf.com/Article/details/ggzjqwfbw.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.sjlbkw.cn/Article/details/gbvmpusxg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gryxqefmj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/gamxfhqmi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gorweeecr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.epnwcf.com/Article/details/gmycmaatx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.yfazqb.com/Article/details/goqoqnvrk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gaequmjfh.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fktsv.cn/Article/details/gcamxppvh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/gfeuguzou.sHtML

[Q90] 生成序号列
来源：http://www.share.tarul.cn/Article/details/gbaypbvbx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/grxbtucea.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gydtaqcfu.sHtML

R. Bash 专题
来源：http://3g.vehdjk.com/Article/details/gmgjkqkql.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpbfldyzw.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/gblravvgg.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gtgpfckkv.sHtML

set -euo pipefail
来源：http://wap.tarul.cn/Article/details/geqorsfpg.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gwtsqurnd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.yfazqb.com/Article/details/gulopjwjk.sHtML

[R03] 只读变量
来源：http://www.m.share.bbcook.cn/Article/details/ggbxnytdh.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gklqyrnlw.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gjnbfaqok.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.epnwcf.com/Article/details/gnuwujzcu.sHtML

[R05] 参数默认值
来源：http://3g.yfazqb.com/Article/details/gmtctrvfu.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/grgygipvz.sHtML

[R06] 判断命令是否存在
来源：http://baike.sjlbkw.cn/Article/details/gunkjyame.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gwcogdmlr.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gablcdtqv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/gmxhlmsoj.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/gmwsfftlg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/grxymamdz.sHtML

[R09] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gopqqbbuq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/gxsxkymdt.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/gubckqvdo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/glxouvvma.sHtML

[R11] case 多分支
来源：http://m.share.epnwcf.com/Article/details/grppprwyj.sHtML

case "$1" in
来源：http://baike.epnwcf.com/Article/details/gwzrodfpf.sHtML

start) echo "启动" ;;
来源：http://www.share.tarul.cn/Article/details/grktxvjcx.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gjwehijlm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fktsv.cn/Article/details/gmjqbiera.sHtML

esac
来源：http://baike.bbcook.cn/Article/details/gnprvspev.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/glwzyntng.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gbrmacyxb.sHtML

[R13] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/girxqbume.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gvpbieldj.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gkifzitmd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/goahhfawl.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gelzzfyxa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.vehdjk.com/Article/details/ggdhnjufn.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/gtsihnugt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gmjvlguxn.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/gajdqywxo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fktsv.cn/Article/details/gqbbvwigf.sHtML

[R18] 遍历数组
来源：http://baike.vehdjk.com/Article/details/gcmxbsjtk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gpvzcwfxg.sHtML

[R19] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gaodxpptc.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/gmtdkcikh.sHtML

[R20] 关联数组（字典）
来源：http://wap.fktsv.cn/Article/details/gbzuodahs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gmjbkkhyx.sHtML

[R21] 字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gthvluvzx.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gjnvnftny.sHtML

[R22] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/ghikqxqps.sHtML

echo "${s:0:5}"
来源：http://baike.epnwcf.com/Article/details/glhhssxmz.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gcrstdqaz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/gslzwvakc.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gwwsukyoi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fktsv.cn/Article/details/gjzmckltl.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/gdfortjyd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/guqisfcux.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gubhfgdka.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.vehdjk.com/Article/details/gwohpegrx.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gucztbkmu.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gmhmeilrl.sHtML

[R28] 浮点运算
来源：http://baike.fktsv.cn/Article/details/gpzxomlqy.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gonhuatvn.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/giczjyigu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gwtkvxqik.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gvjhxxjfz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fktsv.cn/Article/details/gwzxjhqlz.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gkbgynpve.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gxpjorvvl.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/gwwqkijus.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gnsjnsjzs.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gsvduooib.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gkqusxsoz.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/gopigmrdv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gisuyfksm.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gbpafyjem.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.vehdjk.com/Article/details/gdpzgfwqw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/gaoekhhuo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gbraxjggo.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gjjkrgyly.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gqyslryba.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gacvmjyud.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fktsv.cn/Article/details/gjoowvygv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/guzraokcu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gbntgmnec.sHtML

[R40] 追加写日志
来源：http://3g.bbcook.cn/Article/details/gmvloofda.sHtML

echo "log" >> out.log
来源：http://blog.tarul.cn/Article/details/gndqlwgfv.sHtML

[R41] 丢弃输出
来源：http://blog.epnwcf.com/Article/details/ggrhbyfmz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gzevzbjbm.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gehubsddt.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gnektjwob.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/ghplkqjzl.sHtML

find . -name "*.log" -type f
来源：http://read.share.fktsv.cn/Article/details/gjjadglpm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.vehdjk.com/Article/details/gakznlmvl.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gprsjamuv.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gnropvfui.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gaicfgxmd.sHtML

[R46] 递归替换文件内容
来源：http://baike.bbcook.cn/Article/details/gifyyhebq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gakjxltbq.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gltayhoaw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.epnwcf.com/Article/details/gfpxhwqsv.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/ggjyrnohy.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.bbcook.cn/Article/details/gnhzzoceq.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/gsnxrmdlv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fktsv.cn/Article/details/gzefcgjgp.sHtML

[R50] awk 求和
来源：http://www.blog.tarul.cn/Article/details/gmzgbvlcn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gfqnmobst.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gcfmqmmnu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/gwwlmfbcb.sHtML

[R52] 统计行数
来源：http://baike.vehdjk.com/Article/details/gjinbmryo.sHtML

wc -l a.txt
来源：http://www.blog.vehdjk.com/Article/details/gtjtgrkod.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/gqonpiqbt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/gsievepax.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/gwkhxuqpj.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gsdfvvrbw.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gdjxbnmxc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/ghcqirkji.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gvyeibpxe.sHtML

scp file user@host:/path/
来源：http://mobile.fktsv.cn/Article/details/gazmofsnb.sHtML

[R57] 远程执行命令
来源：http://baike.epnwcf.com/Article/details/gqgzoeglr.sHtML

ssh user@host 'uptime'
来源：http://www.share.yfazqb.com/Article/details/gmgtjmunk.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gnjouopow.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fktsv.cn/Article/details/gsnxjcfjz.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gbmbmfrzs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/gqbmcwuzp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gvjpnjbgs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gpcqyzdee.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/geuxsikui.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/ggtozutlo.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gveqzafnc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/guuiulssj.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gijpobgld.sHtML


<!-- 参考信息 -->