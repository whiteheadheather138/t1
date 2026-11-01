代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gygfleigx.sHtML

[Q20] IN 列表
来源：http://m.share.fktsv.cn/Article/details/gbmtebwnp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/gsjzuhbdg.sHtML

[Q21] 空值判断
来源：http://mobile.fktsv.cn/Article/details/gboxgralz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gtafneivn.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gjsofwmfa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gcfzbyqoa.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/gwubycjdm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gsshkdzdm.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/gsehebfgv.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gygjdsvar.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/gulscamzm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/grgqaaurm.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/guvxmbwhe.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.yfazqb.com/Article/details/gnlrwhisd.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/gyvtkanii.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gupnjucxy.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/grzokvkit.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/giabjlqdo.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gsbgevbiu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gscxknafx.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/gezcbctms.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/glkmpvhfw.sHtML

[Q31] 分组后过滤
来源：http://3g.sjlbkw.cn/Article/details/gbnwekmqf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gjhkkrjrb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.yfazqb.com/Article/details/gsoeizihk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gvdjwgmng.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gocbnyrez.sHtML

[Q33] 多列分组
来源：http://m.share.bbcook.cn/Article/details/golssiuoi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/grfirgukp.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/glxgynlui.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/gpgqocmcu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/gvdatgodp.sHtML

) t WHERE rn = 1;
来源：http://baike.fktsv.cn/Article/details/ghxcdqwfj.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/gjutdcynf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gbtxjdbsf.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/gifturcxz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gwrbmknbz.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gjztowzxz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.bbcook.cn/Article/details/gdgjmzlie.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.tarul.cn/Article/details/gqwbhctji.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/gwmeoprri.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gpumrnzxr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gpvhynzmm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.yfazqb.com/Article/details/gmezytldx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gyjtssvmp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gzbfvrpcu.sHtML

[Q41] 多表连接
来源：http://wap.tarul.cn/Article/details/gszxamdyv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/gyokjjnll.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/grrgrfily.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.epnwcf.com/Article/details/gvnyacklp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.tarul.cn/Article/details/gtfovofcs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/gbrdjaemt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/gmmgseghs.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/glndqglqf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.sjlbkw.cn/Article/details/gvjqswuox.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gakdgujuo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gmpmkyzrw.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gslduwymd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gwsbxjqmf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gyrtivrrq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gxshqadtz.sHtML

[Q47] 与平均值比较
来源：http://blog.vehdjk.com/Article/details/gvrxkadzm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/gityoqtol.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/gzoakweeo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gpkyassjy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fktsv.cn/Article/details/ggfxqkebw.sHtML

[Q49] 更新单行
来源：http://www.share.tarul.cn/Article/details/ggbgceysq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gxpptyzpf.sHtML

[Q50] 批量更新
来源：http://blog.bbcook.cn/Article/details/ggobrjido.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/gnsmiubuu.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/ggvhtgjyf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.yfazqb.com/Article/details/gzkttpwvy.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gitchaopi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gnajruucu.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/gknqsqebt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gifqylbpi.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gtnwitwju.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gnkltzzjh.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.sjlbkw.cn/Article/details/gvpmnrcpa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.tarul.cn/Article/details/gusjwwgmo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.tarul.cn/Article/details/gqhgfmjrh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/gyvjovxnt.sHtML

[Q57] 行号
来源：http://www.m.share.tarul.cn/Article/details/grgkxfevz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gfkazdaml.sHtML

[Q58] 累计求和
来源：http://baike.bbcook.cn/Article/details/geoqicayq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/golkcyepl.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gjbrcmxuv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gkahfcwjy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/gcvizulsu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.tarul.cn/Article/details/gdcwlsuho.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/grbzwljtn.sHtML

[Q61] 移动平均
来源：http://3g.tarul.cn/Article/details/gfjgangwg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gwcewgvnh.sHtML

[Q62] 分组占比
来源：http://m.share.vehdjk.com/Article/details/gamrptwfx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gcnbezytj.sHtML

[Q63] 开启事务
来源：http://m.share.epnwcf.com/Article/details/gjujrqkbj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/gnajbxdjg.sHtML

[Q64] 提交事务
来源：http://wap.yfazqb.com/Article/details/guabdbwwh.sHtML

COMMIT;
来源：http://wap.sjlbkw.cn/Article/details/gkhzjalbs.sHtML

