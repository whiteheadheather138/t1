代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/gxejfuidj.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/gwofshbef.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gmbkidfll.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/guqmuegsu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.bbcook.cn/Article/details/grcgqrhjp.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gmroazdyr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/gppipicfl.sHtML

[Q21] 空值判断
来源：http://3g.tarul.cn/Article/details/gyhatlshs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/gjaxrjumf.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gbkxwzsby.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.yfazqb.com/Article/details/gkyiqzqro.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/gcgalgwal.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.bbcook.cn/Article/details/getbjdtds.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/gxvvhzltu.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gheplkutr.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.epnwcf.com/Article/details/gftzchuam.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/gobdqvwbg.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gyjzdotzo.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.epnwcf.com/Article/details/gmvysrhwg.sHtML

[Q27] 条件计数
来源：http://read.share.yfazqb.com/Article/details/ggmswmuzo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/gbzjgziyk.sHtML

[Q28] 求和与平均
来源：http://www.blog.yfazqb.com/Article/details/goqvusjxk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gfdywbwqy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gqqogjvim.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/glkfxyfvu.sHtML

[Q30] 分组统计
来源：http://3g.tarul.cn/Article/details/gbeufvryk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gvgmywldk.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/gkezaqzqf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/ggbdbeeoi.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gjbdvgwmo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/ghbyxsaow.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/gnfkhyihx.sHtML

[Q33] 多列分组
来源：http://baike.yfazqb.com/Article/details/garmfuaco.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.sjlbkw.cn/Article/details/gokcrpqfy.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/gqaajnnvz.sHtML

SELECT * FROM (
来源：http://www.share.bbcook.cn/Article/details/gjitsdvst.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.epnwcf.com/Article/details/gqpziztcc.sHtML

) t WHERE rn = 1;
来源：http://mobile.sjlbkw.cn/Article/details/guxlaslvb.sHtML

[Q35] 内连接
来源：http://3g.bbcook.cn/Article/details/gsklovjhk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gyiwnewdb.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gznwdnegp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gtfybcvhi.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/gdshdxfvq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.bbcook.cn/Article/details/gvoyzjcya.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.vehdjk.com/Article/details/gtstkxutq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.epnwcf.com/Article/details/gtgiiihei.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.sjlbkw.cn/Article/details/gqlxaetjg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gbdibhgtl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gulbfbrhc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/goiodqwfb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/gajxgyitg.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/gglcqjtrz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.bbcook.cn/Article/details/gowfsgpff.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/gpsqyzdde.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.epnwcf.com/Article/details/gsbjgcpzg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gvxkumsum.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gmhuptoxm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fktsv.cn/Article/details/gdbdmecvy.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gpylprkom.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fktsv.cn/Article/details/gmqwqljxg.sHtML

[Q44] IN 子查询
来源：http://mobile.tarul.cn/Article/details/gjnsxdbzi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/gdmzbpdqj.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/glsztsyky.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gguvcnmdq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gpzypbqzy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gloistuho.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.tarul.cn/Article/details/gfchfhmwz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gfevcfijz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.yfazqb.com/Article/details/ganlpppon.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.tarul.cn/Article/details/gafhrqqru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gwmxjaqxm.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gnuyphglm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/ggyejhhux.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/glcaschlx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gmmbdphwc.sHtML

[Q51] 用子查询更新
来源：http://www.share.bbcook.cn/Article/details/gatxthiym.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/gfuiyzkkz.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gtcwbjtbd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gjyfnuimi.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/gsdocjylo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gzuzdugip.sHtML

[Q54] 清空表
来源：http://www.m.share.yfazqb.com/Article/details/glrcolodc.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gvuipbmdh.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.tarul.cn/Article/details/gbwdvuzvk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gfsmcfrtd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/gokynpolj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.tarul.cn/Article/details/gwfmzauvk.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/ggiuzxvir.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gljtzdsvp.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gxsjedovj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/gqqnxxpus.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gwdukwlio.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gxqmbrrep.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/gngmihxjx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.yfazqb.com/Article/details/gkseizdrr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gldrpewsn.sHtML

[Q61] 移动平均
来源：http://wap.tarul.cn/Article/details/gnvtszvif.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gjhtzlblr.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gfveddzsm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gyzrdkvey.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gobfolome.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/ggdtwzygl.sHtML

