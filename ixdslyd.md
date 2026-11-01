代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.bbcook.cn/Article/details/gypoisimj.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/gapmpjtoz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.epnwcf.com/Article/details/goblavggk.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gzgsqwrzv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fktsv.cn/Article/details/gjzjogrey.sHtML

[Q22] 排序
来源：http://mobile.epnwcf.com/Article/details/gxuajbbux.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gxalzgmve.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/gwnvigfte.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.tarul.cn/Article/details/gozxcgaol.sHtML

[Q24] 去重
来源：http://read.share.vehdjk.com/Article/details/ghzntbtih.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/gzqurxpqq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gqeswxihq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/grtwxortp.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/gtrlqyxtv.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/gpoewbqnq.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gosdjmgbk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/gexystjit.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/gvpersywi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gjsvonqig.sHtML

[Q29] 最大最小值
来源：http://wap.fktsv.cn/Article/details/gonlmnukj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/ghmdyjpgq.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/gxzlcvdpq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gnbmdcvko.sHtML

[Q31] 分组后过滤
来源：http://mobile.tarul.cn/Article/details/gjcxakyfo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/gzfdlfwwv.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gmjqppspf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gvhlnhlmu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/gqmtlnvsd.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/gghbnniib.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.sjlbkw.cn/Article/details/gwdvdpgvt.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gynzcmhhm.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/gsizwmyor.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/gfnpadzyu.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/gumzdzhlt.sHtML

[Q35] 内连接
来源：http://baike.sjlbkw.cn/Article/details/gvovgjtcx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/gptjskgxb.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/gyvrbxpmg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gmzxsywzj.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gbklxmqox.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fktsv.cn/Article/details/ghbihljxl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gmfaqnfxw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/grotwceqr.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.bbcook.cn/Article/details/goqgpglso.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.bbcook.cn/Article/details/gcfgnackc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gxwpeuxyd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gnevscihz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gjsnokhzh.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gztzshngs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gytcjobyj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/gvviyhqqz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.bbcook.cn/Article/details/gamasowvl.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gbdybczqi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gdnmaeyml.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gkucrsezs.sHtML

[Q43] 标量子查询
来源：http://baike.yfazqb.com/Article/details/gtervrgxb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.tarul.cn/Article/details/guhyckais.sHtML

[Q44] IN 子查询
来源：http://wap.vehdjk.com/Article/details/gddsrxclv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/giqiykoep.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.tarul.cn/Article/details/gaucinply.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gmiqylnso.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.yfazqb.com/Article/details/gjcieejij.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/glvevrqut.sHtML

[Q47] 与平均值比较
来源：http://wap.fktsv.cn/Article/details/gdxlvxztn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.vehdjk.com/Article/details/glkqtuuie.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/gglyqhptk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gjvszxkay.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gykahibex.sHtML

[Q49] 更新单行
来源：http://read.share.vehdjk.com/Article/details/gktdfdeey.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/grxbzmofy.sHtML

[Q50] 批量更新
来源：http://www.share.fktsv.cn/Article/details/gbqccrfud.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gizencnxv.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gfxtwzuid.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/gqlpauzvi.sHtML

[Q52] 删除指定行
来源：http://read.share.tarul.cn/Article/details/gkcmzgdok.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gmwbuyptq.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gojpvfvba.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gkgufflws.sHtML

[Q54] 清空表
来源：http://3g.epnwcf.com/Article/details/gyqifyoev.sHtML

TRUNCATE TABLE logs;
来源：http://blog.tarul.cn/Article/details/gvohgntut.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.vehdjk.com/Article/details/gfadufxct.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gsnngesnj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.sjlbkw.cn/Article/details/gdtxdqica.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/gasejfzfl.sHtML

[Q57] 行号
来源：http://www.m.share.tarul.cn/Article/details/gkfudvmhj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/gtvikvxfp.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/ghwskyvsd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gzjcjyzza.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/ghmsjldza.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gfnkhorkr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gczxbwmta.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.sjlbkw.cn/Article/details/gbfyftdbv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gnupfdwtm.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gtadjqcgd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gfnvtybws.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/ghifenarl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gzaspydxh.sHtML

[Q63] 开启事务
来源：http://baike.sjlbkw.cn/Article/details/gmrrqcfqs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.yfazqb.com/Article/details/gvrewtpxx.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/ggnqctlma.sHtML

COMMIT;
来源：http://read.share.sjlbkw.cn/Article/details/giwcyoesu.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gquxlghvt.sHtML

ROLLBACK;
来源：http://mobile.tarul.cn/Article/details/gfjonblbh.sHtML

[Q66] 行锁查询
来源：http://read.share.epnwcf.com/Article/details/gxzzqnusv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/geekclbnh.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gyfdujags.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.tarul.cn/Article/details/gjeifjkzp.sHtML

[Q68] 保存点
来源：http://read.share.bbcook.cn/Article/details/grtlprwpk.sHtML

