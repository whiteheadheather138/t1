代发 wailian999

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/glgsntmov.sHtML

[Q16] 查询指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gblyliopg.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gsqpywbxo.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/gozlpsifq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/germspwds.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/gpkgraidq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gzojmovwv.sHtML

[Q19] 范围查询
来源：http://m.share.epnwcf.com/Article/details/gnbdpbfqe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gfgvhrocl.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gyxiitbbw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fktsv.cn/Article/details/ghvxvruqr.sHtML

[Q21] 空值判断
来源：http://3g.tarul.cn/Article/details/gzlspnfok.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gqdgwyhuj.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gxbyiqaqi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/gtghfnodj.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gtujildmm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gzpbxcumr.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gbuzxwyqs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gbiuonbqz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.vehdjk.com/Article/details/gxjwmxtwk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/ghoemknoh.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/gyyhsdwar.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gdbyqceft.sHtML

[Q27] 条件计数
来源：http://baike.sjlbkw.cn/Article/details/ghdbfmysq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gvizrhsis.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gnuftwfic.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gnokxegzi.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/grnxpzkjm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gjbyqbhxp.sHtML

[Q30] 分组统计
来源：http://blog.sjlbkw.cn/Article/details/ghlxolfkh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gjoxtirjv.sHtML

[Q31] 分组后过滤
来源：http://m.share.bbcook.cn/Article/details/gcjezikzt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/gaoqurvet.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gdbmnrvjs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gzyrpfxoc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gljtjsmkc.sHtML

[Q33] 多列分组
来源：http://blog.fktsv.cn/Article/details/gmvmgumnr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fktsv.cn/Article/details/gwradpruf.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/gbvpkyaki.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/gxterglat.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/gyqzjlddk.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/gwuexohcs.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gspiehiqf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gwzcqldtx.sHtML

[Q36] 左连接
来源：http://blog.sjlbkw.cn/Article/details/gppoejkqn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gdbcenjld.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gdcxjrnwi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.epnwcf.com/Article/details/gadgkqbxw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.yfazqb.com/Article/details/gfctxnqwo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.bbcook.cn/Article/details/gbyzdxzba.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.tarul.cn/Article/details/gjngqlnzn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.epnwcf.com/Article/details/gagswejfj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.tarul.cn/Article/details/ghncxsvvk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fktsv.cn/Article/details/gtzkrqhxp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.sjlbkw.cn/Article/details/gmltssamw.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/gtpthkskx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.tarul.cn/Article/details/gojiepumd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.epnwcf.com/Article/details/gnviljzrj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gaqiqujyc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/ggkzfyekp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.epnwcf.com/Article/details/gavzyndaq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/gvtbalopx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.vehdjk.com/Article/details/gvqsgpeey.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fktsv.cn/Article/details/gpbuskimg.sHtML

[Q44] IN 子查询
来源：http://baike.epnwcf.com/Article/details/girevshez.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.yfazqb.com/Article/details/gbmqrdwjx.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gzlsqgcuy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gtlsqwogo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.tarul.cn/Article/details/gikucnppc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/geijnbdum.sHtML

[Q47] 与平均值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gpruffiei.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fktsv.cn/Article/details/gzhqgmtnp.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/goerlryue.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/gnjilwrkt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.yfazqb.com/Article/details/grezfazdy.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/gqbazbqtt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gxgepeqqj.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/gbgldklop.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/ghrhcfguh.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gcrwrpful.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gvznggqhu.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/gbxxwwrfu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/gboxnsswp.sHtML

[Q53] 按条件删除
来源：http://m.share.epnwcf.com/Article/details/ghhxybegr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.yfazqb.com/Article/details/gettclsuy.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/gypbcyobz.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.sjlbkw.cn/Article/details/gatqlmtoo.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/grbgzlzgm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/geiwielzt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gfrrgcedm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gkzzulgaj.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/ggaibckir.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gapavtfre.sHtML

[Q58] 累计求和
来源：http://read.share.tarul.cn/Article/details/gwpnlgksw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gccdtoexz.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/gtfsowrod.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gakvlkegb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.vehdjk.com/Article/details/gmkacdsqc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gvzepbbki.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fktsv.cn/Article/details/getxnxijg.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gwlplstvo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/ggrqymgzg.sHtML

[Q62] 分组占比
来源：http://m.share.sjlbkw.cn/Article/details/gqyuaglph.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/ghhnpgmak.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/ggdcrhbxo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/gjwhxnmzs.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/gaakqlwtq.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/gqtzdaycm.sHtML

[Q65] 回滚事务
来源：http://3g.bbcook.cn/Article/details/grlmssvmk.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/gfvivgpxn.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/gjiidyyck.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gwqnquaex.sHtML

