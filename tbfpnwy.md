代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://3g.tarul.cn/Article/details/gfefxxeiz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.vehdjk.com/Article/details/gzhqggqnl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.yfazqb.com/Article/details/galowymxo.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/glcxqmnbc.sHtML

SELECT * FROM users;
来源：http://mobile.epnwcf.com/Article/details/gvesztcgo.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gdgfycisr.sHtML

SELECT id, name FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gcvmwzdqv.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/grpciasbo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gkgsxtntk.sHtML

[Q18] 模糊匹配
来源：http://mobile.vehdjk.com/Article/details/gqkmjduer.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gxvntttnq.sHtML

[Q19] 范围查询
来源：http://baike.fktsv.cn/Article/details/gnpolssip.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/gdgqdhgiv.sHtML

[Q20] IN 列表
来源：http://www.blog.bbcook.cn/Article/details/glazpjggq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.bbcook.cn/Article/details/gnxqqoicm.sHtML

[Q21] 空值判断
来源：http://baike.bbcook.cn/Article/details/gyczxstiv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.epnwcf.com/Article/details/gbxtrcvva.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/ggjktiaha.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gwkotvefi.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/gvfhbbnzf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.vehdjk.com/Article/details/gcxmtqcab.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/gxjadnudz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.bbcook.cn/Article/details/gltbcmngh.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.tarul.cn/Article/details/gyxlnopri.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.tarul.cn/Article/details/gmonlwdug.sHtML

[Q26] 计数
来源：http://read.share.vehdjk.com/Article/details/gfbbswhqx.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fktsv.cn/Article/details/gujwvativ.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gcxykhqvs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.epnwcf.com/Article/details/gtrjfwknp.sHtML

[Q28] 求和与平均
来源：http://mobile.epnwcf.com/Article/details/gokbtecms.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gwsrsnzdq.sHtML

[Q29] 最大最小值
来源：http://wap.epnwcf.com/Article/details/gxkxvxmrs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.vehdjk.com/Article/details/gtrkuzjdv.sHtML

[Q30] 分组统计
来源：http://blog.fktsv.cn/Article/details/gkamexiph.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gbuutdglb.sHtML

[Q31] 分组后过滤
来源：http://blog.epnwcf.com/Article/details/gjbhyztnl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/gapuzyiwh.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/ggwnrrwac.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gfanavtlt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.sjlbkw.cn/Article/details/gbkxumjfn.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gcubqpcdr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/gwcyuyanv.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/gsbmpfroy.sHtML

SELECT * FROM (
来源：http://www.share.tarul.cn/Article/details/gfctbpeyx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/guomqmnwk.sHtML

) t WHERE rn = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gfwkdjzcq.sHtML

[Q35] 内连接
来源：http://mobile.epnwcf.com/Article/details/getsbvxub.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gzdksmanz.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/gxvvgsius.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gfjrvxnyf.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gygqnhtri.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/gfmxaovch.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gscphweyt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.vehdjk.com/Article/details/gfmdhwycz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fktsv.cn/Article/details/gicbjkuhi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.tarul.cn/Article/details/gkcwlnmma.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.vehdjk.com/Article/details/gjwpqodts.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fktsv.cn/Article/details/grnyahltk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gmmixoftc.sHtML

[Q41] 多表连接
来源：http://m.share.yfazqb.com/Article/details/glfrczvgr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.sjlbkw.cn/Article/details/glkoegwjz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.bbcook.cn/Article/details/gnnfyrrud.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gdfwcrxyg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gcwossqdt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.yfazqb.com/Article/details/gegydmjvc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gvofwcbhh.sHtML

[Q43] 标量子查询
来源：http://mobile.fktsv.cn/Article/details/gdfiovqnn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.bbcook.cn/Article/details/gikfxherm.sHtML

[Q44] IN 子查询
来源：http://wap.yfazqb.com/Article/details/goekxctad.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/grhobuilz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.vehdjk.com/Article/details/gywwrgnii.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gxksmoywe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.yfazqb.com/Article/details/ghahjemik.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gpibykddi.sHtML

[Q47] 与平均值比较
来源：http://read.share.tarul.cn/Article/details/ggfxohjrm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/guxnuaodr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.epnwcf.com/Article/details/gktfzqmzw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gkrfteraq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gzqmvrzma.sHtML

[Q49] 更新单行
来源：http://blog.fktsv.cn/Article/details/gurqjmwei.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gjajbnupg.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gpzrqcmlw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.tarul.cn/Article/details/ghouewzyu.sHtML

[Q51] 用子查询更新
来源：http://mobile.tarul.cn/Article/details/gxwjwyxns.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gvxsfrgqt.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gemxgsxok.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gawsxcpnz.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/gbujpcplk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gqyahbrdd.sHtML