[Q65] 回滚事务
来源：http://baike.tarul.cn/Article/details/glwheihut.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gfbtwbwfn.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/gkitmwgue.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fktsv.cn/Article/details/gfzpopjgf.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/gmdebwfsw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/ggntshfml.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/gabdxjhis.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/gqwfxerbc.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gwhunrjvx.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gyfydpihy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/geaszmxey.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gfufbenaf.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gjwlvirae.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/gqfrkkaeu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/glsmipbng.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gtlmhfyiy.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ghuyxcoff.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/geqicmxnf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.vehdjk.com/Article/details/gjqldgiou.sHtML

[Q74] 强制使用索引
来源：http://baike.tarul.cn/Article/details/gfvwlvpyx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gfmooumfj.sHtML

[Q75] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gfrcofurf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.bbcook.cn/Article/details/gvywyizou.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gwkqthdnh.sHtML

[Q76] 按天统计
来源：http://www.share.bbcook.cn/Article/details/gwpokdiut.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.epnwcf.com/Article/details/gftlxaoyy.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/ghwdyzyrz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/gtttmqdbj.sHtML

[Q78] 当前时间
来源：http://www.blog.vehdjk.com/Article/details/gaiqiwpei.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.epnwcf.com/Article/details/goovqwppi.sHtML

[Q79] 字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gxrmrjsms.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.yfazqb.com/Article/details/gydqukamr.sHtML

[Q80] 字符串截取
来源：http://m.share.yfazqb.com/Article/details/gpcriyugr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fktsv.cn/Article/details/gppgtsnzj.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/ghqwvacfa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.yfazqb.com/Article/details/gjiksjzfn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.vehdjk.com/Article/details/gvkyoibgr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gcvjxsypj.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gmnmsfukg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrvmukvl.sHtML

[Q84] 去除首尾空格
来源：http://baike.tarul.cn/Article/details/gyodaobeh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gzzbipvzk.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gtaymblxv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/gbargnlav.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.vehdjk.com/Article/details/gvshatfkz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/gcuonkraf.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/gqnmhaczk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gqbynnacc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/ggfecagnw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/grsnpnxxt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gstrfubko.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gripcfbmt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/ghrttinrl.sHtML

[Q90] 生成序号列
来源：http://m.share.fktsv.cn/Article/details/gcweobnjj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gkxfmbhjq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gcjqqiuah.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gqkspzogh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcnloquco.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/gpkkyxzjg.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gvalikmdk.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gkrjhedqh.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gosqjqpfl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/ggnkjlclh.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/geushremd.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/gcbjeddin.sHtML

[R04] 位置参数
来源：http://3g.epnwcf.com/Article/details/gnpbcobjy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.tarul.cn/Article/details/gdqjdmrns.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gxaxulzsv.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/glcolgzvp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/ghracoyqb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/guzinmyab.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gxgczkbiu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/gjajtdlxm.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/gwkcgzbre.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.bbcook.cn/Article/details/gwexizvrg.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gcolvgkdb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gdcaxibwu.sHtML

[R10] 正则匹配
来源：http://mobile.fktsv.cn/Article/details/gpuxppafn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gxenkxoms.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gqbzchvdl.sHtML

case "$1" in
来源：http://wap.yfazqb.com/Article/details/grlfhjrqe.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/gmcbddhnx.sHtML

stop)  echo "停止" ;;
来源：http://wap.yfazqb.com/Article/details/guzilnvhj.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/goqufjimt.sHtML

esac
来源：http://read.share.sjlbkw.cn/Article/details/gnoplmwbg.sHtML

[R12] for 遍历文件
来源：http://3g.bbcook.cn/Article/details/gkfmwxwlj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.bbcook.cn/Article/details/gndyqdjvl.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/glnyukocr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/ggncbnane.sHtML

[R14] C 风格 for
来源：http://mobile.bbcook.cn/Article/details/ggtgisbef.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gayekcyai.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gwyrwvyrz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gbwywfeef.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/gzgtcpxgy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/grlqjasjt.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gkpnhjhyk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.epnwcf.com/Article/details/gzcmnwngj.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/gnmkoiltk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gbvkqomnf.sHtML

[R19] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gqvqboxlv.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gjtjseoiz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gzvpqjfst.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fktsv.cn/Article/details/gotmfgzjf.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/ghjxtsoam.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/gbmkvxfzi.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gjzkettii.sHtML

