代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.share.tarul.cn/Article/details/gtihokzdh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gznbnyiva.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.yfazqb.com/Article/details/guqvsxtnw.sHtML

[Q15] 查询全部
来源：http://blog.epnwcf.com/Article/details/gqicjripg.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gcnoepcby.sHtML

[Q16] 查询指定列
来源：http://www.m.share.yfazqb.com/Article/details/gtebkppla.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gkrgvqkui.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/gpluxwjuu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gbwzbudkg.sHtML

[Q18] 模糊匹配
来源：http://www.blog.vehdjk.com/Article/details/gwjfwrusn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/gcmadiaqn.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/gpfifsele.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.yfazqb.com/Article/details/gqbultgfq.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/gyvvcjinj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.epnwcf.com/Article/details/givvaqkmy.sHtML

[Q21] 空值判断
来源：http://baike.bbcook.cn/Article/details/gqfrvrjbd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.vehdjk.com/Article/details/gqbooitin.sHtML

[Q22] 排序
来源：http://baike.epnwcf.com/Article/details/gmccfeleh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/ghzgmriqf.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/gmjatoouv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gjmupadwk.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gefvkrrcx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/guoivtepf.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gvxzyjfur.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gejueoxcz.sHtML

[Q26] 计数
来源：http://www.m.share.tarul.cn/Article/details/gxwvkzovn.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/grmpvzovy.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/gtdbplrwk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gtolvnpme.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gjgmxxsom.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gsceskrog.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gmpoxqjnq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/galddqpqp.sHtML

[Q30] 分组统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpuyjjda.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gffoekibt.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/gxwbyionk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.tarul.cn/Article/details/gwezekmcg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gshugpldr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gcdcsfhct.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/ghybuesxi.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gmlwjzhnk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.sjlbkw.cn/Article/details/gzdtsobop.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gtggaqfcr.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/gddiaozeh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gmbfmnrvy.sHtML

) t WHERE rn = 1;
来源：http://www.blog.yfazqb.com/Article/details/gkqmzffcm.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/grnhgmmgo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gjnjqcppi.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gfvzyeeow.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gqhsikkkr.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/ghpvbzslj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gbwpftowo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/gbvljffoe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfuxvajn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gyeazuvor.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.bbcook.cn/Article/details/gzkgcxlry.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.bbcook.cn/Article/details/gbdpqglku.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.vehdjk.com/Article/details/gnmqadpes.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gvsvvvrrf.sHtML

[Q41] 多表连接
来源：http://www.share.yfazqb.com/Article/details/gtkcnonls.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/gsrtvdkhd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.sjlbkw.cn/Article/details/glbpvqpij.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/gwjboeivk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gsojsqrwu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/gjcjnjhgh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.tarul.cn/Article/details/ginbjodkf.sHtML

[Q43] 标量子查询
来源：http://3g.sjlbkw.cn/Article/details/gyjxplxcp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.yfazqb.com/Article/details/gpzhofdyp.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gpwkcdwgt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.sjlbkw.cn/Article/details/gupryqxkr.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/gqjcisrfm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/ggisrqbuw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.yfazqb.com/Article/details/gxbkonquh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gvpabpnbd.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gaagxmuyt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/gkiddahwb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gjnuqxnym.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.sjlbkw.cn/Article/details/gzkqphkyw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gdlvpnodq.sHtML

[Q49] 更新单行
来源：http://www.m.share.fktsv.cn/Article/details/gkprzmuut.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gjoapkror.sHtML

[Q50] 批量更新
来源：http://www.share.bbcook.cn/Article/details/ghtkcdzci.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/guzitbhst.sHtML

[Q51] 用子查询更新
来源：http://baike.yfazqb.com/Article/details/gqjkdssgz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/gkqcijvgq.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gksrvlidw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gbseczioj.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/gjpeuejky.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gfdxqpzkq.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/gygbghfvr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/gyanjdehe.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmpkehjk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/gcceueqbf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gnquqnrng.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/ghjtoipgi.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gotwhrtvr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.yfazqb.com/Article/details/geswrixcn.sHtML

[Q58] 累计求和
来源：http://3g.tarul.cn/Article/details/goudultov.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/guzwfwekt.sHtML

[Q59] 分组内累计
来源：http://m.share.bbcook.cn/Article/details/gbgstembs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gylkznppd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.yfazqb.com/Article/details/gonkcrfzc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.tarul.cn/Article/details/gqwzyphmf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gzzaceqsk.sHtML

[Q61] 移动平均
来源：http://mobile.bbcook.cn/Article/details/gqknxsgwr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/glzudgtaf.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/gojslxrnq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gsglzqtgh.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/gjjeaqyru.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gowdfuhab.sHtML