[Q54] 清空表
来源：http://read.share.fktsv.cn/Article/details/gohwjqoqj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdsgjnxk.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/gvbgxoyrx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gsnakdqsq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/grbwsgbkt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.bbcook.cn/Article/details/gqcugrmzs.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/gmyvavteo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/grmnhhkta.sHtML

[Q58] 累计求和
来源：http://m.share.tarul.cn/Article/details/gxrwndhfk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/geusgtexj.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gckmnwqxd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/grfdiqind.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.tarul.cn/Article/details/gohlzlqoi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.yfazqb.com/Article/details/gfwipvlpa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gqgzbjihr.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/gpgoksosi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gelfqnrmi.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gjshyvqkb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/ggtllucdd.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gidvpkysk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gobdtchsw.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gyhoznmnn.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/gnaqusrjh.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gdoqqvswv.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gpnejxilp.sHtML

[Q66] 行锁查询
来源：http://m.share.yfazqb.com/Article/details/gtnbkcmds.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gnucdshdl.sHtML

[Q67] 设置隔离级别
来源：http://www.share.epnwcf.com/Article/details/gvpnrlcnk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gnucasgin.sHtML

[Q68] 保存点
来源：http://m.share.bbcook.cn/Article/details/gpydnodos.sHtML

SAVEPOINT sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gcmgerqjy.sHtML

ROLLBACK TO sp1;
来源：http://3g.bbcook.cn/Article/details/gyplcarju.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gipwtjovq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/ggzemjfzb.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/gmazcejwl.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gflrqnvge.sHtML

[Q71] 查看建表语句
来源：http://www.blog.yfazqb.com/Article/details/gcojuqjij.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gpndqpran.sHtML

[Q72] 查看索引
来源：http://blog.epnwcf.com/Article/details/gteethmos.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gpsxipqvy.sHtML

[Q73] 查看表状态
来源：http://m.share.fktsv.cn/Article/details/gelypmzbh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gzkiholjs.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gpklafwgs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fktsv.cn/Article/details/gpltbfjqo.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gjfguotyc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gzklebpxi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/gsfgscoqy.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gbdofqbeu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gmjnvznmn.sHtML

[Q77] 时间加减
来源：http://blog.yfazqb.com/Article/details/gnkkqfgho.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.bbcook.cn/Article/details/gjwxoemcb.sHtML

[Q78] 当前时间
来源：http://mobile.yfazqb.com/Article/details/gsvxftuup.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/ghyyourlo.sHtML

[Q79] 字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gjgfbyqif.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.vehdjk.com/Article/details/guywdnzhu.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/gxrcvtztx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gwtfwkvrs.sHtML

[Q81] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gndquocvr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gjeluhltf.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.sjlbkw.cn/Article/details/gbcwnqrtd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/grrjdtkmp.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gditkzwax.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpfseuvih.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/glztgskcr.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gntlkjofc.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gcivzdqjx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/gcihbjagi.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gptmlxlvw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/ggpfadebp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/ghqypwges.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gidtcnctb.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gnglppjrs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.bbcook.cn/Article/details/gbgftzidz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gircjenqd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gktnolvrp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.bbcook.cn/Article/details/gjjneyxkh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gacdijiyz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/glnvaybty.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpmcfdxby.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gweeopvry.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtjhnrlhq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.bbcook.cn/Article/details/grxigjdgl.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fktsv.cn/Article/details/ghzzmwycy.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gvtqvbsvp.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gvoriqnek.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.sjlbkw.cn/Article/details/ggbmmyqua.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/guphzknrh.sHtML

readonly PI=3.14
来源：http://wap.yfazqb.com/Article/details/gpkkkgogb.sHtML

[R04] 位置参数
来源：http://3g.fktsv.cn/Article/details/gxvurcehz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/giwrjxqjc.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gxygzrrla.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gjptenprn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/gdoffysdm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/ghllzgvml.sHtML

[R07] if 判断文件
来源：http://www.m.share.bbcook.cn/Article/details/gwmnthdbz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gpzxjsxel.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gcvonofyq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.yfazqb.com/Article/details/gsntcdepk.sHtML

[R09] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gnycuybrr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gntlthott.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/gvgkmjyhe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/gcvzxhfoi.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gvkvqqwgy.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gukjoheyz.sHtML

start) echo "启动" ;;
来源：http://m.share.bbcook.cn/Article/details/gklfxfgqz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gpqmdqpyx.sHtML

*)     echo "未知命令" ;;
来源：http://baike.vehdjk.com/Article/details/gczkmlgzm.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/ghpknpqsu.sHtML