SAVEPOINT sp1;
来源：http://mobile.yfazqb.com/Article/details/gxxcxskyl.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.epnwcf.com/Article/details/gohvjufxu.sHtML

[Q69] 查看执行计划
来源：http://www.blog.tarul.cn/Article/details/gnfzlzfby.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/gqvlprxab.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.bbcook.cn/Article/details/gctudoxmb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/gmjwabloi.sHtML

[Q71] 查看建表语句
来源：http://www.share.bbcook.cn/Article/details/gpxujvenc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.sjlbkw.cn/Article/details/gndbhfgkg.sHtML

[Q72] 查看索引
来源：http://www.blog.tarul.cn/Article/details/ggzjvmjeq.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/gjdbkrhcp.sHtML

[Q73] 查看表状态
来源：http://blog.epnwcf.com/Article/details/gfjhnxcis.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.bbcook.cn/Article/details/gjrmnvbro.sHtML

[Q74] 强制使用索引
来源：http://www.blog.sjlbkw.cn/Article/details/gbsdrdfut.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.sjlbkw.cn/Article/details/gswzxalxb.sHtML

[Q75] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gfesiqsyg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gfcjrkcid.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/giwjburvv.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/gofxiqanm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.epnwcf.com/Article/details/genljhcry.sHtML

[Q77] 时间加减
来源：http://www.share.bbcook.cn/Article/details/gnrvfozbr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/glqlltmnl.sHtML

[Q78] 当前时间
来源：http://read.share.epnwcf.com/Article/details/grhulicqk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/ggricgsdq.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gkjoxgaex.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/ggssiagol.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/gahayixpj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gncqcatlq.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gsnjlsayi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.vehdjk.com/Article/details/gcamptkiq.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.epnwcf.com/Article/details/gnycjeqxk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gkxymupvx.sHtML

[Q83] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gmftwkddm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gkukzlfaj.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/goufsjxrl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gpkoyezwx.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gefzopbzy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gwzdmnnen.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.epnwcf.com/Article/details/grcthlmzn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gkommzalk.sHtML

[Q87] JSON 字段做条件
来源：http://blog.epnwcf.com/Article/details/gmlkhtsed.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gggpljbvq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gacwitedw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.vehdjk.com/Article/details/gwvwrloic.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/ggbrzfzkp.sHtML

[Q89] 判断表是否存在
来源：http://wap.yfazqb.com/Article/details/gnkwslfbd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/gomsixfgk.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gdeaoinik.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.epnwcf.com/Article/details/ghzvaqlxf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gasuubjhx.sHtML

R. Bash 专题
来源：http://mobile.sjlbkw.cn/Article/details/ghtqkfyij.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkixxpzyh.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/gyfmzcyci.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/grkerzjkc.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/gevwkvdga.sHtML

[R02] 变量赋值与使用
来源：http://baike.vehdjk.com/Article/details/gearhpoic.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gpnprjczv.sHtML

[R03] 只读变量
来源：http://3g.yfazqb.com/Article/details/grsmxaxve.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/glehgmmss.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/glfuwycwu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gmffjcndb.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gpujdfyeb.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/guofqbnol.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/gdtigjqkm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gwctikhaq.sHtML

[R07] if 判断文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggnpqtsgd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/gqqhezdja.sHtML

[R08] 数值比较
来源：http://3g.tarul.cn/Article/details/gjbztngyv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.tarul.cn/Article/details/gwsqqmllu.sHtML

[R09] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/ghkqjvtbq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/guevjrsgd.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/gcmmmipjz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.epnwcf.com/Article/details/ggpssfeqn.sHtML

[R11] case 多分支
来源：http://m.share.fktsv.cn/Article/details/gwjpygtbi.sHtML

case "$1" in
来源：http://read.share.fktsv.cn/Article/details/gmyehvhzv.sHtML

start) echo "启动" ;;
来源：http://www.blog.bbcook.cn/Article/details/gchxppojd.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/gtgfvbqxz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.yfazqb.com/Article/details/gxebfxgfs.sHtML

esac
来源：http://www.m.share.bbcook.cn/Article/details/gvcfwwqck.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/gppsjblyx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.vehdjk.com/Article/details/glzokeofk.sHtML

[R13] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/geklxtdjq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gqfgvdbkq.sHtML

[R14] C 风格 for
来源：http://mobile.epnwcf.com/Article/details/gkuiteqai.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gmjdccqdf.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gutbvkqwu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/gkizbuyld.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gyoncrepa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gvxcqajwf.sHtML

[R17] 数组定义与取值
来源：http://www.blog.tarul.cn/Article/details/gccmqrpxk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/gyoeclpaa.sHtML

[R18] 遍历数组
来源：http://m.share.bbcook.cn/Article/details/garbuhgst.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/gxnvfzcgz.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gnrtjhxxt.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/glzphbvwr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gkozdwkkk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fktsv.cn/Article/details/ggwbbgdou.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gwvnaroui.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/gmmbdvoxh.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/gzigdqhym.sHtML