[Q64] 提交事务
来源：http://www.m.share.yfazqb.com/Article/details/gjxrnvwby.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gygxfwnej.sHtML

[Q65] 回滚事务
来源：http://read.share.vehdjk.com/Article/details/guyiihrbr.sHtML

ROLLBACK;
来源：http://m.share.sjlbkw.cn/Article/details/gapjgndql.sHtML

[Q66] 行锁查询
来源：http://www.m.share.epnwcf.com/Article/details/ghrrtrhhj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.epnwcf.com/Article/details/grtolkblq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.vehdjk.com/Article/details/gndaxjkdh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gdkwbqypj.sHtML

[Q68] 保存点
来源：http://baike.bbcook.cn/Article/details/gxbttwsln.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/grtwohdae.sHtML

ROLLBACK TO sp1;
来源：http://blog.fktsv.cn/Article/details/gpusokgwl.sHtML

[Q69] 查看执行计划
来源：http://read.share.fktsv.cn/Article/details/gutqfueem.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gfsbbgxvo.sHtML

[Q70] 更新统计信息
来源：http://wap.bbcook.cn/Article/details/ghieptlsc.sHtML

ANALYZE TABLE users;
来源：http://blog.sjlbkw.cn/Article/details/gmaukqzar.sHtML

[Q71] 查看建表语句
来源：http://m.share.sjlbkw.cn/Article/details/gvcmjqyjd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.yfazqb.com/Article/details/gtqqzwatl.sHtML

[Q72] 查看索引
来源：http://3g.epnwcf.com/Article/details/grqsatdlf.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fktsv.cn/Article/details/gzmkuxqkn.sHtML

[Q73] 查看表状态
来源：http://blog.epnwcf.com/Article/details/gxzvnitjq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gbtwrywed.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/ghmevehuc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gsgqpmkbk.sHtML

[Q75] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gknpbeucu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gbeownfbn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/ggwizuvms.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gsfeojmnh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.yfazqb.com/Article/details/grdxcgzib.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/gsfquszxe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fktsv.cn/Article/details/gwhjresch.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/gvfabltbp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.yfazqb.com/Article/details/geyfevrlv.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/gqyekftii.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gtehxzoou.sHtML

[Q80] 字符串截取
来源：http://3g.vehdjk.com/Article/details/gaqdewwlr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fktsv.cn/Article/details/gsmetqmei.sHtML

[Q81] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gkltfceae.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gctyiyoff.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.bbcook.cn/Article/details/ghdrcbnqn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqzoshgjn.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gzhhngjue.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gmpjykpmd.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gxnhenceu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gurttycjo.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/gjgvtpipr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/glpcdiyou.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/gdcmlmbki.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/geydghtlu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.tarul.cn/Article/details/gflxxuonw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.epnwcf.com/Article/details/guqqsjwpx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.yfazqb.com/Article/details/gbvomycwd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.yfazqb.com/Article/details/ghnvsioxd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gvqbpyciv.sHtML

[Q89] 判断表是否存在
来源：http://3g.yfazqb.com/Article/details/gxggmlltc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/gblkyakuv.sHtML

[Q90] 生成序号列
来源：http://3g.tarul.cn/Article/details/gjvdppmyo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/gnhtlukck.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guxglvkxw.sHtML

R. Bash 专题
来源：http://www.m.share.vehdjk.com/Article/details/gaupnsnst.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gffxjdxrb.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gsqzgesch.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/goswdwkcg.sHtML

set -euo pipefail
来源：http://mobile.sjlbkw.cn/Article/details/gkjdsectn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/gmgtfursb.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.vehdjk.com/Article/details/gwpvfytvl.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/gzelpwniv.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/gkzgbzcrn.sHtML

[R04] 位置参数
来源：http://www.share.fktsv.cn/Article/details/gxhosjahc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/glxjznytj.sHtML

[R05] 参数默认值
来源：http://www.share.sjlbkw.cn/Article/details/gsjlciqig.sHtML

name="${1:-default}"
来源：http://read.share.epnwcf.com/Article/details/ghiazpcmg.sHtML

[R06] 判断命令是否存在
来源：http://3g.tarul.cn/Article/details/gigiikzqm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.vehdjk.com/Article/details/gxqpyxdot.sHtML

[R07] if 判断文件
来源：http://www.m.share.bbcook.cn/Article/details/grtwwjoga.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/gjlgozdle.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gbbkekdst.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gfbyzeirt.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gscglruji.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.epnwcf.com/Article/details/gxfxjcwtt.sHtML

[R10] 正则匹配
来源：http://wap.bbcook.cn/Article/details/gzbxyxkzi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/gkauvpreq.sHtML

[R11] case 多分支
来源：http://www.blog.yfazqb.com/Article/details/gzaahmwig.sHtML

