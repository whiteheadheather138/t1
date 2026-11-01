代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/gldmfxtpv.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/gpzgbmwlc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/geebnxdrd.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/ggzigzfim.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gbzfgqwyz.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gsiliwtpa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gzvqmvgla.sHtML

[Q23] 分页
来源：http://baike.fktsv.cn/Article/details/gaqafngjj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.bbcook.cn/Article/details/gohrvvrau.sHtML

[Q24] 去重
来源：http://3g.yfazqb.com/Article/details/gjqhvjdpz.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gkkalifrj.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/gxotxazpa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fktsv.cn/Article/details/gkzyegvqt.sHtML

[Q26] 计数
来源：http://wap.fktsv.cn/Article/details/gkxxzlotb.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gqdhmpdwo.sHtML

[Q27] 条件计数
来源：http://read.share.yfazqb.com/Article/details/gogcbclzs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.vehdjk.com/Article/details/gaxhjgxeb.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/gxmtdzcda.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gdgmzzxno.sHtML

[Q29] 最大最小值
来源：http://blog.vehdjk.com/Article/details/gutrlooyy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gxngpiwiq.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gbbtpvons.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gkkefqncg.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/gndgyxqfr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gyixwsdcp.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gkorkelev.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gjmpmvxez.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.bbcook.cn/Article/details/goypbdyar.sHtML

[Q33] 多列分组
来源：http://blog.epnwcf.com/Article/details/gjylgmayf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.tarul.cn/Article/details/gvrlppamp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/gyshbccyc.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/gqydcetwz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.yfazqb.com/Article/details/gcamgtkqt.sHtML

) t WHERE rn = 1;
来源：http://baike.fktsv.cn/Article/details/gweidebvh.sHtML

[Q35] 内连接
来源：http://www.share.tarul.cn/Article/details/glrxchslx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gjphjppqd.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/gcpqiffbr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/giyyiykji.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/giydnxiiv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gfyltzykb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gxgcgzvae.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.yfazqb.com/Article/details/gqpvlrlkj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fktsv.cn/Article/details/gcmnpuczq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.vehdjk.com/Article/details/gfyucutvi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fktsv.cn/Article/details/gbnrhefgl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gefwfjqyu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gyvtpfyay.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/gfuzeucko.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/gvpqhznub.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gmzfkmtjs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.epnwcf.com/Article/details/ghjjrdnpv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gsyzjwnwn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/getwtsqng.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gdhlawqgr.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gncavxcxz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.epnwcf.com/Article/details/geejvyzzq.sHtML

[Q44] IN 子查询
来源：http://3g.vehdjk.com/Article/details/gfoojbncp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/gqqbtghvc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gpubadtia.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gbhmjvvsg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gflfmlhjv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gsskkbeca.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/garpldwvr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gaqamuodq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.bbcook.cn/Article/details/gonxlhnyh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.tarul.cn/Article/details/glvpptmcy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gwxcqmhlz.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gzkywohio.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/guyvijwrh.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gabzqcyjr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.vehdjk.com/Article/details/gmiixaqqp.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gbxjixggh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/gaoxcxovx.sHtML

[Q52] 删除指定行
来源：http://baike.sjlbkw.cn/Article/details/gzcbmlhqb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gzddonevj.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gunyerniv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fktsv.cn/Article/details/guvqwjido.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/guuwfhjwp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.yfazqb.com/Article/details/giozsfiuk.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.yfazqb.com/Article/details/gdqejxqom.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/gxcjkhmfu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/givkecayr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gppmuutfl.sHtML

[Q57] 行号
来源：http://blog.tarul.cn/Article/details/gmposahbi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.tarul.cn/Article/details/gnqnysghq.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/gysxtaxsr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gsiofjmqz.sHtML

[Q59] 分组内累计
来源：http://m.share.tarul.cn/Article/details/gsjnjjjug.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gueeqjfiv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.vehdjk.com/Article/details/guudidfsb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fktsv.cn/Article/details/ghehlhdxb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gcboqwgwi.sHtML

[Q61] 移动平均
来源：http://3g.sjlbkw.cn/Article/details/gxhacjimw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gnsqvykxq.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/girnitpwa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gpnmvhybx.sHtML

