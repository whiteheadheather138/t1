代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gczlrzrvv.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gjvfjizmg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gblpyuiar.sHtML

[Q25] 只取前 N 条
来源：http://m.share.bbcook.cn/Article/details/gxhuqyouc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gmyzcyqls.sHtML

[Q26] 计数
来源：http://3g.yfazqb.com/Article/details/glhyoyoxq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gshkkozde.sHtML

[Q27] 条件计数
来源：http://baike.sjlbkw.cn/Article/details/giataauzk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/gwfiljaqd.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/guvezbzdz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gpqcnbahu.sHtML

[Q29] 最大最小值
来源：http://m.share.vehdjk.com/Article/details/gplfibrxu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gnguevkmx.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gfgcsejwi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gzzlinuuh.sHtML

[Q31] 分组后过滤
来源：http://3g.sjlbkw.cn/Article/details/gsubdtxsh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gygnsrqom.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gogtxizpn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gizsnaucz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/gwkrriicb.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gitxhsfnb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gltkkmxpl.sHtML

[Q34] 每组取第一条
来源：http://www.blog.yfazqb.com/Article/details/gsgtccjyw.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/gbaygyphy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.bbcook.cn/Article/details/gofepynfh.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gudhgowsl.sHtML

[Q35] 内连接
来源：http://www.m.share.fktsv.cn/Article/details/gcgfbnboz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/geofxdoei.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/goccjreme.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gtzoxujwk.sHtML

[Q37] 右连接
来源：http://blog.epnwcf.com/Article/details/gxogavzbj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/gbbiokuap.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/gmvwvgkaf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gjftlldyk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fktsv.cn/Article/details/gyzdbuqsm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/gfhzapvyi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.bbcook.cn/Article/details/gczsiuync.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/gisrdcyyu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.vehdjk.com/Article/details/gzdjaanfi.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/gqhctubkq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gdplubqhe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.epnwcf.com/Article/details/gvtqttmzb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gptgxlzlg.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/gnmhepldw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.yfazqb.com/Article/details/ggrnrkpuv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/gfpfspwox.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/gljbbbycq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.sjlbkw.cn/Article/details/gjuaqkwtk.sHtML

[Q44] IN 子查询
来源：http://www.share.tarul.cn/Article/details/gyertfieq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/goyrfiopv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fktsv.cn/Article/details/gdsbbibeo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/gqetjogvx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.tarul.cn/Article/details/gwrftbpeq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gkytslrtc.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.epnwcf.com/Article/details/gcpftlmob.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/gprxqbgwo.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.yfazqb.com/Article/details/gkxoxcoan.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/gfshplxbu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/growyceyn.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/guvyouwgm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gwfwkbnbm.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/ghvwhqsbx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.vehdjk.com/Article/details/gyznffsep.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gkvqiduda.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gezyxzmmw.sHtML

[Q52] 删除指定行
来源：http://3g.fktsv.cn/Article/details/gsvwyofbv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gyymnqgnl.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/gysvfayar.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gyezuyjew.sHtML

[Q54] 清空表
来源：http://m.share.epnwcf.com/Article/details/gkwuedztr.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.yfazqb.com/Article/details/gvccguwnt.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/goswqxcsr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gqrsodcay.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gdfxvtctx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhqbjgit.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gabolfbwz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/gupmcowzy.sHtML

[Q58] 累计求和
来源：http://blog.tarul.cn/Article/details/ggbwyxiew.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gmiglbxak.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/gveolfmum.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gaoozcteg.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/glujevfxd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gafhhrkvq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gnbvbmkay.sHtML

[Q61] 移动平均
来源：http://mobile.vehdjk.com/Article/details/guztngtvt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/ghaioiljx.sHtML

[Q62] 分组占比
来源：http://www.share.epnwcf.com/Article/details/getppzzll.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gvtqkuqbw.sHtML

[Q63] 开启事务
来源：http://m.share.tarul.cn/Article/details/ghpsaziee.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gbktwvxtb.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gukyqeoyy.sHtML

COMMIT;
来源：http://mobile.bbcook.cn/Article/details/gcfwgaklr.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gcsfgyaou.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gfzlydogs.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/giigdpchm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.sjlbkw.cn/Article/details/gxgccxegj.sHtML

[Q67] 设置隔离级别
来源：http://3g.epnwcf.com/Article/details/gptfosapk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gbaidqiyk.sHtML

[Q68] 保存点
来源：http://www.m.share.bbcook.cn/Article/details/gjluqgyht.sHtML