[Q64] 提交事务
来源：http://mobile.vehdjk.com/Article/details/gybqemdrk.sHtML

COMMIT;
来源：http://mobile.vehdjk.com/Article/details/gpkuhnydq.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/gbalyrbva.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/gdliddbew.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/ggleydhmq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fktsv.cn/Article/details/gyvlnczml.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.yfazqb.com/Article/details/gtoyoyrsh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/ginbdnont.sHtML

[Q68] 保存点
来源：http://wap.epnwcf.com/Article/details/gykgfoypt.sHtML

SAVEPOINT sp1;
来源：http://blog.sjlbkw.cn/Article/details/gjwsopwdr.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/gdrfrmlrh.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gnwqjqzvi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gjxfuxipl.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fktsv.cn/Article/details/gflbgbbjs.sHtML

ANALYZE TABLE users;
来源：http://read.share.fktsv.cn/Article/details/geekmelxl.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.bbcook.cn/Article/details/gwjpdbcqh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.bbcook.cn/Article/details/gdbyzcuus.sHtML

[Q72] 查看索引
来源：http://m.share.epnwcf.com/Article/details/gscscabni.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ghwkwfnhg.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/ggdsokqsl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gpeijeoal.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gohzfpltm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.bbcook.cn/Article/details/gatgduzju.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gbgsuvgqv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/glkukbdyz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gbxbndljx.sHtML

[Q76] 按天统计
来源：http://wap.sjlbkw.cn/Article/details/gibkkgdyi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/gftvccjga.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gyefnkwtx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/ghlufqskx.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/gtcivyfmj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fktsv.cn/Article/details/gsecvrayi.sHtML

[Q79] 字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gxdrcsguj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gmvxrbohs.sHtML

[Q80] 字符串截取
来源：http://baike.epnwcf.com/Article/details/giozyrvzb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.epnwcf.com/Article/details/gzxietkpp.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gqjzmzzgh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/gbtptotie.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.tarul.cn/Article/details/gapkbjtcg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gfxjioqqj.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gvljvtkpb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gnmolrifp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/gkngaewvk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gvlrzmrdl.sHtML

[Q85] 数值取整
来源：http://www.share.tarul.cn/Article/details/gfwvayzsj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.bbcook.cn/Article/details/ggbhsirkt.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/gvojbyfya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/goyzijswg.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.epnwcf.com/Article/details/gtcybnnpy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.tarul.cn/Article/details/gzvbyzejf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gwcnuspki.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fktsv.cn/Article/details/gtoprguab.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gcywaclrk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gkxnxuvvc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gxhffmacy.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gmriwacus.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.yfazqb.com/Article/details/gloxslyyz.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvqqxsgqh.sHtML

R. Bash 专题
来源：http://www.share.sjlbkw.cn/Article/details/gltcgjmhi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdpzfqigq.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gvebkewlv.sHtML

#!/usr/bin/env bash
来源：http://blog.epnwcf.com/Article/details/gbntexgxr.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gnsceplfc.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gcpocnxdv.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/gwhxstsdf.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gkfigdzsy.sHtML

readonly PI=3.14
来源：http://www.blog.yfazqb.com/Article/details/gtdoxjmtw.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/gcjdjoqje.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/gpbhktqor.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/gjezhbnfo.sHtML

name="${1:-default}"
来源：http://read.share.yfazqb.com/Article/details/gujyabwnp.sHtML

[R06] 判断命令是否存在
来源：http://blog.sjlbkw.cn/Article/details/ghoxckvwr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gyvejfguf.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/ggkqhowkv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/gvxvcabmd.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gphorhgwi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.tarul.cn/Article/details/gdxotzoam.sHtML

[R09] 字符串比较
来源：http://wap.tarul.cn/Article/details/gdajjpbre.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gjedybnhl.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/gkcdkedmf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnavrxht.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gotaohbjn.sHtML

case "$1" in
来源：http://m.share.tarul.cn/Article/details/gwpdngyrm.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gtzyezmax.sHtML

stop)  echo "停止" ;;
来源：http://blog.bbcook.cn/Article/details/gbcmarwvw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.bbcook.cn/Article/details/gxoutbclp.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gcvhewopx.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gwzziooxc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gjmllrcoe.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gpmnthqxf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gqznbjxrd.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/gimyccwjn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gifjgfhtk.sHtML

