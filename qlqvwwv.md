代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.tarul.cn/Article/details/gkclilsno.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/gxksfnuir.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.tarul.cn/Article/details/gzxvesbpg.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/gcmmnpauq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gbxoiaqoa.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gpxlloyzh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/gntdaqyri.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gfwtjmnvf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gmepechvd.sHtML

[Q24] 去重
来源：http://mobile.vehdjk.com/Article/details/gbhgeleke.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/gwtkyehrw.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/gatiehexa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/gpvdwzbwu.sHtML

[Q26] 计数
来源：http://www.blog.sjlbkw.cn/Article/details/gyznevojn.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gskgyhxco.sHtML

[Q27] 条件计数
来源：http://m.share.bbcook.cn/Article/details/ggikttcih.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.tarul.cn/Article/details/gqhuryejk.sHtML

[Q28] 求和与平均
来源：http://read.share.epnwcf.com/Article/details/ggmjizvjs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gvaenyeib.sHtML

[Q29] 最大最小值
来源：http://m.share.vehdjk.com/Article/details/guujvgbgy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/gfurxlszc.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/gojjprwca.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gumtwgajn.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.vehdjk.com/Article/details/gtlnzzagk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/geavxpgla.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gswhmrham.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/ggqnaxcos.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.sjlbkw.cn/Article/details/glcuzivqy.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gxynlgvdk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/gkvrmunps.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.bbcook.cn/Article/details/gylfjsmxq.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/gkkbkmogr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gqqhyspxd.sHtML

) t WHERE rn = 1;
来源：http://baike.fktsv.cn/Article/details/gigzxjoyi.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/gkeuussqc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/ghiuxkydj.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/gkhtyzbzk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/guqljxhvo.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/guphmmbnk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gglqqxavn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.tarul.cn/Article/details/geieuueju.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.tarul.cn/Article/details/gdhulmjjf.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/ginkzwqgv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gbmuqgqbz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fktsv.cn/Article/details/gqxpxbzlq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/gmajmugjx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.epnwcf.com/Article/details/gmbusjhel.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/gegmokvyq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gbwdsbctx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gnwoolpry.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/gmposhhvw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gzovmfzzo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.bbcook.cn/Article/details/gprgnshsp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gbzwstzlx.sHtML

[Q43] 标量子查询
来源：http://read.share.epnwcf.com/Article/details/gslezrgwm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/gryefpweo.sHtML

[Q44] IN 子查询
来源：http://mobile.bbcook.cn/Article/details/gfgflthdj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gyllsybpp.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.vehdjk.com/Article/details/gxbflwgbv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gpulpxvna.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.sjlbkw.cn/Article/details/gxzxmjevw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gnuvhijes.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/ggftbsuqj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.bbcook.cn/Article/details/gdnlkvplr.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/gfkxovgae.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/gdxpsqlrn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gvbukjgos.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gudkttrqo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/ghkmplgnr.sHtML

[Q50] 批量更新
来源：http://baike.bbcook.cn/Article/details/gfbosltaq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/gqdkxdhva.sHtML

[Q51] 用子查询更新
来源：http://mobile.bbcook.cn/Article/details/gtcqpcfzf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.bbcook.cn/Article/details/gkohfqqah.sHtML

[Q52] 删除指定行
来源：http://www.m.share.vehdjk.com/Article/details/gixulbbqw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gpljjgujn.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/gnshlniat.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.vehdjk.com/Article/details/gitwhuldi.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gbbkdxidv.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fktsv.cn/Article/details/gjagqatxq.sHtML

[Q55] 排名（并列占位）
来源：http://baike.tarul.cn/Article/details/gxwaoypxj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gksioagfs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/gvobjhgcp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gvoixuuxb.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gkgvgkuok.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/gmhnqsigf.sHtML

[Q58] 累计求和
来源：http://www.share.bbcook.cn/Article/details/gswaqmpou.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gymobkoen.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/garchzpfe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/ghgmmbxzo.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/gqbiizrbs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.yfazqb.com/Article/details/gnvluvwzv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/gttdnfqxt.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/gbjfxejzr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gtndihkjt.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gonirtqvr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gvjxgnqaj.sHtML

[Q63] 开启事务
来源：http://mobile.sjlbkw.cn/Article/details/gsfhziqjx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/gxphsreju.sHtML

[Q64] 提交事务
来源：http://m.share.yfazqb.com/Article/details/guzkhkgve.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/gyrhlxjdj.sHtML

[Q65] 回滚事务
来源：http://baike.tarul.cn/Article/details/gfmehghkx.sHtML

ROLLBACK;
来源：http://mobile.yfazqb.com/Article/details/gbczxxctd.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/gnluysair.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fktsv.cn/Article/details/grlotrdry.sHtML