case "$1" in
来源：http://www.m.share.fktsv.cn/Article/details/gamkpuava.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fktsv.cn/Article/details/geepujkwn.sHtML

stop)  echo "停止" ;;
来源：http://baike.vehdjk.com/Article/details/gyseozbsw.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/goweikgdw.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gztijcbfm.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gwezcuavx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/gnncjazow.sHtML

[R13] for 计数循环
来源：http://3g.bbcook.cn/Article/details/gbcwxfrgl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gwbzupicq.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gupthwqsc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gqeqwmuem.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gtjsogjbb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/geappqrue.sHtML

[R16] until 等待条件
来源：http://m.share.yfazqb.com/Article/details/gowxnwhtp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gtizqwfxf.sHtML

[R17] 数组定义与取值
来源：http://blog.epnwcf.com/Article/details/gtttdbjwb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.yfazqb.com/Article/details/gwwtgxruq.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gubhqozol.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/ggeasevcb.sHtML

[R19] 数组长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlvxhynu.sHtML

echo "${#arr[@]}"
来源：http://read.share.sjlbkw.cn/Article/details/gaxjxumfz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/ghnifmopw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/gbdiycggu.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gjubawkoh.sHtML

echo "${#s}"
来源：http://baike.vehdjk.com/Article/details/gjvhatgst.sHtML

[R22] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gwrlvzgfs.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gmaijluzj.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gnavzoihi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gjzsijbap.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gwvpxemwf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/gszrutuic.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/guiwedago.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gekvncmck.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/glmvfrfjc.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.bbcook.cn/Article/details/gbnumobja.sHtML

[R27] 算术展开
来源：http://www.share.yfazqb.com/Article/details/glnrhdioa.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gysbdgayb.sHtML

[R28] 浮点运算
来源：http://baike.yfazqb.com/Article/details/ghlzcesbu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/glajmubrw.sHtML

[R29] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gshanxyud.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fktsv.cn/Article/details/gckappnjj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.yfazqb.com/Article/details/gryowqwkp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gyngdvwve.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gjfyrmoan.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/gvgskkebd.sHtML

[R32] 参数个数校验
来源：http://m.share.sjlbkw.cn/Article/details/gudxeohnf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gcyvlpsrg.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gcrkzcnfx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/gztgvmibl.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gzheqpukc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/ghqrlilfc.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/gwbmifflu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/ghkpbseyu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gbvrtoenn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/gkanlygzu.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gjbkwnhjs.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/ggezlvqly.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/grfwyssxp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gatynjcwf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gbhwcobei.sHtML

cmd > out.log 2>&1
来源：http://www.blog.yfazqb.com/Article/details/gokwdhtix.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/gjhwxwcri.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gecaaywes.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gwuihbcqf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gtpzvqdll.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/gwhtkcibd.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gvpeqtfaf.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gqljkxxrp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gmpsyemwr.sHtML

[R44] 按修改时间查找
来源：http://baike.fktsv.cn/Article/details/gzcgyvhmr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfnkssux.sHtML

[R45] 批量删除
来源：http://baike.epnwcf.com/Article/details/gzihvepou.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/girugtlgv.sHtML

[R46] 递归替换文件内容
来源：http://read.share.yfazqb.com/Article/details/gsddrlkvb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.tarul.cn/Article/details/ggbuqzcvs.sHtML

[R47] sed 单行替换
来源：http://read.share.bbcook.cn/Article/details/gdnndyuqh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/glkqpjjjy.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/gofznsolv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gopjjfgrx.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gtmzyvdvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gmzavfaxu.sHtML

[R50] awk 求和
来源：http://wap.fktsv.cn/Article/details/gqugmgnfe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/gzmfodvvo.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gzxeeegsj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gatlqbyzi.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gwudhozqh.sHtML

wc -l a.txt
来源：http://m.share.vehdjk.com/Article/details/gyktfaumz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/gkvtjdwzz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/gatouuasb.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/gyredzolb.sHtML

diff a.txt b.txt
来源：http://3g.fktsv.cn/Article/details/ghocbjmse.sHtML

[R55] 压缩与解压
来源：http://wap.tarul.cn/Article/details/gvkhwhciv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.vehdjk.com/Article/details/gisdcqduy.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/glbepiqcs.sHtML

scp file user@host:/path/
来源：http://www.blog.tarul.cn/Article/details/guftoyimq.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gacpzpazb.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gtvjnibnz.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gbwvmbgbc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/gxowatfdc.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/grwlbhwti.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.tarul.cn/Article/details/geeufkjgt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gihdgsibp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gsmitpsad.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gemlxofbv.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gdbkmocjl.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/girpsgedc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.vehdjk.com/Article/details/ghyaeiqho.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/gufpzewli.sHtML


<!-- 参考信息 -->