[Q63] 开启事务
来源：http://baike.yfazqb.com/Article/details/gdmsyurgd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/glvvdvini.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gchywmfua.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gsakgujog.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gfitatvtz.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gixldwgzp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.bbcook.cn/Article/details/gqdmvbnce.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.bbcook.cn/Article/details/ghmdwfwgl.sHtML

[Q67] 设置隔离级别
来源：http://baike.yfazqb.com/Article/details/gbisrhtfw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/gwsldibhn.sHtML

[Q68] 保存点
来源：http://www.blog.yfazqb.com/Article/details/gbagdjmbs.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gganuetqe.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/gzuqzjafq.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gsotolhkn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.yfazqb.com/Article/details/gtzvothzn.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gqhfhcmbb.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/gndtwoiyh.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/gakxtdipu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.epnwcf.com/Article/details/gytupbmng.sHtML

[Q72] 查看索引
来源：http://blog.vehdjk.com/Article/details/geywetttd.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gofijgmyp.sHtML

[Q73] 查看表状态
来源：http://www.share.yfazqb.com/Article/details/gyflwxtdq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gixjlmszh.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gzrxcfrcq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.sjlbkw.cn/Article/details/grpduedwg.sHtML

[Q75] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gzscfzacz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/goatdkooa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gawqeqkry.sHtML

[Q76] 按天统计
来源：http://www.blog.epnwcf.com/Article/details/gjynegeik.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gwlbqqosa.sHtML

[Q77] 时间加减
来源：http://baike.tarul.cn/Article/details/ghhepolbp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.vehdjk.com/Article/details/gcljrlddn.sHtML

[Q78] 当前时间
来源：http://www.blog.bbcook.cn/Article/details/gvqosljhl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.bbcook.cn/Article/details/gygkzlyoc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gqlwurpto.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gsnickwoq.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gzvfyzwhe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gohezaasn.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gtyozihtn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/gqlwylhxv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.vehdjk.com/Article/details/gcswckrxk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/ghswloujx.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gthykqjov.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gfjuggxkh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/gnvrrpmuj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvegltyd.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/gzchlxshh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.tarul.cn/Article/details/gscllfvxv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.vehdjk.com/Article/details/gnhvvadyf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gzthnqftt.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/glglkosuh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gpysfkrpp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.tarul.cn/Article/details/gpslbomfo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gangyfobt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gowdujfig.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/glorezvwp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gjecqcctw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gfgewqsta.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/guxixacox.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glkobyhmh.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/gwxtuetio.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcjibdgia.sHtML

[R01] shebang 与严格模式
来源：http://m.share.sjlbkw.cn/Article/details/gpfwtjsli.sHtML

#!/usr/bin/env bash
来源：http://3g.yfazqb.com/Article/details/gstywvhhf.sHtML

set -euo pipefail
来源：http://baike.sjlbkw.cn/Article/details/gpotfmsot.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/ggttcfogm.sHtML

name="Tom"; echo "$name"
来源：http://blog.tarul.cn/Article/details/gpsljiwwl.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gppbgdguf.sHtML

readonly PI=3.14
来源：http://mobile.sjlbkw.cn/Article/details/gzaytzxzb.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gnqkbdkko.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/gsubejhxu.sHtML

[R05] 参数默认值
来源：http://wap.tarul.cn/Article/details/gfcdvkzqt.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gwvopepct.sHtML

[R06] 判断命令是否存在
来源：http://m.share.vehdjk.com/Article/details/gwgmfxumo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gldrvojqc.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/gmkblowee.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.epnwcf.com/Article/details/gymfksras.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/gleylgarx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.yfazqb.com/Article/details/gpvmjuyoi.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gjhwupxqw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/glzbcfldf.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/gktxzrqte.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/gahlofqit.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gupbwuokl.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/gbhxczpfl.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/grgkvglol.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/garoerjgx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gxqivccyk.sHtML

esac
来源：http://3g.tarul.cn/Article/details/gfubadvpr.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/guggllfwl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.sjlbkw.cn/Article/details/gecskdthx.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gnwpgykdm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gpqsqmqsj.sHtML

[R14] C 风格 for
来源：http://mobile.sjlbkw.cn/Article/details/gmvlxygvn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gavfuihqs.sHtML

[R15] while 逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gtdskmoff.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gwydxzqfe.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/gsyzfqjgc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fktsv.cn/Article/details/galwlgoyr.sHtML

