代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/gaxltkvkw.sHtML

[Q18] 模糊匹配
来源：http://www.blog.tarul.cn/Article/details/gpupcrosz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.tarul.cn/Article/details/gaidjwylq.sHtML

[Q19] 范围查询
来源：http://www.blog.sjlbkw.cn/Article/details/gyzggieyo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/gpjfngbff.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gyqluwuqp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gewyrefrq.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/grdekocyd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gomjgygmk.sHtML

[Q22] 排序
来源：http://read.share.yfazqb.com/Article/details/geuqxsshi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.bbcook.cn/Article/details/gkvpyakwc.sHtML

[Q23] 分页
来源：http://www.m.share.vehdjk.com/Article/details/gbkdirsbt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.epnwcf.com/Article/details/gadzdlxwo.sHtML

[Q24] 去重
来源：http://blog.sjlbkw.cn/Article/details/ggpmdbwom.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.epnwcf.com/Article/details/gsrszhxnl.sHtML

[Q25] 只取前 N 条
来源：http://m.share.yfazqb.com/Article/details/grziqiode.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/gkuyplwia.sHtML

[Q26] 计数
来源：http://www.m.share.epnwcf.com/Article/details/gzoyudeiz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.bbcook.cn/Article/details/gjmcvpzfp.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gszyqaerl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.vehdjk.com/Article/details/gvumfguaw.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/gpowdwpyv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gljxapaqy.sHtML

[Q29] 最大最小值
来源：http://3g.sjlbkw.cn/Article/details/ghpqnlwiv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/gsaywlkho.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/gdyxqhzlx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gueqbbyho.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/guetjhggy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/ggjgdtzyj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/glkpshpda.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gncqgnctf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gnsxfplvs.sHtML

[Q33] 多列分组
来源：http://read.share.sjlbkw.cn/Article/details/gkxsrdsfu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/gjazhhwxr.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fktsv.cn/Article/details/gudklfvmo.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/gkaxtrxiu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gugiqidqb.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/gznzcxfev.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/gdudawach.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gazuwjrsx.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gqcluvoaw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gtzsedfgv.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gklmhdsnu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.epnwcf.com/Article/details/gjsbsteve.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gvomlbahl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.yfazqb.com/Article/details/guhbgyrrw.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gyuughosd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.epnwcf.com/Article/details/gvjhykhhz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/grbjfjulx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gpzutjplb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gdopnrtls.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/gplnvrtwp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.vehdjk.com/Article/details/gnscxbhnq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.bbcook.cn/Article/details/gweszljdg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/gegfcwtwm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjekwaxk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/ggeqwoodz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.bbcook.cn/Article/details/gtlqstnfq.sHtML

[Q43] 标量子查询
来源：http://wap.yfazqb.com/Article/details/gzmmftcrt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/gmvjtegtv.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gofrfjphx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.sjlbkw.cn/Article/details/gidbknfte.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gyjkhkiwz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gghmtawmn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.yfazqb.com/Article/details/gqszcpyow.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gmjxioyer.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gorhsrbcv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/gxtcjsapf.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/grpaawmfe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/goixuefus.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gtjxrwtkw.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/gqbefqvzy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gcwblyhqx.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/ggwwdkwzv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gggvrntlq.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/gsmszkhpd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fktsv.cn/Article/details/gkirayhan.sHtML

[Q52] 删除指定行
来源：http://mobile.epnwcf.com/Article/details/gxtmyrjdy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gredcvowy.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/giiwdlayd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.bbcook.cn/Article/details/gpgxoknxa.sHtML

[Q54] 清空表
来源：http://read.share.tarul.cn/Article/details/gzuotvjto.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/gpahrjkwk.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fktsv.cn/Article/details/gevmdimid.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/ghxrknxzf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gjebslnld.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.bbcook.cn/Article/details/grwtqeety.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gpolmsmky.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gidmhpjoc.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/gchqzjjub.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gibraxcag.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/gxqfqrzqs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gixnjxpax.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/gvnkkcuab.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fktsv.cn/Article/details/geueuyzos.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/geeqnqjge.sHtML

[Q61] 移动平均
来源：http://3g.yfazqb.com/Article/details/grgefzdqe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gcxjglhsw.sHtML

[Q62] 分组占比
来源：http://www.blog.yfazqb.com/Article/details/gxijdxjmf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gsfyaorqm.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gycsulqkp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.epnwcf.com/Article/details/gtsfdmndr.sHtML

[Q64] 提交事务
来源：http://m.share.yfazqb.com/Article/details/gbfxwlnar.sHtML

COMMIT;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaansdbmh.sHtML

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/gxbwmetvx.sHtML

ROLLBACK;
来源：http://blog.fktsv.cn/Article/details/gzoqayjjz.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gqzeulfgf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fktsv.cn/Article/details/gzhetmqqo.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.yfazqb.com/Article/details/guiybvmjh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.bbcook.cn/Article/details/gzbubfhbu.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gvjsriivn.sHtML

