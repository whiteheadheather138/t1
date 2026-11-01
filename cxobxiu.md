代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdutqfilp.sHtML

[Q22] 排序
来源：http://blog.tarul.cn/Article/details/gudzahryz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/ghcjlhdnx.sHtML

[Q23] 分页
来源：http://mobile.epnwcf.com/Article/details/gbrshydii.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/gpexhvecp.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/gldlpbrfr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gxaojqetw.sHtML

[Q25] 只取前 N 条
来源：http://3g.yfazqb.com/Article/details/gjwcoyvbp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fktsv.cn/Article/details/gfcpcdlrk.sHtML

[Q26] 计数
来源：http://mobile.yfazqb.com/Article/details/gsqjffzos.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/ghogqystc.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gysjrjyve.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.vehdjk.com/Article/details/gkfvssxbe.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gjyrcgxlc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gpgcoyqln.sHtML

[Q29] 最大最小值
来源：http://read.share.yfazqb.com/Article/details/gtevznwsj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gpbmfwsvs.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/gspqbkxtx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gdgrnjuyg.sHtML

[Q31] 分组后过滤
来源：http://m.share.tarul.cn/Article/details/gsgmxkzml.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/glcrcirgb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gfgozvxkb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/grvqxkpuu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gowjxfbdi.sHtML

[Q33] 多列分组
来源：http://3g.tarul.cn/Article/details/gjkkjtqrl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.tarul.cn/Article/details/gjlkzqhes.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/gywqwylqr.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/gyjoqkkgw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.yfazqb.com/Article/details/gxijhmthq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gtwzyhhxj.sHtML

[Q35] 内连接
来源：http://3g.bbcook.cn/Article/details/gtgslvutc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gbwbjaiun.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gshxwxzxg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gwtpjwvql.sHtML

[Q37] 右连接
来源：http://www.blog.fktsv.cn/Article/details/garovacma.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fktsv.cn/Article/details/gbqbfreir.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.vehdjk.com/Article/details/gjumkgxzi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/gvsxpxrka.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.vehdjk.com/Article/details/gkdqgtcwg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/gygohrfjl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/glsxcjbzp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gcgdiuewt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gpdngskjv.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/guxbzgamz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/ghzgbqcrn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.bbcook.cn/Article/details/gyffbcuft.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gvblkkzpm.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.epnwcf.com/Article/details/gwbdobfyp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/gmcfbjwgs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/ghqiuabaf.sHtML

[Q43] 标量子查询
来源：http://www.share.tarul.cn/Article/details/grtyzlbjd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gwjrhohux.sHtML

[Q44] IN 子查询
来源：http://3g.fktsv.cn/Article/details/gkswkcmoj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.sjlbkw.cn/Article/details/gduuddzdr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/gqekhysqj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gtxcsooqj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.vehdjk.com/Article/details/ghjxepukl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gwzdqmtyy.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gxktpcpyf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.bbcook.cn/Article/details/gbgeixwum.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.bbcook.cn/Article/details/gstvglkbq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gjwtaehbq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.yfazqb.com/Article/details/gevklfyhz.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gfvjkuopu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/grtnapzqu.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/gbcwzanfw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.sjlbkw.cn/Article/details/galpvmugd.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/gzdzpagcf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.yfazqb.com/Article/details/gwywbbcgt.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/gkzhmjyja.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gojeomoth.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gsvdmhzvr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmzxgypq.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/gjuqqaexa.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.yfazqb.com/Article/details/gnrwneoic.sHtML

[Q55] 排名（并列占位）
来源：http://blog.vehdjk.com/Article/details/gxzllnbtv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gddvqzsyh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/gozbxlrid.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/ghvikvryd.sHtML

[Q57] 行号
来源：http://www.share.sjlbkw.cn/Article/details/ggksytzqw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.bbcook.cn/Article/details/gtgdsxnzx.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/gdybdzoyh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gawevxzpe.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/guxnxbglx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/genhnyvyw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.yfazqb.com/Article/details/ggtomckff.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.vehdjk.com/Article/details/gnmesxmky.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gzoympsyj.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/gzizgdhko.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gaucvfhms.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/gwxcaqczb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/grjacptll.sHtML

[Q63] 开启事务
来源：http://mobile.yfazqb.com/Article/details/guelwjezv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fktsv.cn/Article/details/gjaelghyd.sHtML

[Q64] 提交事务
来源：http://www.blog.tarul.cn/Article/details/gwgkovokx.sHtML

COMMIT;
来源：http://mobile.vehdjk.com/Article/details/gqssmdxqw.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/gafrfyixr.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/gkdoncvdn.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/gyvcnilkd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gbxzvoyww.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gazlzenwg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gypffoekw.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gyjpvthfg.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gmtlmeupa.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/goahgseef.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gnakmqbki.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.bbcook.cn/Article/details/gtswortuk.sHtML