[Q67] 设置隔离级别
来源：http://mobile.sjlbkw.cn/Article/details/gmzlqhdnd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gxkelxpwb.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/gtxmhgtdk.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/goijmhwem.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gkrlqhyxj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gqrdneinh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/glmjeqgth.sHtML

[Q70] 更新统计信息
来源：http://www.share.fktsv.cn/Article/details/gfibvdown.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gbpiemzwp.sHtML

[Q71] 查看建表语句
来源：http://read.share.tarul.cn/Article/details/givmdolds.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/guedemxer.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gxsatdkqb.sHtML

SHOW INDEX FROM users;
来源：http://wap.epnwcf.com/Article/details/gjuysfmlc.sHtML

[Q73] 查看表状态
来源：http://blog.vehdjk.com/Article/details/gppiatfec.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.bbcook.cn/Article/details/gmbuioaay.sHtML

[Q74] 强制使用索引
来源：http://read.share.tarul.cn/Article/details/gibatvszi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gwmyrulcx.sHtML

[Q75] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/govmhdcax.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gmxscckbq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.yfazqb.com/Article/details/gphmokacx.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/gqlabbnsy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/gsrpluapq.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfojzxtd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gqafsrrvb.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gzckwzmwh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fktsv.cn/Article/details/gsewdqdrc.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gjiewzsnw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.epnwcf.com/Article/details/gsvljdhvk.sHtML

[Q80] 字符串截取
来源：http://m.share.sjlbkw.cn/Article/details/gnnszrrwt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gcumkhjas.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gqnuzdaxo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/gvjguiyjg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gcwwswtmm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/ghqqdueqy.sHtML

[Q83] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gakdcpycc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gsdgsyfsk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/gnaayrudo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/guluhfunx.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/gfttxfeqr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gzzkvczsk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gwluokyqe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gttgagugk.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gxokdrxbm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gubgrgglb.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.epnwcf.com/Article/details/gbfpyutey.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/gyvduengn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.vehdjk.com/Article/details/gapyqumpx.sHtML

[Q89] 判断表是否存在
来源：http://wap.fktsv.cn/Article/details/gqbgsuhpx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.yfazqb.com/Article/details/gllnlvizz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/ggqudphrf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.sjlbkw.cn/Article/details/glpaiujgc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gutwktnqd.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gcwfftnrv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grqpizbue.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/guqiuvhcz.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gxmflnkav.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/gwmhoewou.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gxshsxunm.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/gweejfder.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/ghaxstrii.sHtML

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/gykjaiydc.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/gmhstucis.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gkzhngkwq.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/gsrzlgulg.sHtML

name="${1:-default}"
来源：http://blog.epnwcf.com/Article/details/gwowrsngf.sHtML

[R06] 判断命令是否存在
来源：http://m.share.yfazqb.com/Article/details/gehvphtbo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gkaykncpf.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gctxsklrm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.bbcook.cn/Article/details/glnjgtwsy.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/gpnskbelp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gbiikncoy.sHtML

[R09] 字符串比较
来源：http://3g.fktsv.cn/Article/details/gqxrrmues.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/grlxoiucb.sHtML

[R10] 正则匹配
来源：http://m.share.yfazqb.com/Article/details/gbuwftqvg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/grvdzomvy.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/gdgcanjtj.sHtML

case "$1" in
来源：http://read.share.vehdjk.com/Article/details/glgsadqni.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/gthxclrno.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.epnwcf.com/Article/details/gqtenvnfp.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.vehdjk.com/Article/details/grnryojzf.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gsodwgjlx.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/gifaamgxn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.epnwcf.com/Article/details/gdxomgeru.sHtML

[R13] for 计数循环
来源：http://3g.bbcook.cn/Article/details/gwhusgccc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/gamgiyldv.sHtML

[R14] C 风格 for
来源：http://m.share.vehdjk.com/Article/details/gzwtaeich.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gzjhnfvyk.sHtML

[R15] while 逐行读文件
来源：http://3g.epnwcf.com/Article/details/gawofquop.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/gpadmkawt.sHtML

[R16] until 等待条件
来源：http://read.share.bbcook.cn/Article/details/gdxaqikrr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gmogpstbv.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gpmwgsxga.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.vehdjk.com/Article/details/gitcziunj.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/gwjfpjfdi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.bbcook.cn/Article/details/gwedocosx.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/gglfjyyxf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpacmklwu.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gdjwujkwe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/ganrtooll.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/glebvrjlc.sHtML

echo "${#s}"
来源：http://mobile.tarul.cn/Article/details/gxpheoqhg.sHtML