SAVEPOINT sp1;
来源：http://mobile.epnwcf.com/Article/details/gnpmtvwfq.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gdiqsrgzo.sHtML

[Q69] 查看执行计划
来源：http://m.share.fktsv.cn/Article/details/gwtphderk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fktsv.cn/Article/details/gbgcnfxym.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/gndhhpysr.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/gkpmyueia.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/ganraupan.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gmmjvwfup.sHtML

[Q72] 查看索引
来源：http://3g.sjlbkw.cn/Article/details/gdkqsnrwj.sHtML

SHOW INDEX FROM users;
来源：http://baike.epnwcf.com/Article/details/gqkpwdups.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gwafiebkj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.epnwcf.com/Article/details/gbubsxlkx.sHtML

[Q74] 强制使用索引
来源：http://mobile.fktsv.cn/Article/details/goewyibgv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/gojqglalj.sHtML

[Q75] 日期格式化
来源：http://wap.vehdjk.com/Article/details/goahsijcr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gcpneswpv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gqrshkmsj.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gdnwfqukt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.yfazqb.com/Article/details/geehaqdwg.sHtML

[Q77] 时间加减
来源：http://baike.yfazqb.com/Article/details/gfcgxcnrh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.tarul.cn/Article/details/gegvhscdu.sHtML

[Q78] 当前时间
来源：http://mobile.fktsv.cn/Article/details/gvxahwqsp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gsnohrvjw.sHtML

[Q79] 字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gijfcuomp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gwefmvyma.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gjlfssboj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/gtsphhkvw.sHtML

[Q81] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gvahpdufh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/guylvmrzo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gbxhjiidd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/glheuzghv.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gojeqhsos.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.tarul.cn/Article/details/ghayeekxv.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fktsv.cn/Article/details/glffuxkru.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/ghmipwqwe.sHtML

[Q85] 数值取整
来源：http://read.share.tarul.cn/Article/details/glazrvlsz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/gvmrybkug.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gnqdbnszv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gjpdhneim.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fktsv.cn/Article/details/ggiwkzdsm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.vehdjk.com/Article/details/gulmpdzfd.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.yfazqb.com/Article/details/gixarkaqp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gpgfndmrv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gzckunsrh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.yfazqb.com/Article/details/gfojadsty.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fktsv.cn/Article/details/gstvtdraq.sHtML

[Q90] 生成序号列
来源：http://3g.sjlbkw.cn/Article/details/gllynnwcu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.vehdjk.com/Article/details/gfbfljkrb.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwyqxbnar.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/gafjhywnh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gglxewtok.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/ggwjgcyzl.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/ghvptmkfh.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gzfslnyqz.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gxodootyc.sHtML

name="Tom"; echo "$name"
来源：http://m.share.yfazqb.com/Article/details/gysyyrcca.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/geqqnxcym.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/gtowvyexo.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/ggfeldvut.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.sjlbkw.cn/Article/details/gqidkctdk.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/gwggwgaja.sHtML

name="${1:-default}"
来源：http://www.blog.bbcook.cn/Article/details/gmxxtobpq.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gncdqvuem.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gxjytjobq.sHtML

[R07] if 判断文件
来源：http://3g.epnwcf.com/Article/details/gtubzqdnj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/grtputtwe.sHtML

[R08] 数值比较
来源：http://wap.vehdjk.com/Article/details/gwlnycbug.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.bbcook.cn/Article/details/gfcfjcwgk.sHtML

[R09] 字符串比较
来源：http://wap.tarul.cn/Article/details/giisiburz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/gixllikxy.sHtML

[R10] 正则匹配
来源：http://3g.epnwcf.com/Article/details/gtlqhkksi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/grkaniniv.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/govdlgdtp.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/grcbfuoaw.sHtML

start) echo "启动" ;;
来源：http://wap.tarul.cn/Article/details/gkkbpjimt.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gkoponhso.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.tarul.cn/Article/details/guabvfuld.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gbndcbqta.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/ggsyghlcx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.epnwcf.com/Article/details/gnvgciiqs.sHtML

[R13] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/ghspdvayh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/grpxxkcsp.sHtML

[R14] C 风格 for
来源：http://m.share.vehdjk.com/Article/details/gcrfwxkan.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gehwhrwhr.sHtML

[R15] while 逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gtqyexfcw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/gnagtrgka.sHtML

[R16] until 等待条件
来源：http://www.share.epnwcf.com/Article/details/gcudorgzz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/giwklkzws.sHtML

[R17] 数组定义与取值
来源：http://wap.fktsv.cn/Article/details/gjlorgbyd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fktsv.cn/Article/details/gywlwfqlv.sHtML

[R18] 遍历数组
来源：http://www.blog.vehdjk.com/Article/details/gueefunhi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.vehdjk.com/Article/details/gbulriqdi.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/gxuahtnvo.sHtML

