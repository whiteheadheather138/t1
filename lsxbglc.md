代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/gazbnwtfx.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gzcnnuank.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gpdlpzhwz.sHtML

[Q19] 范围查询
来源：http://mobile.vehdjk.com/Article/details/gfsbxumxj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.tarul.cn/Article/details/gbavetcgw.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/gcmwfcfrr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gtwvzueuy.sHtML

[Q21] 空值判断
来源：http://baike.epnwcf.com/Article/details/gwbovtqck.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gujslpewo.sHtML

[Q22] 排序
来源：http://3g.tarul.cn/Article/details/gumuxcfot.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.vehdjk.com/Article/details/gqdnedhls.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gtubvvfqn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/gjwmncjsg.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gvfdsejmk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/gitjfvuqb.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/gopzkjhud.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gosobsjpr.sHtML

[Q26] 计数
来源：http://m.share.bbcook.cn/Article/details/goujgewvb.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gbsfzxbnh.sHtML

[Q27] 条件计数
来源：http://baike.sjlbkw.cn/Article/details/gkysscghh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gyzyzqjpy.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gzktgvwpz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.tarul.cn/Article/details/gmydnptyn.sHtML

[Q29] 最大最小值
来源：http://3g.fktsv.cn/Article/details/gjrqankll.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.yfazqb.com/Article/details/grueiqtah.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/gtwslzqeq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gtlghhjzp.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/gsxipkabr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fktsv.cn/Article/details/gaexmrqtr.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gbxdsfgyo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gpwjjsgtw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/gftblgjet.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/gckuxoazy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.vehdjk.com/Article/details/gaortziuc.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/gwkwfqpay.sHtML