[R22] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gfuioubwu.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gbpslhdmm.sHtML

[R23] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/ghnilndrb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fktsv.cn/Article/details/gcaimwwla.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gnnfzvemb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.sjlbkw.cn/Article/details/gqbonwpvy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gevdknncw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.sjlbkw.cn/Article/details/gflsuclnm.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gttvsivla.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/gaejfeadl.sHtML

[R27] 算术展开
来源：http://www.blog.tarul.cn/Article/details/gwenrjalv.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gdlmprxpk.sHtML

[R28] 浮点运算
来源：http://baike.tarul.cn/Article/details/gjvfbptzr.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gazyunrhd.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/gkmbqxhsz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.sjlbkw.cn/Article/details/gvpkbzjdh.sHtML

[R30] 函数返回状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gvbmemrli.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/gjxvefnvi.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/gjlcvshhy.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.yfazqb.com/Article/details/gqqleclij.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/gvngtping.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/geacvpazc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gahopwlrv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gtrwztgtn.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/grqlvwyax.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gspnkheqa.sHtML

[R35] 后台执行并等待
来源：http://baike.vehdjk.com/Article/details/gulxlbawo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gqpfeiigx.sHtML

[R36] 并发执行多个任务
来源：http://m.share.vehdjk.com/Article/details/goczveszh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.bbcook.cn/Article/details/gexsoyftr.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/gbovloktt.sHtML

files=$(ls -1)
来源：http://baike.yfazqb.com/Article/details/gtmaxmxkw.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/ghqixtqyq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.bbcook.cn/Article/details/gkerndigz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.sjlbkw.cn/Article/details/gwyvlsxcs.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/gtomanwfe.sHtML

[R40] 追加写日志
来源：http://blog.yfazqb.com/Article/details/gafnqyjnt.sHtML

echo "log" >> out.log
来源：http://baike.fktsv.cn/Article/details/gusrquafl.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/ghqrvbnqh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/glgjejgpo.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gmuifvrbz.sHtML

wc -l < a.txt
来源：http://www.share.bbcook.cn/Article/details/gixvotlho.sHtML

[R43] 按名字查找文件
来源：http://3g.vehdjk.com/Article/details/ghssqcqkq.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gbzlcxuai.sHtML

[R44] 按修改时间查找
来源：http://m.share.vehdjk.com/Article/details/gkxhngjpx.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/goiiykolo.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/gdagpbtbc.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.sjlbkw.cn/Article/details/glrrhgwbw.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/ghdortzla.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.sjlbkw.cn/Article/details/gdqoevlek.sHtML

[R47] sed 单行替换
来源：http://blog.yfazqb.com/Article/details/grikdjmpi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gkegxqmgx.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gyknjvghf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.vehdjk.com/Article/details/gqjcwhgvx.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/ggedbifyi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.yfazqb.com/Article/details/gmpvpmitw.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gdnuqdnsz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gxxcoglce.sHtML

[R51] 排序去重取前几
来源：http://www.blog.sjlbkw.cn/Article/details/ggcbppxcf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.sjlbkw.cn/Article/details/gicjpbkij.sHtML

[R52] 统计行数
来源：http://m.share.yfazqb.com/Article/details/gvzftxkic.sHtML

wc -l a.txt
来源：http://www.blog.vehdjk.com/Article/details/gepceywzj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.epnwcf.com/Article/details/gchmoljfd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gapkkbksm.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/gwbrcvqwi.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gvmaiycah.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gsbzcskml.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/gxylrnpcg.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gwmgmayfw.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/gxnmxbhkj.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gutepzkjj.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/ghnezjven.sHtML

[R58] 下载文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzukjiif.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.bbcook.cn/Article/details/gnbkfsmjt.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gzlqheumd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.yfazqb.com/Article/details/glqyuibus.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gmjarsdhz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.bbcook.cn/Article/details/gopmhmije.sHtML

[R61] 磁盘占用
来源：http://m.share.tarul.cn/Article/details/gqltjkieo.sHtML

df -h;  du -sh *
来源：http://wap.fktsv.cn/Article/details/gxhlhlunj.sHtML

[R62] 找最占空间的文件
来源：http://mobile.sjlbkw.cn/Article/details/gqmrffuve.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gsovgspqa.sHtML

[R63] 内存与进程
来源：http://www.m.share.bbcook.cn/Article/details/gsbdnufcp.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gzsjwspay.sHtML

[R64] 结束进程
来源：http://blog.vehdjk.com/Article/details/ggvbxvwfk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gynzrmfur.sHtML

[R65] 查看端口占用
来源：http://read.share.sjlbkw.cn/Article/details/gedielfdp.sHtML


<!-- 参考信息 -->