SAVEPOINT sp1;
来源：http://baike.vehdjk.com/Article/details/gkjepawdx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gcgwtzqol.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gmpmsihcy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.epnwcf.com/Article/details/gjfumxgqb.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/gkwybhmaf.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/gemsrdnop.sHtML

[Q71] 查看建表语句
来源：http://wap.tarul.cn/Article/details/gfqkmxnhi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gajwagvko.sHtML

[Q72] 查看索引
来源：http://www.share.yfazqb.com/Article/details/gvkqtumnc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/ggabcsyvo.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gmnytqfvq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.epnwcf.com/Article/details/gifzkqcto.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gmdymhgsp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/gqnauovoz.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/ghblxvesf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/grnchtkhc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gopckbiwb.sHtML

[Q76] 按天统计
来源：http://baike.vehdjk.com/Article/details/gwbmrbhae.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fktsv.cn/Article/details/gwbscjniy.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/gocmaqozu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.yfazqb.com/Article/details/gfmfxzfio.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/gaqvanoeh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gtcegpkqe.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/gpzlekvoj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gwfiigyiu.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/giyotbhhj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/grakoptpa.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gyvvuzsrj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.bbcook.cn/Article/details/gyrpirezu.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fktsv.cn/Article/details/grznhkyec.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gtsehipen.sHtML

[Q83] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gpwdrmnme.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gvwfyysvr.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/gihfazpba.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/glkfibxox.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/gvujmttye.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/gkelnytxu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/gmrzcegtd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/gjpgnwbgl.sHtML

[Q87] JSON 字段做条件
来源：http://blog.tarul.cn/Article/details/grjaofwto.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvahdmpo.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.bbcook.cn/Article/details/grkslyskc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.epnwcf.com/Article/details/gndbjfemz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/gufvjpvmi.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/ggfsyucwo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gqfwjgggq.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/ggvpzsayv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fktsv.cn/Article/details/ghlysiggq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghzzjzisq.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gwavspcsw.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geftlsatj.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.epnwcf.com/Article/details/gjoqmhyoc.sHtML

#!/usr/bin/env bash
来源：http://baike.vehdjk.com/Article/details/gnmkhliht.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gblmhzlwl.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/glpmvtkob.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.tarul.cn/Article/details/gitngjjdo.sHtML

[R03] 只读变量
来源：http://www.share.bbcook.cn/Article/details/gvdqysvms.sHtML

readonly PI=3.14
来源：http://mobile.epnwcf.com/Article/details/gvntqwrza.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gyigyafze.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/ghaewubjp.sHtML

[R05] 参数默认值
来源：http://www.m.share.epnwcf.com/Article/details/giqemrhcb.sHtML

name="${1:-default}"
来源：http://baike.epnwcf.com/Article/details/gwgweclul.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/gfaznrecm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gxjakmqqr.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/giyolsrcq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gnhdcsuuq.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/gmobrudpq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/gvbddznrv.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/grcyfxyhr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.epnwcf.com/Article/details/guiffjqsf.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/grrrszdpa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/ghujltzbs.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/gngpfkgax.sHtML

case "$1" in
来源：http://baike.bbcook.cn/Article/details/gxlfcyefi.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gmajycjpj.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/gejkdrwvi.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gefynwjmu.sHtML

esac
来源：http://wap.vehdjk.com/Article/details/guofwduda.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/gtslxzryr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/gcbxfonnx.sHtML

[R13] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/ghdkzywya.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gelsibbou.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/gwwzlnqzj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gcmrrwcov.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gmqpwacwn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/guqcwzwsc.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gublocqmy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/goivknxea.sHtML

[R17] 数组定义与取值
来源：http://www.blog.yfazqb.com/Article/details/gtshibkhq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gyoqtrory.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/ghzlazfks.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gquuykwfk.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gjfeoiqab.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/guvxueobq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gkumjqlcb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/gexuqfggy.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/gkgsmqcyu.sHtML

echo "${#s}"
来源：http://www.blog.tarul.cn/Article/details/gxsbernzg.sHtML

[R22] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/guvsaxrcj.sHtML

echo "${s:0:5}"
来源：http://www.blog.sjlbkw.cn/Article/details/gauyraeul.sHtML

[R23] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/ghhxbpxpx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.sjlbkw.cn/Article/details/gwmjquiso.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gvsozahbr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gebqlnpdz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/gdneeosjj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.sjlbkw.cn/Article/details/ghjcfoixe.sHtML

[R26] 命令替换
来源：http://wap.fktsv.cn/Article/details/gcmmwtthy.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gvfaofzll.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/gtofacjnl.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/gzyilpvad.sHtML