SELECT * FROM (
来源：http://mobile.tarul.cn/Article/details/ghahrpgnx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/gxytxrndq.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/gejjjkvis.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gwomoniif.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gelbwwtbo.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/gqoocagmd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/glktyuhth.sHtML

[Q37] 右连接
来源：http://3g.yfazqb.com/Article/details/germewpyr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gdfztfffa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.vehdjk.com/Article/details/gvhgxkrpp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.epnwcf.com/Article/details/golrgbpzo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.epnwcf.com/Article/details/ggjsqksxo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.bbcook.cn/Article/details/grkbyhtto.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fktsv.cn/Article/details/gimdjrzgi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gphwudfim.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gwolkuelz.sHtML

[Q41] 多表连接
来源：http://mobile.yfazqb.com/Article/details/gojtojpbo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gakwjosgw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.vehdjk.com/Article/details/gorcoiupf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gjaezhlrr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.yfazqb.com/Article/details/ghlofgrqp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.yfazqb.com/Article/details/gceybovyb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/gzhsrjsgs.sHtML

[Q43] 标量子查询
来源：http://baike.yfazqb.com/Article/details/gjkjkbqiu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gtrxycjhi.sHtML

[Q44] IN 子查询
来源：http://baike.tarul.cn/Article/details/gusmcdtfa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.tarul.cn/Article/details/gpzfitsrh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.yfazqb.com/Article/details/ggwqhycbq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gdpgrakbe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gxtbyscvi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/givmatkzz.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/gbcpkklht.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.epnwcf.com/Article/details/gsosmzxkm.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gfcjacvlt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.epnwcf.com/Article/details/gromqhcsr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.vehdjk.com/Article/details/ggazevuxm.sHtML

[Q49] 更新单行
来源：http://baike.fktsv.cn/Article/details/ggxizkzkn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gedtopnye.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gwonchrmp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/gvqveqwbh.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gofwyvjzi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.bbcook.cn/Article/details/gyeanyjpx.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/glrjacivl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gbggfgdkm.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/ghfvagani.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/gumgfxuza.sHtML

[Q54] 清空表
来源：http://www.m.share.tarul.cn/Article/details/gxqyyhckj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gkkzcdibe.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gypbvonim.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gopngftag.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.yfazqb.com/Article/details/gursvahhd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/geeccndsa.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/grqtnmkij.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdkxwgejx.sHtML

[Q58] 累计求和
来源：http://read.share.vehdjk.com/Article/details/gerjupqzv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/ggkccspeo.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/gcjlzxady.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gnkrkdptv.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/grdltddhx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.bbcook.cn/Article/details/gurmanivk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gcpjjrezo.sHtML

[Q61] 移动平均
来源：http://3g.tarul.cn/Article/details/gjpellyfn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gogrxcqgu.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/gfpwgrllz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gbeyxtynm.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/griqjokvh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/geirvmhkd.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/gvpqwrzfo.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/gghwnqdcv.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/gfwcvfcxb.sHtML

ROLLBACK;
来源：http://blog.epnwcf.com/Article/details/gabzjeral.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/gpgfkqtms.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gdlxsccjg.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gzmbcrumn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.sjlbkw.cn/Article/details/glskhnmmp.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/geuzbxhel.sHtML

SAVEPOINT sp1;
来源：http://m.share.epnwcf.com/Article/details/gsjuyimvh.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gzjwoxjom.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gttpcweyv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.yfazqb.com/Article/details/gftzahovu.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.epnwcf.com/Article/details/gddixdlkj.sHtML

ANALYZE TABLE users;
来源：http://www.share.fktsv.cn/Article/details/gznbwbezt.sHtML

[Q71] 查看建表语句
来源：http://baike.sjlbkw.cn/Article/details/gfalhxgya.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/ggnqdfasm.sHtML

[Q72] 查看索引
来源：http://3g.sjlbkw.cn/Article/details/gndilxmor.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/ghrsvrfad.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gugrgyxim.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gnqiopjol.sHtML

[Q74] 强制使用索引
来源：http://www.blog.sjlbkw.cn/Article/details/gcisuaevy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.tarul.cn/Article/details/gmqhqnatf.sHtML

[Q75] 日期格式化
来源：http://blog.fktsv.cn/Article/details/ghofozmtu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.vehdjk.com/Article/details/gisqolivu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.tarul.cn/Article/details/gbaqvcpxc.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gbqymhupe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/glyicrzcd.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gzafleudv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.epnwcf.com/Article/details/gehbdgqqs.sHtML

[Q78] 当前时间
来源：http://wap.bbcook.cn/Article/details/gulnhltkx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.sjlbkw.cn/Article/details/golgowfra.sHtML

[Q79] 字符串拼接
来源：http://baike.fktsv.cn/Article/details/gmpwmacwy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/gjcrnwvgs.sHtML

[Q80] 字符串截取
来源：http://www.share.bbcook.cn/Article/details/gswgovwqr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.tarul.cn/Article/details/gtpihshqq.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gqtnzhqpo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gopvqzdkp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fktsv.cn/Article/details/gmrktxfgt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gfphrjcaw.sHtML

[Q83] 大小写转换
来源：http://m.share.tarul.cn/Article/details/ghsymtlsh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gzojrsocx.sHtML

[Q84] 去除首尾空格
来源：http://wap.bbcook.cn/Article/details/gabpdcluw.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gmigubihg.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gyghgjmlm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/giicelgry.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.yfazqb.com/Article/details/gzqelimrk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gpiivxgjd.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/gkbxawjah.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fktsv.cn/Article/details/gakbvjdut.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.yfazqb.com/Article/details/gxtqwniwi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.epnwcf.com/Article/details/gsgyfcygi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.bbcook.cn/Article/details/gbshvsdtm.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gpnuyvopz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.vehdjk.com/Article/details/gkuwyjqqd.sHtML

[Q90] 生成序号列
来源：http://blog.fktsv.cn/Article/details/gnonkalur.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.vehdjk.com/Article/details/ghcrsesbd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpcvgivgm.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/gxyayxwrs.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gonbyfqyj.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gubfzjyae.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gemxmxyiy.sHtML

set -euo pipefail
来源：http://www.m.share.yfazqb.com/Article/details/gsfmsytjh.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/gyavyhmfr.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gcfvmgsys.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/gseunixld.sHtML

readonly PI=3.14
来源：http://blog.bbcook.cn/Article/details/gdndeojzh.sHtML

[R04] 位置参数
来源：http://m.share.tarul.cn/Article/details/gvgeggzyj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gjwxpxljj.sHtML

[R05] 参数默认值
来源：http://wap.tarul.cn/Article/details/gzxzjehlr.sHtML

name="${1:-default}"
来源：http://blog.epnwcf.com/Article/details/gqryyqish.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gfpamnsdr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gwwwmuaoz.sHtML

[R07] if 判断文件
来源：http://read.share.fktsv.cn/Article/details/gxxzbgtzm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gjcsqyivi.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gzuwjynum.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gqorshqhj.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gkeyydgvp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.vehdjk.com/Article/details/grdzbftqf.sHtML

[R10] 正则匹配
来源：http://baike.bbcook.cn/Article/details/gxpiahung.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.tarul.cn/Article/details/gegjddzwv.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/gcwjdaxcx.sHtML

case "$1" in
来源：http://read.share.bbcook.cn/Article/details/gkhrzvvtq.sHtML

start) echo "启动" ;;
来源：http://www.share.epnwcf.com/Article/details/gzlpojbei.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gihxdrgiu.sHtML

*)     echo "未知命令" ;;
来源：http://3g.yfazqb.com/Article/details/gjekkelex.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gmbgnzxyi.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gjwcambbz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.vehdjk.com/Article/details/gpqsghtka.sHtML

[R13] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gimzskvix.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gllczeexr.sHtML

[R14] C 风格 for
来源：http://m.share.fktsv.cn/Article/details/gweestjik.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gbvmaagdv.sHtML

[R15] while 逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gkwmvrtaj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/gzwfwiljy.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gtdpbydjf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gbbxhfboy.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gpcqrqxtm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.vehdjk.com/Article/details/gcgxwdumi.sHtML