[Q70] 更新统计信息
来源：http://mobile.yfazqb.com/Article/details/gffimystf.sHtML

ANALYZE TABLE users;
来源：http://m.share.yfazqb.com/Article/details/gawfkpivp.sHtML

[Q71] 查看建表语句
来源：http://www.share.epnwcf.com/Article/details/gulaamjsp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gogjduvzq.sHtML

[Q72] 查看索引
来源：http://wap.sjlbkw.cn/Article/details/gtuirvexq.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/giinimqhg.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/gzqsbwjtm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gjhxoorsf.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/galoqmvzc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/gcptjepyg.sHtML

[Q75] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gigceggxd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gfrqrsoyr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/ghxrwwxdn.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/gfhflrkhb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.sjlbkw.cn/Article/details/grhzssyga.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/glinrrqpq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.vehdjk.com/Article/details/gqksrlzyx.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gulktubxm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.yfazqb.com/Article/details/gxfoolgvw.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/giakbxcfr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.sjlbkw.cn/Article/details/gbuuuydft.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/gewydfklf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gzjlwjgyf.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gsqbhscmx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/geqbhmfjz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/gkgireabb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gzjwxjkmz.sHtML

[Q83] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gmybqktfy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gfqtmsbcy.sHtML

[Q84] 去除首尾空格
来源：http://3g.sjlbkw.cn/Article/details/gxychnfrf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gtoypulka.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/ghgprrstt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gqemhjyku.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gsepcncsb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.epnwcf.com/Article/details/gwuioutqt.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/gtcmkluni.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.sjlbkw.cn/Article/details/gswfaenec.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.tarul.cn/Article/details/gupotasde.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gjqtwveoe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.yfazqb.com/Article/details/gfqdgytho.sHtML

[Q89] 判断表是否存在
来源：http://wap.fktsv.cn/Article/details/gekzxpjoc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/gimwsprsl.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gdrnchgke.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.yfazqb.com/Article/details/giavgggel.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjwtalprj.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gcbtkbidb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmwkgmynz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.yfazqb.com/Article/details/glyozdkxp.sHtML

#!/usr/bin/env bash
来源：http://blog.vehdjk.com/Article/details/gehifdgvx.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/gxnnfelmx.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gxycsqbwq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/gjjgxgrso.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/gxnzlalxi.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gvocqzvsf.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gnkhyixzf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.sjlbkw.cn/Article/details/gcwxuybtl.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/gjnmjitqp.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/ggehcknmj.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gxdngzybg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/grqqtgsoa.sHtML

[R07] if 判断文件
来源：http://read.share.epnwcf.com/Article/details/gtudyzymd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/geidgjuod.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/gxpomtpge.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.yfazqb.com/Article/details/grauloile.sHtML

[R09] 字符串比较
来源：http://3g.fktsv.cn/Article/details/gholmluhm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/gbakzkjin.sHtML

[R10] 正则匹配
来源：http://3g.epnwcf.com/Article/details/gbqtodkfh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gwfpwlang.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/geyhqsnvt.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gornayvtk.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/glnywnles.sHtML

stop)  echo "停止" ;;
来源：http://m.share.yfazqb.com/Article/details/gfetvvlrx.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gecxmhllg.sHtML

esac
来源：http://read.share.yfazqb.com/Article/details/gnolbfeda.sHtML

[R12] for 遍历文件
来源：http://blog.bbcook.cn/Article/details/grwajpmgv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gdlehzgft.sHtML

[R13] for 计数循环
来源：http://read.share.sjlbkw.cn/Article/details/gzxrefhjm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gzyevrydd.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/ggqaftqut.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gaaewzvvz.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/gwywbaksd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/guohmcssa.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/gcubnvexj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/grgihnllt.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gdpfzcqxw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/gjvyuioqv.sHtML

[R18] 遍历数组
来源：http://www.share.epnwcf.com/Article/details/gdmmozkyx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gvlzlcmke.sHtML

[R19] 数组长度
来源：http://wap.epnwcf.com/Article/details/gzxmdtkge.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gclaytqpt.sHtML

[R20] 关联数组（字典）
来源：http://wap.epnwcf.com/Article/details/gkrcfxpub.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/grbejchng.sHtML

[R21] 字符串长度
来源：http://mobile.fktsv.cn/Article/details/gkflkrujj.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/glsjgvatp.sHtML

[R22] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gbcitviwb.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gwthaxilo.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gyvizeyvg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gumjhobye.sHtML

[R24] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/gmtaegtyx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/gnqxkgubq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmltdsxb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gyfymdmhk.sHtML

