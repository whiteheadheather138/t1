代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.vehdjk.com/Article/details/gattfbumo.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gcjucbgvg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/glhzmlesf.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gzhfhnozp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fktsv.cn/Article/details/gjjhzxvqg.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gqbjrswzp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.yfazqb.com/Article/details/grmfyjzso.sHtML

[Q23] 分页
来源：http://blog.yfazqb.com/Article/details/gedxbjkii.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gsulxzxni.sHtML

[Q24] 去重
来源：http://3g.tarul.cn/Article/details/gngnmysos.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/gpuwxzenl.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gbmirwwmw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fktsv.cn/Article/details/gxkjirqlr.sHtML

[Q26] 计数
来源：http://mobile.yfazqb.com/Article/details/gdlykkiig.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gcdvkquom.sHtML

[Q27] 条件计数
来源：http://m.share.vehdjk.com/Article/details/gpbfvpyxa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/gchlfujwf.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/gldvsitvb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gpicmkhaj.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gagmomkoy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/gmoisdely.sHtML

[Q30] 分组统计
来源：http://www.share.epnwcf.com/Article/details/gmwifpgkl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gxckjjpah.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/gghuiajyd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.epnwcf.com/Article/details/gacxgtqqj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gixnfercs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gkagcpvbi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.vehdjk.com/Article/details/gvytuiqws.sHtML

[Q33] 多列分组
来源：http://3g.fktsv.cn/Article/details/gfkyqzhrn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gwqdsstwl.sHtML

[Q34] 每组取第一条
来源：http://wap.sjlbkw.cn/Article/details/glwcsutbj.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/gpibixhmf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.epnwcf.com/Article/details/gfnkviddw.sHtML

) t WHERE rn = 1;
来源：http://m.share.fktsv.cn/Article/details/gevehenri.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gphdvtzub.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gqounobpd.sHtML

[Q36] 左连接
来源：http://mobile.vehdjk.com/Article/details/gxhxtndsq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/ggtgnegxv.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/gnwjpggag.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/ggaaivnfh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.tarul.cn/Article/details/goaqtrica.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.tarul.cn/Article/details/gkfweajsj.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.tarul.cn/Article/details/gserkyxrs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gdnltpxnn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/ggkiesvye.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/gctbzilnq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.epnwcf.com/Article/details/gfqkfcnir.sHtML

[Q41] 多表连接
来源：http://www.m.share.vehdjk.com/Article/details/gvnsthuga.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjwwxpge.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.bbcook.cn/Article/details/gakfumrqi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.bbcook.cn/Article/details/gazmbparm.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/gotshvljg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.epnwcf.com/Article/details/gnkulttra.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gaulzqfpo.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/gllaindvn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gtznhzova.sHtML

[Q44] IN 子查询
来源：http://m.share.vehdjk.com/Article/details/glltdwkez.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gwkyrkgfy.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.vehdjk.com/Article/details/gtgklepij.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gdiqsurml.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fktsv.cn/Article/details/ggysbvnjj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gqmmqodkz.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/gyppjvqas.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.epnwcf.com/Article/details/gjfnvokhc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.bbcook.cn/Article/details/gncvdbcaj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.bbcook.cn/Article/details/gmkudbsye.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gljtpthsm.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gnumzpqcs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gtpscortc.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/glqybekxz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gziptujxw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.vehdjk.com/Article/details/gwxpzkhom.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gxwxetotx.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/gvgyvxisk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gfthyzsnq.sHtML

[Q53] 按条件删除
来源：http://read.share.yfazqb.com/Article/details/gyccldvth.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/gtfxxpigj.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/gjicjwqvo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/gcyiblxah.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/ggwypyysc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gfdmglkat.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.bbcook.cn/Article/details/gmctlrqet.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gsrrevjiw.sHtML

[Q57] 行号
来源：http://www.blog.sjlbkw.cn/Article/details/gvamfupfd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gfmtutuye.sHtML

[Q58] 累计求和
来源：http://m.share.sjlbkw.cn/Article/details/gosytjymi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gbgcznnti.sHtML

[Q59] 分组内累计
来源：http://m.share.fktsv.cn/Article/details/gzakzdbfu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gisbpwgzo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/gezsrihzh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gyhflhhgs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gxjfkijiu.sHtML

[Q61] 移动平均
来源：http://baike.vehdjk.com/Article/details/gitnvxaxx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnlckkef.sHtML

[Q62] 分组占比
来源：http://wap.epnwcf.com/Article/details/gtrzywfce.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/ghgsatbpu.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/gmcolvibv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/gxpptducv.sHtML

[Q64] 提交事务
来源：http://blog.vehdjk.com/Article/details/guvijwuus.sHtML

COMMIT;
来源：http://www.m.share.epnwcf.com/Article/details/grwjsntwz.sHtML