[R28] 浮点运算
来源：http://3g.fktsv.cn/Article/details/gmbstazmu.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.vehdjk.com/Article/details/gbrwhqxpq.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gztbkhmhs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/gqktohawx.sHtML

[R30] 函数返回状态码
来源：http://read.share.fktsv.cn/Article/details/gneeovltx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/gybvabzmo.sHtML

[R31] 局部变量
来源：http://blog.yfazqb.com/Article/details/gclactyum.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gpyanushq.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/gebytuaee.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/ghovqbcoc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/ghxgbhyno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gdyvqjpfi.sHtML

[R34] 退出时清理
来源：http://3g.tarul.cn/Article/details/gmuzpipxb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gwwrqynjt.sHtML

[R35] 后台执行并等待
来源：http://baike.vehdjk.com/Article/details/gcugxkfbi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.yfazqb.com/Article/details/gcgvaafyi.sHtML

[R36] 并发执行多个任务
来源：http://m.share.yfazqb.com/Article/details/gxbbelqnq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpgblnqh.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.vehdjk.com/Article/details/gtitzlpar.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/gfziuysuf.sHtML

[R38] 管道串联
来源：http://www.blog.yfazqb.com/Article/details/glnlvmycx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.bbcook.cn/Article/details/gqpcuykci.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/glineklmk.sHtML

cmd > out.log 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/ggpefomfd.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gzejkhstm.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/gndgvqxli.sHtML

[R41] 丢弃输出
来源：http://3g.epnwcf.com/Article/details/gcvnwmkko.sHtML

cmd >/dev/null 2>&1
来源：http://blog.tarul.cn/Article/details/guaicubuh.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/ghqbgsnsr.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gdvqhdebs.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/ggoeycuyo.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gzrxlycud.sHtML

[R44] 按修改时间查找
来源：http://m.share.tarul.cn/Article/details/gbxtedmpv.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gherlreac.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbjyaide.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gfzryfuiw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gkzyssmhh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gqauxauwf.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gtbfxpcgo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.tarul.cn/Article/details/gmltvbfkn.sHtML

[R48] awk 取指定列
来源：http://www.blog.epnwcf.com/Article/details/gdzpqggsx.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gixuibhwf.sHtML

[R49] awk 带条件
来源：http://baike.bbcook.cn/Article/details/grguqljld.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gbwaayjbf.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/gmqyrptpf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gmmkyqotb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.yfazqb.com/Article/details/gcsyqwgvp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fktsv.cn/Article/details/gnulbfthq.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gqywlviee.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gpbimxntz.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.vehdjk.com/Article/details/gswzixihg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.vehdjk.com/Article/details/guftmiber.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gvetgyusr.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gkbrdbphc.sHtML

[R55] 压缩与解压
来源：http://blog.epnwcf.com/Article/details/gpajkxfjm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.vehdjk.com/Article/details/gdxlzdpuv.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/gcwhmxqjk.sHtML

scp file user@host:/path/
来源：http://baike.tarul.cn/Article/details/gcqqedvye.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gycklcgwe.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gmnymrwiu.sHtML

[R58] 下载文件
来源：http://www.blog.vehdjk.com/Article/details/gzdrfeeqj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gziyjfimo.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gvhyvimpy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/gaejrlknp.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gqgcgnhgp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/gwnjqtmsm.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fktsv.cn/Article/details/gqgkmbmkw.sHtML

df -h;  du -sh *
来源：http://3g.epnwcf.com/Article/details/ghybfbise.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gqhkqrnvh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gpbegmpfc.sHtML

[R63] 内存与进程
来源：http://wap.sjlbkw.cn/Article/details/gtagenuuw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/gqjwwchou.sHtML

[R64] 结束进程
来源：http://blog.epnwcf.com/Article/details/gmzjkzqca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.epnwcf.com/Article/details/gmrkkmjah.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gnzjusfpr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.tarul.cn/Article/details/ghzfwiorv.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/gbnyqbulz.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/gmiszvuzg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gufdzwuoy.sHtML

openssl rand -hex 16
来源：http://www.blog.sjlbkw.cn/Article/details/gibvzwpbo.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/grjljacsm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/gyzdsyhwe.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gnvbbevsa.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/ggtvceegf.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/gkuaxhxyz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.bbcook.cn/Article/details/gfgamgscv.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gogllcjtk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/gctzhjfos.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gxgwjkjwc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gfwchlzlm.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/gptblrqsz.sHtML


<!-- 参考信息 -->