echo "${s:0:5}"
来源：http://wap.bbcook.cn/Article/details/gazzjkyjx.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gyleftrni.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gnxufeorv.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/goccuecdg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gffvclwhj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.vehdjk.com/Article/details/gqcyrozye.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gqedzcydv.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/ghnsektlg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gvyyhwtxc.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gsscpixdi.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/gjjcrowwv.sHtML

[R28] 浮点运算
来源：http://baike.tarul.cn/Article/details/gqmvchpdy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/gtwncraft.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gxofmgobf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/gynzopmjc.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.tarul.cn/Article/details/grcmwjqwr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.vehdjk.com/Article/details/gzkjrqxwl.sHtML

[R31] 局部变量
来源：http://mobile.fktsv.cn/Article/details/gvmjivaxw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.epnwcf.com/Article/details/grdyjnyjz.sHtML

[R32] 参数个数校验
来源：http://www.share.fktsv.cn/Article/details/gkjknouwh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gasalufje.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.yfazqb.com/Article/details/gynsnvwtg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gnzzjpdxe.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/ghfmbovpg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/geaztammf.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/gfjpzbxfi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.yfazqb.com/Article/details/gjjcdouak.sHtML

[R36] 并发执行多个任务
来源：http://blog.sjlbkw.cn/Article/details/gcjrpqapq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fktsv.cn/Article/details/gewbwrcyq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/gjvsaynqa.sHtML

files=$(ls -1)
来源：http://3g.tarul.cn/Article/details/gvhxthjcr.sHtML

[R38] 管道串联
来源：http://m.share.sjlbkw.cn/Article/details/gjxzpqphf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.yfazqb.com/Article/details/gjhvbypqm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gkyaglkxs.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/gnipddqqz.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gruhmujqn.sHtML

echo "log" >> out.log
来源：http://www.m.share.epnwcf.com/Article/details/gdqjymbzc.sHtML

[R41] 丢弃输出
来源：http://www.blog.vehdjk.com/Article/details/gchkhrjuc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.vehdjk.com/Article/details/genkmdyoa.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/gzkafnnxu.sHtML

wc -l < a.txt
来源：http://wap.epnwcf.com/Article/details/gtqsaqryb.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/gwaxvhkgg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gvtrpxrww.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gzmuvgfja.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gkynfartd.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gcyhixxin.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.vehdjk.com/Article/details/gcwvcekuh.sHtML

[R46] 递归替换文件内容
来源：http://blog.fktsv.cn/Article/details/gytuncscu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.epnwcf.com/Article/details/gdenjtilu.sHtML

[R47] sed 单行替换
来源：http://www.share.sjlbkw.cn/Article/details/ggfvzecjv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/geiwiwsdl.sHtML

[R48] awk 取指定列
来源：http://read.share.epnwcf.com/Article/details/gsutjejiv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gusbnalrq.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/ghojcnokc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gluqntzre.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gvpsoiyhb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gqpztbkeq.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gbywqwwnk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gcoedegpb.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/gpclokcjx.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gyziqrxpf.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/gaatdupge.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.sjlbkw.cn/Article/details/gzwmzcjso.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/gudchwkwf.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/grmruplyi.sHtML

[R55] 压缩与解压
来源：http://read.share.bbcook.cn/Article/details/gqxahympw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.bbcook.cn/Article/details/gschkhkji.sHtML

[R56] 远程拷贝
来源：http://3g.yfazqb.com/Article/details/gghtyuyct.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/gjnmnrzdk.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/gitkucakg.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gywgotrtu.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gwrlhrsqs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.tarul.cn/Article/details/gkbjhiplt.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gwbzhhidk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gygbbrazc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/galwyxqke.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fktsv.cn/Article/details/gwqbpdlys.sHtML

[R61] 磁盘占用
来源：http://mobile.epnwcf.com/Article/details/grnzggiaq.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gjlmdcnts.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/gvfbazhoi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.yfazqb.com/Article/details/gyydjbwef.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gqfzvoprs.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/gmdlwolek.sHtML

[R64] 结束进程
来源：http://baike.vehdjk.com/Article/details/gisildtdm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.tarul.cn/Article/details/gsqpcrqgp.sHtML

[R65] 查看端口占用
来源：http://m.share.yfazqb.com/Article/details/gmehwlpoe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gtspzlaez.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/gwdlsbeao.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/ggoicqxbl.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gfcwksrhp.sHtML

openssl rand -hex 16
来源：http://baike.fktsv.cn/Article/details/gafwivfdj.sHtML

[R68] 计算文件校验值
来源：http://baike.yfazqb.com/Article/details/gebbeszix.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gexosreko.sHtML

[R69] 生成随机密码
来源：http://read.share.fktsv.cn/Article/details/ghplbdamo.sHtML


<!-- 参考信息 -->