[R12] for 遍历文件
来源：http://read.share.epnwcf.com/Article/details/gyyankkqh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gsunvytif.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gstgulshd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/geiwbczwa.sHtML

[R14] C 风格 for
来源：http://m.share.vehdjk.com/Article/details/gkrzbnwnd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/giymvzqjs.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gyjsrgweb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/gxvnvuwbf.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/grglodovl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gxpjzyafn.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gzcsqobgd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gohuxghki.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gflkfotrp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gpkjacmrs.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gwdgagouy.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/gewepygob.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gvrzobpgy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/gphzizmvm.sHtML

[R21] 字符串长度
来源：http://3g.bbcook.cn/Article/details/gefedfdcm.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gdtfqmtmt.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gmtdpdwmc.sHtML

echo "${s:0:5}"
来源：http://wap.vehdjk.com/Article/details/ghwmlowbb.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gqhpjmmoa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.epnwcf.com/Article/details/gfxycccld.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/grkbeyuou.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.bbcook.cn/Article/details/ganennpcc.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.epnwcf.com/Article/details/glxaeryue.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/gexgpemet.sHtML

[R26] 命令替换
来源：http://mobile.bbcook.cn/Article/details/gxnboqldc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gwjdwhsez.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gsiwhehxt.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gdphtugsh.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/glmtacluk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gfvuaoicm.sHtML

[R29] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gfuoyokef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/ggaiamuyj.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gjmskncmb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gxblixrtj.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gvhevuljz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/gdwejxiwp.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/gdbxwsujv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gomfybkhg.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gywzbhaqx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/grhhxopxd.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gylurhnmn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gaxtverau.sHtML

[R35] 后台执行并等待
来源：http://www.blog.vehdjk.com/Article/details/gmozsjrky.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.yfazqb.com/Article/details/gfbkgkrfl.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/gixcjtgti.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gvpsqeiis.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gbcgtzqgn.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gvblgidns.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/gghbsoeoa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fktsv.cn/Article/details/gawfguzqq.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gqixwsnfk.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gvvisvfmj.sHtML

[R40] 追加写日志
来源：http://www.blog.bbcook.cn/Article/details/gpkhqokmw.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/glwigoxyc.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gqkapmhnl.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gudssgstu.sHtML

[R42] 输入重定向
来源：http://wap.tarul.cn/Article/details/gojixkvse.sHtML

wc -l < a.txt
来源：http://blog.bbcook.cn/Article/details/gacqrypxf.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gsylthlpp.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/gptoulfej.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/grfqvhuze.sHtML

find . -mtime -7 -type f
来源：http://www.share.fktsv.cn/Article/details/ggqcaxvpl.sHtML

[R45] 批量删除
来源：http://m.share.sjlbkw.cn/Article/details/gzyduecee.sHtML

find . -name "*.tmp" -delete
来源：http://blog.bbcook.cn/Article/details/gyohekmcf.sHtML

[R46] 递归替换文件内容
来源：http://blog.fktsv.cn/Article/details/gkoevyevr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.sjlbkw.cn/Article/details/gakqvnfku.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/grvwxanwz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gtttfrxja.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gnvanficp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gdlpkprza.sHtML

[R49] awk 带条件
来源：http://www.share.tarul.cn/Article/details/gwghfjhrl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/gcalgsumb.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/gsdthenyx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gywbwauqe.sHtML

[R51] 排序去重取前几
来源：http://mobile.epnwcf.com/Article/details/ghnrjayob.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.bbcook.cn/Article/details/gfsqvgxjd.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/ggbtmiwzb.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gpngzeyhi.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.sjlbkw.cn/Article/details/gjjgwzswp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.tarul.cn/Article/details/gzfjznvzg.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/grrqakumy.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/gbuoonukc.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/gnxkbiqbe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.yfazqb.com/Article/details/gadnpkhir.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gxbayfupb.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/gnqfvbfll.sHtML

[R57] 远程执行命令
来源：http://3g.sjlbkw.cn/Article/details/geirtgqsv.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gojvtraaq.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gptjchnes.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.tarul.cn/Article/details/glsngmzmh.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/gmydwpfdk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fktsv.cn/Article/details/gutfkahom.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gnufjcgda.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.sjlbkw.cn/Article/details/gpbjkbnry.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gohthdmob.sHtML

df -h;  du -sh *
来源：http://baike.fktsv.cn/Article/details/gbcoqbael.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gkdfawoqj.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/guvoulhzh.sHtML

[R63] 内存与进程
来源：http://baike.vehdjk.com/Article/details/gedpffyag.sHtML


<!-- 参考信息 -->