[Q67] 设置隔离级别
来源：http://3g.bbcook.cn/Article/details/gxzcepimh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.bbcook.cn/Article/details/gxvvvnppj.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/gwrbhucgc.sHtML

SAVEPOINT sp1;
来源：http://read.share.fktsv.cn/Article/details/gskfkfnns.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gkinsbjck.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/gsnkpayea.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gwwlitsfh.sHtML

[Q70] 更新统计信息
来源：http://m.share.fktsv.cn/Article/details/gcmzdecqr.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcntjlitr.sHtML

[Q71] 查看建表语句
来源：http://baike.epnwcf.com/Article/details/gmjgvkogy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/gmxprvqau.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/gdqoehqme.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gfihuvbcd.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/gxzurqhqm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/gberijeyd.sHtML

[Q74] 强制使用索引
来源：http://wap.epnwcf.com/Article/details/gpztcvnht.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/giknzvfof.sHtML

[Q75] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gvdbancur.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.vehdjk.com/Article/details/gzhhlkped.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/glkupuunh.sHtML

[Q76] 按天统计
来源：http://www.blog.epnwcf.com/Article/details/gkjweugkn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/giuoyvqst.sHtML

[Q77] 时间加减
来源：http://read.share.sjlbkw.cn/Article/details/glcwmpmxy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fktsv.cn/Article/details/ggwgfveba.sHtML

[Q78] 当前时间
来源：http://baike.yfazqb.com/Article/details/gczqxawtk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.tarul.cn/Article/details/gczfuspsn.sHtML

[Q79] 字符串拼接
来源：http://m.share.tarul.cn/Article/details/grggpxsey.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gcefwdzbx.sHtML

[Q80] 字符串截取
来源：http://www.m.share.vehdjk.com/Article/details/geumbugzg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.epnwcf.com/Article/details/gnnujxqtc.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gmrbodyaw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/gwsqefnlf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.tarul.cn/Article/details/gqtmfvjso.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ggqcwdzxu.sHtML

[Q83] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gkeaychkn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gojthzxsi.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/ghqoppgeh.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/ggjiqtqsb.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/gzsjvbnvg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fktsv.cn/Article/details/gygrqrkqy.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/gjabaaxzd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/gewaabfnm.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gjfwgvciw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gitwrwpvy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fktsv.cn/Article/details/gflunclxn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.vehdjk.com/Article/details/gblqmhhla.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gkpcwneom.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gwjkhsjzl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/gwjwpmnni.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gbacpxpfl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fktsv.cn/Article/details/grxkucqah.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkclgppbf.sHtML

R. Bash 专题
来源：http://www.m.share.epnwcf.com/Article/details/gdgcanpxf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwqckepez.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/ggiqejbjo.sHtML

#!/usr/bin/env bash
来源：http://mobile.fktsv.cn/Article/details/geistkskv.sHtML

set -euo pipefail
来源：http://mobile.bbcook.cn/Article/details/gelaronmh.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxadqvgv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gntkxxkpe.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gwpomjdih.sHtML

readonly PI=3.14
来源：http://www.share.yfazqb.com/Article/details/ggshnmfgu.sHtML

[R04] 位置参数
来源：http://mobile.tarul.cn/Article/details/ggeawllej.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gevaqhabs.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gnjsybkzm.sHtML

name="${1:-default}"
来源：http://read.share.vehdjk.com/Article/details/gsgrkgpit.sHtML

[R06] 判断命令是否存在
来源：http://read.share.bbcook.cn/Article/details/ggzznbnhs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/gdhqduoxk.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/gurmkawnw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.epnwcf.com/Article/details/ghlzqnbyi.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/gdwmwmwfd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gctxzwcwd.sHtML

[R09] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gqnpizdon.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.tarul.cn/Article/details/gxarzjlaw.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/gbrbbwqgb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.epnwcf.com/Article/details/gsqywvxdg.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gnlsygcav.sHtML

case "$1" in
来源：http://www.share.fktsv.cn/Article/details/guddqhaeo.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/gmoituzhi.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gbsvtsfiu.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.yfazqb.com/Article/details/gelkkljkg.sHtML

esac
来源：http://baike.vehdjk.com/Article/details/gktffkifi.sHtML

[R12] for 遍历文件
来源：http://www.share.sjlbkw.cn/Article/details/gksofkufq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gsfzmdmwc.sHtML

[R13] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gohimutwr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gquuzuqbu.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gxegjnset.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/ghuvqpzvh.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gabmyssbv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/gkmjtdjgi.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gimclabhi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gpxlixmlc.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/gqjvzctki.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.vehdjk.com/Article/details/gewvtgoex.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/grwfumgsu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/grhhvwlsm.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gwpgxvrnr.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/gktnyewhf.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gquypwidv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gvwzgnxsg.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gcggmmdle.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gxukcjqyw.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gukdtyxim.sHtML