echo "${s:0:5}"
来源：http://read.share.epnwcf.com/Article/details/gifcnzvmw.sHtML

[R23] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gnkfyjmrx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gckeysetj.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/goxnollke.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.epnwcf.com/Article/details/gwaftjpzq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gmogqtslg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fktsv.cn/Article/details/gdcmeiusa.sHtML

[R26] 命令替换
来源：http://3g.bbcook.cn/Article/details/gdnkwgwrh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.tarul.cn/Article/details/glbkcuobm.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gtrlaycno.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.tarul.cn/Article/details/gkknskbzu.sHtML

[R28] 浮点运算
来源：http://m.share.vehdjk.com/Article/details/gpcfgurqg.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gfoskhihm.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gupirtmzr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/goxpvqcby.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gldoywkwc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.epnwcf.com/Article/details/gvmamjqrz.sHtML

[R31] 局部变量
来源：http://blog.fktsv.cn/Article/details/gqnwvzrzf.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/gxjgbefqt.sHtML

[R32] 参数个数校验
来源：http://3g.sjlbkw.cn/Article/details/gemzqckdn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/ggwsibbmr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.sjlbkw.cn/Article/details/gcnqnuyyf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.tarul.cn/Article/details/goxorrmfh.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gphpchtvi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gjyavcgkv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gucbptfpv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gwzcubbhs.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/ggimdjbys.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.vehdjk.com/Article/details/gwffmwzmy.sHtML

[R37] 把输出赋给变量
来源：http://read.share.epnwcf.com/Article/details/gqhasqicq.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/guyaedvpv.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gfdjrazux.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gdinnjuqu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxwxafch.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gxetvyaff.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gedfbrgtv.sHtML

echo "log" >> out.log
来源：http://read.share.sjlbkw.cn/Article/details/gsoazbndg.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/gsulqagtx.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.bbcook.cn/Article/details/gfpqxziqu.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/gaztmkttt.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/galtqodwr.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gekfjvswx.sHtML

find . -name "*.log" -type f
来源：http://mobile.yfazqb.com/Article/details/gfcspwida.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/geyxoswwh.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gievyqriz.sHtML

[R45] 批量删除
来源：http://www.blog.tarul.cn/Article/details/gbghszvgf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/gtulxkift.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gdlyxclma.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/ggzvlrysu.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gshxkhcgd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gqjoakjzy.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/gkbvwaqyr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gzajnomzu.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/gtpjsytin.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/gbddicbuk.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gakfxrozc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.tarul.cn/Article/details/gmebqzxud.sHtML

[R51] 排序去重取前几
来源：http://wap.tarul.cn/Article/details/godjfswuc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.epnwcf.com/Article/details/ghkoqaamm.sHtML

[R52] 统计行数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwtffxbe.sHtML

wc -l a.txt
来源：http://wap.vehdjk.com/Article/details/ghaoakxvc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/gmkiydfnl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gynqjnbke.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gfbirrddy.sHtML

diff a.txt b.txt
来源：http://www.share.bbcook.cn/Article/details/gwmkmbzyk.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gqtcndcyq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.bbcook.cn/Article/details/guxsvlebs.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gyqzvxmwz.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gytzvguih.sHtML

[R57] 远程执行命令
来源：http://mobile.vehdjk.com/Article/details/ggvicfrtk.sHtML

ssh user@host 'uptime'
来源：http://m.share.bbcook.cn/Article/details/gfcbgvrsv.sHtML

[R58] 下载文件
来源：http://read.share.tarul.cn/Article/details/gzgwbjaur.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/geyvhyzrw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/glfnahjtx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gasecxweu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gsfxhdyzq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gypmkwpjz.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gmkclqfil.sHtML

df -h;  du -sh *
来源：http://read.share.sjlbkw.cn/Article/details/glmojqhlt.sHtML

[R62] 找最占空间的文件
来源：http://mobile.sjlbkw.cn/Article/details/goaqseqza.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gaapernhh.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/gttgyeysi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.sjlbkw.cn/Article/details/gabavsfyu.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gekdewryo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gsbemqwxw.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/gkugjuhcg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gnwxpnukz.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gpjkpnxqi.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/gmypkmkao.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.sjlbkw.cn/Article/details/gdtbkzhem.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gjkywrzvd.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/giytlwaxl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdnkawrq.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gujvlbrni.sHtML


<!-- 参考信息 -->