echo "${#arr[@]}"
来源：http://mobile.vehdjk.com/Article/details/guejgwiax.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/gztcaihsw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.epnwcf.com/Article/details/gacawmukb.sHtML

[R21] 字符串长度
来源：http://blog.tarul.cn/Article/details/gblvxwqml.sHtML

echo "${#s}"
来源：http://www.share.vehdjk.com/Article/details/grvszysth.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/goglnrvem.sHtML

echo "${s:0:5}"
来源：http://www.share.bbcook.cn/Article/details/gddrxfmwl.sHtML

[R23] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gjbzcyqry.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/gpenwrafw.sHtML

[R24] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gzkjkilgm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.bbcook.cn/Article/details/glzjrpvgw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/gcecswnpy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.epnwcf.com/Article/details/guqtfutgf.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gayvzeedi.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.epnwcf.com/Article/details/gsufdbrfe.sHtML

[R27] 算术展开
来源：http://blog.vehdjk.com/Article/details/gftldxgzd.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.tarul.cn/Article/details/gaqtkaomb.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gpejbxive.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.bbcook.cn/Article/details/grcdctmxn.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/ggytokkgk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gvqtodkun.sHtML

[R30] 函数返回状态码
来源：http://3g.sjlbkw.cn/Article/details/gqfihabar.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.sjlbkw.cn/Article/details/gvqnrdxsj.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/gcarzvchu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.yfazqb.com/Article/details/gxujybtmz.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/glusutsvn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gbtupioer.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.sjlbkw.cn/Article/details/gxakpfgck.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gygfahchz.sHtML

[R34] 退出时清理
来源：http://blog.sjlbkw.cn/Article/details/gfglanwbn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gqttxenny.sHtML

[R35] 后台执行并等待
来源：http://blog.sjlbkw.cn/Article/details/gnvdjzmdq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.tarul.cn/Article/details/gmabivzxs.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gltgfpnmd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gsrqqgfoa.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gvwkipfmd.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/gnbkezjnx.sHtML

[R38] 管道串联
来源：http://www.share.vehdjk.com/Article/details/gdplhpgqc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/gaxxuvcnm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gzbblwtok.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gsqtjajdn.sHtML

[R40] 追加写日志
来源：http://wap.sjlbkw.cn/Article/details/gdrjgbrjq.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gjygdcrsc.sHtML

[R41] 丢弃输出
来源：http://www.share.sjlbkw.cn/Article/details/ggkejhrmj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/geyrrewmd.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gdahewtso.sHtML

wc -l < a.txt
来源：http://m.share.tarul.cn/Article/details/gzyizkkqh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gteeytaex.sHtML

find . -name "*.log" -type f
来源：http://www.blog.tarul.cn/Article/details/gcmbqwrvw.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gwkkzxijj.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/gaezjvfzd.sHtML

[R45] 批量删除
来源：http://read.share.fktsv.cn/Article/details/gvkypgsoz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.bbcook.cn/Article/details/glnsysrzg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/guejvqwsw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.sjlbkw.cn/Article/details/ggonxdmyh.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gkfqnanhs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/govkleedd.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gqnxudajo.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/gbxfehfdw.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/goufybias.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.vehdjk.com/Article/details/gtafpznzv.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gnwxbkiix.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/ghqmfsayx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gwxegmpky.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.tarul.cn/Article/details/gvukrurzu.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gwvovcduh.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gjsanebvz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/ghylglypb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/grwuapdzi.sHtML

[R54] 比较两个文件
来源：http://www.blog.fktsv.cn/Article/details/gvlaperjn.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gaeletwta.sHtML

[R55] 压缩与解压
来源：http://www.share.bbcook.cn/Article/details/ginctxjmx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gbiqnoojr.sHtML

[R56] 远程拷贝
来源：http://read.share.tarul.cn/Article/details/gukiuocvn.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/gohdypwsu.sHtML

[R57] 远程执行命令
来源：http://3g.sjlbkw.cn/Article/details/ghjmzxiln.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gdjjbhxzp.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/gghqotlhp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gzfdldmnl.sHtML

[R59] 发 POST JSON
来源：http://m.share.tarul.cn/Article/details/gtzszdhzc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.bbcook.cn/Article/details/gksjddrqe.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gxzboideh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/gjlgsnmkp.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gklqixntd.sHtML

df -h;  du -sh *
来源：http://www.share.epnwcf.com/Article/details/gwvispjow.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/goqbfyvvh.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/gxxurdyuw.sHtML

[R63] 内存与进程
来源：http://www.share.bbcook.cn/Article/details/gcwdzpumx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gfvbdffsk.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gayjkrirg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fktsv.cn/Article/details/gsoiaihls.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/gqhspevmu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/grlvukmhn.sHtML

[R66] 定时任务
来源：http://wap.fktsv.cn/Article/details/gzewntplc.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gdydusfcg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gbdatuvhy.sHtML


<!-- 参考信息 -->