[R18] 遍历数组
来源：http://www.blog.sjlbkw.cn/Article/details/gkoypncml.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/gjtrotdqe.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gphibhthd.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/ggevorngp.sHtML

[R20] 关联数组（字典）
来源：http://blog.bbcook.cn/Article/details/gvgyudnyu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gxfpopgig.sHtML

[R21] 字符串长度
来源：http://m.share.fktsv.cn/Article/details/gbszvksef.sHtML

echo "${#s}"
来源：http://wap.yfazqb.com/Article/details/gvrmayaor.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gkvujwiuk.sHtML

echo "${s:0:5}"
来源：http://wap.epnwcf.com/Article/details/gljmqpxzb.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gkjznjsfl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gvpgpviim.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gqlgqkebi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.yfazqb.com/Article/details/gfiyxqbwy.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.tarul.cn/Article/details/gghediogi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gmvbvifgc.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/gyahejmst.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.yfazqb.com/Article/details/gwrowaion.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/gnwssakti.sHtML

echo $((1 + 2 * 3))
来源：http://blog.sjlbkw.cn/Article/details/gwoagaobw.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gcyoqaquu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gmlpajkuq.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/garzchgud.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fktsv.cn/Article/details/gdxguqfta.sHtML

[R30] 函数返回状态码
来源：http://www.share.sjlbkw.cn/Article/details/gphaiazvd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gfxcdirap.sHtML

[R31] 局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gszxuckxx.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gfbwbqkad.sHtML

[R32] 参数个数校验
来源：http://www.share.epnwcf.com/Article/details/gwvsgmjls.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/ggzfrcdwv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.yfazqb.com/Article/details/gchsosdxc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.vehdjk.com/Article/details/gcoyhatiz.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gzslbovjh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gmhdrrrbm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/gvqijolwc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fktsv.cn/Article/details/gkjyhvbrk.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gkordzobe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fktsv.cn/Article/details/gbgmwwgop.sHtML

[R37] 把输出赋给变量
来源：http://read.share.bbcook.cn/Article/details/guswyvtyo.sHtML

files=$(ls -1)
来源：http://3g.vehdjk.com/Article/details/grvfbtaxn.sHtML

[R38] 管道串联
来源：http://www.m.share.bbcook.cn/Article/details/gludvphat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.epnwcf.com/Article/details/genhpiwyb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.bbcook.cn/Article/details/gdegnzmwd.sHtML

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/gcbtgggsm.sHtML

[R40] 追加写日志
来源：http://m.share.epnwcf.com/Article/details/ghaqldwzp.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gtyhrjjke.sHtML

[R41] 丢弃输出
来源：http://www.m.share.vehdjk.com/Article/details/gseuwkoyd.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gqkcfmpoa.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gcuvjryvk.sHtML

wc -l < a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gqmnozodz.sHtML

[R43] 按名字查找文件
来源：http://wap.bbcook.cn/Article/details/gheytvirn.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/goonwpzsb.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/grknzbfaz.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/grtoewrma.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/gibgpyiic.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gxkzjmyou.sHtML

[R46] 递归替换文件内容
来源：http://mobile.epnwcf.com/Article/details/gkfiozyhh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fktsv.cn/Article/details/gabygkcgn.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gcmbquumq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gaoifbdbp.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gjuummifo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gszoedwvv.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gbecqanjm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.tarul.cn/Article/details/glrimiqyi.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gmcnmviqj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gfztztlmw.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/geujkousb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fktsv.cn/Article/details/gykbgtuom.sHtML

[R52] 统计行数
来源：http://www.m.share.epnwcf.com/Article/details/gyaqvafeb.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gnejqztxe.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/ggnuogzhg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.bbcook.cn/Article/details/grfqgylon.sHtML

[R54] 比较两个文件
来源：http://baike.sjlbkw.cn/Article/details/gqtelovnn.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gqaasmdoc.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gcoykcfna.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gonfkddpb.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/ghuowprpr.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gdmcqqkba.sHtML

[R57] 远程执行命令
来源：http://baike.bbcook.cn/Article/details/gzzgtgpig.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/gnuygrlug.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gqlbwquff.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.yfazqb.com/Article/details/gbmskfzso.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gtoqfxrmg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/geemkvtse.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gmxlxwntz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gvlctdhun.sHtML

[R61] 磁盘占用
来源：http://www.share.vehdjk.com/Article/details/guvtflwbv.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gecipdzxo.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gtggszetj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gbmycmtdc.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/gucpkuuid.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/gyzvhmasv.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gtldmefjb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gxbudbjaq.sHtML

[R65] 查看端口占用
来源：http://m.share.vehdjk.com/Article/details/gtcogvhab.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/goiirnjrm.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/gzjedzahe.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.bbcook.cn/Article/details/gcggwiewu.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.epnwcf.com/Article/details/gznjdxdcn.sHtML


<!-- 参考信息 -->