[R15] while 逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/glkpcvljb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/gbctdedfe.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gcaosxvhh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gjkdjhbwx.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/grjjfiozm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.vehdjk.com/Article/details/glusuljha.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gouizxtbw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.epnwcf.com/Article/details/gxrrqkdqr.sHtML

[R19] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/gebefnqeu.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gafxtrdcx.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gehzemojf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/givmgjlet.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/giiodrbpr.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gopxtkbbx.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/gjftyslmt.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gvetkvbpq.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gjsiquave.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.epnwcf.com/Article/details/gmndyghkl.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/grzasepxc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/goamassos.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.sjlbkw.cn/Article/details/gchceavea.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/govcykznb.sHtML

[R26] 命令替换
来源：http://read.share.epnwcf.com/Article/details/geqoefywa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.epnwcf.com/Article/details/gpromxcpm.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gbhnnrmpn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/gyrtdrbmo.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/gmmjvbpgh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.epnwcf.com/Article/details/gkhlelqnd.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/glznszjzr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gopxnstda.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/glfzsadyt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gokemimyn.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/gwpcterzf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gnvccunne.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gyfncfpjp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gfeijkhhs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.sjlbkw.cn/Article/details/gugnrlwvk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.bbcook.cn/Article/details/gaowhfpit.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gchxotvmd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gctqgkmjj.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gfcjqkqat.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/gkyxhykyz.sHtML

[R36] 并发执行多个任务
来源：http://3g.vehdjk.com/Article/details/gzcxatnnr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gdjxwptkw.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/giewnpczl.sHtML

files=$(ls -1)
来源：http://read.share.epnwcf.com/Article/details/gyoqrcgrx.sHtML

[R38] 管道串联
来源：http://3g.epnwcf.com/Article/details/gdejxzgej.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/ggqkkfryb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.vehdjk.com/Article/details/gqplhanwn.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/gvxthvcak.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gktrmodbo.sHtML

echo "log" >> out.log
来源：http://m.share.bbcook.cn/Article/details/gkynyxiog.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gxlzzmlix.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/gjtnkzcub.sHtML

[R42] 输入重定向
来源：http://wap.sjlbkw.cn/Article/details/gwppdqrzp.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/gipqwshwh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/ghzqyadlj.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gmkdxkqpn.sHtML

[R44] 按修改时间查找
来源：http://baike.epnwcf.com/Article/details/gjcxuldeg.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.vehdjk.com/Article/details/ginegqqzs.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gpamseqsw.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gfovpkxwp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.bbcook.cn/Article/details/gizeueqya.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fktsv.cn/Article/details/gjxgpksrz.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gzpusdvga.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gbpsvgmls.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/gfddhwfye.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.tarul.cn/Article/details/ghezytydk.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/giynedshz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/gxlsnvcor.sHtML

[R50] awk 求和
来源：http://www.m.share.vehdjk.com/Article/details/gexchatko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gppqztuzg.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gclmeufle.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gfmrlfzwm.sHtML

[R52] 统计行数
来源：http://www.share.epnwcf.com/Article/details/gkmtkvjzb.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gmhmwvgzs.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/gljajymrd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/ghduxbeuy.sHtML

[R54] 比较两个文件
来源：http://read.share.bbcook.cn/Article/details/gwnhrbcqv.sHtML

diff a.txt b.txt
来源：http://wap.epnwcf.com/Article/details/gtbkokkxz.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/grxnylzco.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.bbcook.cn/Article/details/gcahaubel.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gregsokge.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gmavcyyja.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/glogcxwck.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gfblsxiuz.sHtML

[R58] 下载文件
来源：http://wap.bbcook.cn/Article/details/guflkhzpf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gyxfsxuuc.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/guktuxpbo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/gbvadhynq.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gkndtlruc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gzbehgidw.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gfukxpxck.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/galqjlcpi.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gqidhyupi.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/gelmndkev.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/gkyklassq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/gpyhgufdj.sHtML

[R64] 结束进程
来源：http://read.share.yfazqb.com/Article/details/ggsazofke.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fktsv.cn/Article/details/gozrpjxsw.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/gejmwsbhv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gcjnldbzo.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/gcnqwguec.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gxofsjrgr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.sjlbkw.cn/Article/details/gpzmdpvon.sHtML


<!-- 参考信息 -->