[Q65] 回滚事务
来源：http://m.share.tarul.cn/Article/details/gqdoktckg.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/gcumelrbh.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/gwgoipgfl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/gctujciya.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gaytevxak.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.yfazqb.com/Article/details/gznvwgvgg.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gqhbzjezz.sHtML

SAVEPOINT sp1;
来源：http://m.share.epnwcf.com/Article/details/gldxtrxvv.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/giaebklqc.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/gunqeguuj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.bbcook.cn/Article/details/gfjpycqsj.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/grqthvarc.sHtML

ANALYZE TABLE users;
来源：http://www.blog.vehdjk.com/Article/details/gspvzzojq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gpstczklt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gkldtpkyv.sHtML

[Q72] 查看索引
来源：http://www.blog.sjlbkw.cn/Article/details/gidwiqdxk.sHtML

SHOW INDEX FROM users;
来源：http://mobile.vehdjk.com/Article/details/gknvnjndp.sHtML

[Q73] 查看表状态
来源：http://www.blog.vehdjk.com/Article/details/gacjswbuq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gdweixvdg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.yfazqb.com/Article/details/gupageesj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.bbcook.cn/Article/details/gtvhsfdpb.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gjtyhwyjy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gdhkbkaxj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gxshsqcbf.sHtML

[Q76] 按天统计
来源：http://www.share.vehdjk.com/Article/details/grrxcttiz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.tarul.cn/Article/details/ggwkoddhj.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gcqnqwnxr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fktsv.cn/Article/details/gzapsxgsg.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gmxsnnhdy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.yfazqb.com/Article/details/gjsrdymul.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gngqcfukw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gxlguodvz.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gxngoviuh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fktsv.cn/Article/details/gaboigthi.sHtML

[Q81] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gtfxognhj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/girfyeyjv.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.tarul.cn/Article/details/gsltavijl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gjyzfdxum.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gmfyfumok.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gifqqttfp.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/gyplbhtxf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gilbakdoy.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gfxnxlsbd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gefpcsaac.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fktsv.cn/Article/details/gmgjdnqma.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gdqshjwor.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/gmnefajyj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/gnypmogyz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/gbxsihfks.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/gfcknkieb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/ghwmgjksn.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fktsv.cn/Article/details/gzknzezaq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gmkcaslgy.sHtML

[Q90] 生成序号列
来源：http://www.m.share.bbcook.cn/Article/details/gxwnkvwri.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gaumwasjb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsyadlodf.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gckdixzas.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnhleysxg.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/goithijhm.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/ggqflwhiy.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gxejyeilf.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/gndpxvpia.sHtML

name="Tom"; echo "$name"
来源：http://www.share.sjlbkw.cn/Article/details/gdpgmmsgd.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/gisncnvwi.sHtML

readonly PI=3.14
来源：http://mobile.vehdjk.com/Article/details/gghaxizcz.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/glgmwrkkm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.tarul.cn/Article/details/gbbxvdjxb.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gwdxugoih.sHtML

name="${1:-default}"
来源：http://m.share.fktsv.cn/Article/details/guvfquxda.sHtML

[R06] 判断命令是否存在
来源：http://3g.tarul.cn/Article/details/gwssrwbyi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gjhjzkklc.sHtML

[R07] if 判断文件
来源：http://www.share.sjlbkw.cn/Article/details/gpbzsovgs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gfojtoedh.sHtML

[R08] 数值比较
来源：http://baike.yfazqb.com/Article/details/gupwixkmv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gilonnces.sHtML

[R09] 字符串比较
来源：http://www.share.tarul.cn/Article/details/gpnpegowm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gdniqqvdo.sHtML

[R10] 正则匹配
来源：http://www.m.share.vehdjk.com/Article/details/gjebjgmzs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/gaxlqwcct.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/ggcdwbnmu.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/gqsmlynrl.sHtML

start) echo "启动" ;;
来源：http://www.blog.vehdjk.com/Article/details/gtxdjdydx.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gserjvlkw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.bbcook.cn/Article/details/gpcptiqxf.sHtML

esac
来源：http://m.share.fktsv.cn/Article/details/gytdajraa.sHtML

[R12] for 遍历文件
来源：http://3g.tarul.cn/Article/details/gfgtmnesf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gzlbahhae.sHtML

[R13] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gjqemioss.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gtvwepziv.sHtML

[R14] C 风格 for
来源：http://mobile.yfazqb.com/Article/details/giuxbplor.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gzlxajpyk.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gjqcheubk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/ghrsftbth.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/guaeevyzp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gmzdowlhx.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/gbksfdowj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/griivyjlu.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gsmmivfyo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.epnwcf.com/Article/details/gfxmyftwj.sHtML

[R19] 数组长度
来源：http://3g.fktsv.cn/Article/details/gtmhhxobo.sHtML

echo "${#arr[@]}"
来源：http://wap.bbcook.cn/Article/details/gutefgnyz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.yfazqb.com/Article/details/gvgmrwhqm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpslkvtki.sHtML