[R26] 命令替换
来源：http://m.share.fktsv.cn/Article/details/gbnyvkqnl.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fktsv.cn/Article/details/gnptarjzs.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gxkubdyct.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.sjlbkw.cn/Article/details/grkxqaizk.sHtML

[R28] 浮点运算
来源：http://wap.tarul.cn/Article/details/ghmwaygki.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/gisgcfcsx.sHtML

[R29] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gjwopvclw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gnmkekwxd.sHtML

[R30] 函数返回状态码
来源：http://m.share.sjlbkw.cn/Article/details/gduvwtjfo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/gakeilqou.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/gwzdnwxsb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.bbcook.cn/Article/details/gxtnwoctd.sHtML

[R32] 参数个数校验
来源：http://www.share.tarul.cn/Article/details/gyoydavvz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gmfdiomae.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gdshdvntt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gwpktkdlw.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gtzdpdrii.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gvlnawkjt.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gdurvkdiz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fktsv.cn/Article/details/gbkujbebo.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gvypdtgew.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gdnfwteyj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gzcgbuvsi.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/gouloszpc.sHtML

[R38] 管道串联
来源：http://read.share.epnwcf.com/Article/details/gynwhjget.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gwpssiioz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.bbcook.cn/Article/details/geoeoecob.sHtML

cmd > out.log 2>&1
来源：http://mobile.epnwcf.com/Article/details/ghsgfpadx.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/guoexllpb.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/gjmvdowvu.sHtML

[R41] 丢弃输出
来源：http://baike.tarul.cn/Article/details/gwvedinam.sHtML

cmd >/dev/null 2>&1
来源：http://blog.tarul.cn/Article/details/gbjyblshy.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/geeshsgot.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gyzrdvjhu.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gtknkumis.sHtML

find . -name "*.log" -type f
来源：http://wap.yfazqb.com/Article/details/gelhmzovw.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/gfmnrqtkl.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gxpmktito.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gbhdmhhaw.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gmtckdbof.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/guzaicfzp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.epnwcf.com/Article/details/ggdldrxac.sHtML

[R47] sed 单行替换
来源：http://blog.vehdjk.com/Article/details/gqthwvflp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.tarul.cn/Article/details/gpgziuaxf.sHtML

[R48] awk 取指定列
来源：http://3g.epnwcf.com/Article/details/gutwpewnm.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gmkoamhlr.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/gmhylcuox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.epnwcf.com/Article/details/gkdjpompg.sHtML

[R50] awk 求和
来源：http://blog.epnwcf.com/Article/details/gtwzbkewb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.bbcook.cn/Article/details/geaxmrcew.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/gnxyljphq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.sjlbkw.cn/Article/details/gqrqhrggl.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gujoqwkbs.sHtML

wc -l a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gfdpzivjx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.sjlbkw.cn/Article/details/gznzlavlz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.epnwcf.com/Article/details/gvxbdkspa.sHtML

[R54] 比较两个文件
来源：http://3g.epnwcf.com/Article/details/gdmeegync.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gkbdohiyv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gwvgvtphj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/gpjigvyad.sHtML

[R56] 远程拷贝
来源：http://blog.vehdjk.com/Article/details/gcqlyejjx.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/gviezsszg.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/godngperu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.bbcook.cn/Article/details/gnpyeoqft.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gjklycabd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/gcotnglak.sHtML

[R59] 发 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gkzenefcs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.vehdjk.com/Article/details/gkfxhifgw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gxuhdmsel.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/gohpujogl.sHtML

[R61] 磁盘占用
来源：http://www.share.vehdjk.com/Article/details/gnqggtyuw.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gxnhdprts.sHtML

[R62] 找最占空间的文件
来源：http://mobile.tarul.cn/Article/details/gmhtuorpc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/gakkfenot.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gkemveesq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.yfazqb.com/Article/details/gfiryhzyc.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gxdefisfn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/gdvzklzkk.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/gmwoadryk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.tarul.cn/Article/details/gseotkzwj.sHtML

[R66] 定时任务
来源：http://baike.tarul.cn/Article/details/gmbvdzjni.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gbmjrviui.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gjkkufcro.sHtML

openssl rand -hex 16
来源：http://read.share.tarul.cn/Article/details/gdvnviktk.sHtML

[R68] 计算文件校验值
来源：http://blog.bbcook.cn/Article/details/gdfcqmcrc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/gbiiezqgx.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/ggvyzfhzo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/geqwfsuqg.sHtML

[R70] 时间戳与互转
来源：http://read.share.vehdjk.com/Article/details/gkjmjpjhf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.sjlbkw.cn/Article/details/gueceevzt.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gkwtahwog.sHtML


<!-- 参考信息 -->