[R17] 数组定义与取值
来源：http://wap.fktsv.cn/Article/details/gtlirkdvm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/gqakhaqax.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gxfwnyoxk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gphgeoyyi.sHtML

[R19] 数组长度
来源：http://blog.tarul.cn/Article/details/gsvcedkdh.sHtML

echo "${#arr[@]}"
来源：http://m.share.vehdjk.com/Article/details/gqzbvpzdi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/gywiowflq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gkzumfxsz.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/gkfryrmon.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gzlhkfbzf.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gdaufgmhr.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/gfwnugfyg.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/ghxofuddq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gdrcwqxwb.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gimeevjer.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.vehdjk.com/Article/details/gyibiopka.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/geeyfjpbp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gstynkoov.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/gvxxkwphh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/gelsxovka.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/galztvorl.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/gryvueffr.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/gslylevfu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/ggxufbusx.sHtML

[R29] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gpbgyjlyk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gqtifmdsh.sHtML

[R30] 函数返回状态码
来源：http://mobile.yfazqb.com/Article/details/glpyuiqpv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gvjewninc.sHtML

[R31] 局部变量
来源：http://baike.fktsv.cn/Article/details/gjjvjlowl.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/ghrkgnqof.sHtML

[R32] 参数个数校验
来源：http://3g.sjlbkw.cn/Article/details/gimcuamzj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/giwwlxgii.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/gfnixkihb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.vehdjk.com/Article/details/gbyfevahq.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/gpwklxaco.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/grwnzckpg.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/gfuhbxwlq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gbdfpczyn.sHtML

[R36] 并发执行多个任务
来源：http://blog.bbcook.cn/Article/details/gyrlxdnpg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gvpnkrbsg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gszokcikd.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gyvsjossh.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/godzfvbsk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gyxdhcggi.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/genfupypq.sHtML

cmd > out.log 2>&1
来源：http://wap.fktsv.cn/Article/details/gpxwkhaci.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gxbchhxic.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/glyjleooq.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gkufnltre.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/ggbuagnjp.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gpjneqwde.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gpyuudgir.sHtML

[R43] 按名字查找文件
来源：http://blog.fktsv.cn/Article/details/grmtxipnc.sHtML

find . -name "*.log" -type f
来源：http://baike.yfazqb.com/Article/details/gpirqbnwr.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/ghkmqwvaf.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gyvzrlkfn.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gounuufrd.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gjaplutlw.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/gvowgyzec.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.vehdjk.com/Article/details/gmxnipvqc.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/goiysortu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxipotqf.sHtML

[R48] awk 取指定列
来源：http://www.blog.sjlbkw.cn/Article/details/glpyjwzwp.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gbgppdxsn.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/gdmscorct.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gabulyryl.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/ggniwtyve.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.tarul.cn/Article/details/gyhamjhjp.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gkcnvyhiz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fktsv.cn/Article/details/ghjyqfwjl.sHtML

[R52] 统计行数
来源：http://m.share.epnwcf.com/Article/details/gfchdddjw.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gclyozepi.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/gfxkrczpn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.vehdjk.com/Article/details/gvkqqlvtt.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gengpjdun.sHtML

diff a.txt b.txt
来源：http://read.share.fktsv.cn/Article/details/guxvyaqwz.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/gtdylcwuz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/geqxkujbf.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gjdpivnxt.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gazvekcdv.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/gcwgmipxy.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gbopqmzgj.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gdwjsiyys.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/grqblblls.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/goeaoeqta.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gynqeqcke.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gywoxjaux.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.yfazqb.com/Article/details/gppevbiip.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gqeieppoq.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/gseelxodd.sHtML

[R62] 找最占空间的文件
来源：http://blog.tarul.cn/Article/details/gjyokoaqs.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/glynyslze.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/guurhhzuu.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fktsv.cn/Article/details/gvevrogul.sHtML

[R64] 结束进程
来源：http://m.share.bbcook.cn/Article/details/glmpzvgif.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.tarul.cn/Article/details/glqjmasvm.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/geqffdiix.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gfitdxzhi.sHtML

[R66] 定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gcxurhsaz.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/ggwircgvn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gzguxovck.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gpapfvogl.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/ggvzddgoh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/gkemyutsc.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/gsrlaatbc.sHtML


<!-- 参考信息 -->