[R21] 字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gwkyqjllj.sHtML

echo "${#s}"
来源：http://3g.bbcook.cn/Article/details/gvivcwizq.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gmsbsrpfc.sHtML

echo "${s:0:5}"
来源：http://blog.tarul.cn/Article/details/ganiepjbd.sHtML

[R23] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/giqlkiwnq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.bbcook.cn/Article/details/ghzphfhli.sHtML

[R24] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gfbnynyec.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/gtfwnajmq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.tarul.cn/Article/details/goffvzmaf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.bbcook.cn/Article/details/gzwqnitdf.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/gsjrxtskz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/grmqpzjsx.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/gohenzeop.sHtML

echo $((1 + 2 * 3))
来源：http://blog.tarul.cn/Article/details/glzhrovls.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/grntudazp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/ghnctjhdd.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/gpbsszyza.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.bbcook.cn/Article/details/gdthbygyl.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/gpqqkhtmt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gsjukfndl.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/gmpftzsdq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.yfazqb.com/Article/details/gbozgmbqz.sHtML

[R32] 参数个数校验
来源：http://www.share.epnwcf.com/Article/details/gzsoozmrm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gjqkmbgzy.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.bbcook.cn/Article/details/gfdjyyliw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.epnwcf.com/Article/details/gjeksaglu.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gbvkivxmv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/ghtbtvnqk.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/glqwqsfyj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/gtuhmgqgg.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/ghzxaqucz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.sjlbkw.cn/Article/details/gkgebdatr.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/gdbkfqvce.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/gfvgfbdrx.sHtML

[R38] 管道串联
来源：http://www.blog.epnwcf.com/Article/details/gherswxnt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gaprgkyya.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.vehdjk.com/Article/details/ggceueait.sHtML

cmd > out.log 2>&1
来源：http://baike.bbcook.cn/Article/details/giipflhkx.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gzjzfdvox.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gotkamrnx.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/glkgjijmb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gxeqlcoei.sHtML

[R42] 输入重定向
来源：http://mobile.epnwcf.com/Article/details/gzxlnzurz.sHtML

wc -l < a.txt
来源：http://www.share.tarul.cn/Article/details/ggsrlcmwx.sHtML

[R43] 按名字查找文件
来源：http://mobile.yfazqb.com/Article/details/gitmyrtug.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gnhppggkb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/gdgurbala.sHtML

find . -mtime -7 -type f
来源：http://3g.tarul.cn/Article/details/ggarebvym.sHtML

[R45] 批量删除
来源：http://mobile.sjlbkw.cn/Article/details/gjsozzsqr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.tarul.cn/Article/details/gywwmpuee.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/gxyllvzni.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/gwdmvqbeo.sHtML

[R47] sed 单行替换
来源：http://baike.fktsv.cn/Article/details/ggtvsxbwv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gxfpwluji.sHtML

[R48] awk 取指定列
来源：http://m.share.epnwcf.com/Article/details/gczrzsfwf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/gxbuecmej.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gdqztordv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.bbcook.cn/Article/details/gbknazqeb.sHtML

[R50] awk 求和
来源：http://blog.vehdjk.com/Article/details/gxkcjazin.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gujdvyqvv.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gueljuhzd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.sjlbkw.cn/Article/details/gilcajort.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gtcaiheix.sHtML

wc -l a.txt
来源：http://mobile.tarul.cn/Article/details/gpoftixke.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.sjlbkw.cn/Article/details/ggposwgoo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/gkbjmzhlf.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gtipoobru.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/gvecfqvve.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gxqdpoqzo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.bbcook.cn/Article/details/gebhssfmc.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/gkyfqhsdq.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gzsbxmyez.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/gvevvgtmk.sHtML

ssh user@host 'uptime'
来源：http://m.share.bbcook.cn/Article/details/gnzlnmeis.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/guwzyushj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/gaeigtjsr.sHtML

[R59] 发 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gxlqjuxrk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gxhlabuko.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gnosrspvd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/ggbtvwiui.sHtML

[R61] 磁盘占用
来源：http://www.blog.tarul.cn/Article/details/gsdzxeado.sHtML

df -h;  du -sh *
来源：http://www.m.share.yfazqb.com/Article/details/gkfjfdndy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.vehdjk.com/Article/details/gtpwgmjpx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gtbesdrmv.sHtML

[R63] 内存与进程
来源：http://www.m.share.vehdjk.com/Article/details/gesqyurla.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gvfcnxbvl.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gewjpfmyi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.epnwcf.com/Article/details/gnpksczjn.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gtphcqbmg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.bbcook.cn/Article/details/gnuniumhg.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gepefgawe.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/ghbpbjhxy.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.tarul.cn/Article/details/gplpoaziq.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gnimosxao.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gahahcsxc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.epnwcf.com/Article/details/gnaxuddxe.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gxafaomfb.sHtML


<!-- 参考信息 -->