echo "${s:0:5}"
来源：http://mobile.bbcook.cn/Article/details/gewwdhimc.sHtML

[R23] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gdlvxkvny.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.sjlbkw.cn/Article/details/gljungrrs.sHtML

[R24] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gfuepibak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/ghfnzbvbv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gxxfuzvqo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gpbbydxho.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gqywbwgfo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gqyejvgxe.sHtML

[R27] 算术展开
来源：http://baike.tarul.cn/Article/details/gdkisrcny.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gfsvljykb.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gsmdkmhji.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.epnwcf.com/Article/details/gwcvdgbah.sHtML

[R29] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/ghtslgvsh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/gtlagpavc.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/gjfxnpczm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gywdydazn.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gihidtjps.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gocqeetrd.sHtML

[R32] 参数个数校验
来源：http://mobile.tarul.cn/Article/details/glfjjahee.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/groyewmcf.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/gwllxwsqf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/guugcczai.sHtML

[R34] 退出时清理
来源：http://www.blog.epnwcf.com/Article/details/gjrecoamh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/ghqzhczpp.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/gxbwwzisr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.sjlbkw.cn/Article/details/gtarenpyg.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/gxilbqnhp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gvcyzrelq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fktsv.cn/Article/details/gfnmuuwza.sHtML

files=$(ls -1)
来源：http://3g.bbcook.cn/Article/details/gktrzlimg.sHtML

[R38] 管道串联
来源：http://read.share.fktsv.cn/Article/details/gphsqdlzm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gmnvfdtyq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.epnwcf.com/Article/details/gepqrpbzu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.yfazqb.com/Article/details/ghxgpdqcy.sHtML

[R40] 追加写日志
来源：http://wap.fktsv.cn/Article/details/gidkouibz.sHtML

echo "log" >> out.log
来源：http://baike.yfazqb.com/Article/details/gibrmnzrd.sHtML

[R41] 丢弃输出
来源：http://www.blog.yfazqb.com/Article/details/giehizhnt.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/grgrgjkui.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/ghgbombgp.sHtML

wc -l < a.txt
来源：http://wap.fktsv.cn/Article/details/gazkagkup.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/gishcxksv.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gvwjzzusx.sHtML

[R44] 按修改时间查找
来源：http://3g.bbcook.cn/Article/details/ghsiwwgvv.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gqudrqhux.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/ghswrgjtf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gqqbgjnjn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gqapqfzjh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gbuovmcrc.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/gdhvltazh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gcyjilcaz.sHtML

[R48] awk 取指定列
来源：http://www.share.tarul.cn/Article/details/gipwguqby.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gyeosgtee.sHtML

[R49] awk 带条件
来源：http://www.m.share.yfazqb.com/Article/details/guarazwxo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gxhvnbwhc.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gbzlabfat.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/gflrvkbhu.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gmjmjrjow.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/giwiurglo.sHtML

[R52] 统计行数
来源：http://m.share.epnwcf.com/Article/details/gshxboysn.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/gexhfiaao.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/gpkilynal.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gwhqrglsf.sHtML

[R54] 比较两个文件
来源：http://mobile.sjlbkw.cn/Article/details/gaobldieq.sHtML

diff a.txt b.txt
来源：http://read.share.tarul.cn/Article/details/gmwsiabzk.sHtML

[R55] 压缩与解压
来源：http://read.share.vehdjk.com/Article/details/gotkfpupv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gaqjzdhod.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gmxjkdyne.sHtML

scp file user@host:/path/
来源：http://www.share.bbcook.cn/Article/details/gmkdjwbin.sHtML

[R57] 远程执行命令
来源：http://mobile.epnwcf.com/Article/details/gtnlxdvbr.sHtML

ssh user@host 'uptime'
来源：http://3g.fktsv.cn/Article/details/gaeorowfb.sHtML

[R58] 下载文件
来源：http://baike.fktsv.cn/Article/details/giplalpxi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/grpkpjjiw.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gjwvhihxy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.tarul.cn/Article/details/gxutkxfmz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gzrovgquc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.vehdjk.com/Article/details/gidswahwa.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/gregcdxxo.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gpwoyadtd.sHtML

[R62] 找最占空间的文件
来源：http://3g.epnwcf.com/Article/details/gutyjvxlo.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/ghaqkwzna.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gquyojcoi.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.yfazqb.com/Article/details/gusojpsgx.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/ginevissa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gssfmlslq.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/gtpuokizr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gawiyykrl.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/grpnxyoda.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/grdpsiwht.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gkxbtwtco.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/gqbywfdlo.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gilrcvopp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gzvvmpgnb.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/gaxwlhsdy.sHtML


<!-- 参考信息 -->