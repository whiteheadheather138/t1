代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.bbcook.cn/Article/details/gnqumjgvu.sHtML

[Q26] 计数
来源：http://blog.vehdjk.com/Article/details/gxuenepei.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.tarul.cn/Article/details/ggdiarotz.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gfhousfhe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gxbygweau.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/gftvcfubd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gqqhvxjjz.sHtML

[Q29] 最大最小值
来源：http://read.share.fktsv.cn/Article/details/gmdqngwnh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gjguxxqlr.sHtML

[Q30] 分组统计
来源：http://wap.vehdjk.com/Article/details/gcopklvxv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/goviqntli.sHtML

[Q31] 分组后过滤
来源：http://m.share.sjlbkw.cn/Article/details/gtaeivhwd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fktsv.cn/Article/details/gtsqllhul.sHtML

[Q32] 分组拼接字符串
来源：http://3g.bbcook.cn/Article/details/gherdgbgc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gqpvvqtod.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gpvroqijz.sHtML

[Q33] 多列分组
来源：http://blog.bbcook.cn/Article/details/gqxmrxqrs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.vehdjk.com/Article/details/gggcudlqn.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gffuneubu.sHtML

SELECT * FROM (
来源：http://read.share.epnwcf.com/Article/details/gvrhaaknw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gdnkokqir.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gymonqrwo.sHtML

[Q35] 内连接
来源：http://read.share.epnwcf.com/Article/details/gxasyvdee.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/ghzgquqoi.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gicdawvdo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gssvjxxth.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/gnfzrayfn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/gmzklrkdc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.vehdjk.com/Article/details/gygnvyblr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.epnwcf.com/Article/details/gqrsxvsjz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.tarul.cn/Article/details/gxcjlzblu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.tarul.cn/Article/details/gzofmchwj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/goimzdoep.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gqrescbhd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/gxgjlnbai.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gdfcuqnhg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/ganhhgmlg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/ghgvitgvd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.vehdjk.com/Article/details/gqcsatlcm.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gamthxdcn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gmaeienng.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gtscnybre.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gvqawburl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.epnwcf.com/Article/details/gkdjnelnn.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/giimrhufb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/giotiaoup.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gshcaalii.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gkjmrbatb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.vehdjk.com/Article/details/gheesvvxw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/ghoonywwo.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfzvfqxv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.epnwcf.com/Article/details/gaeoqnpmy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/ghualrdjp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gflivyisl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/grqqapejv.sHtML

[Q49] 更新单行
来源：http://wap.yfazqb.com/Article/details/gnkaaxzoh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gxcwxyqnw.sHtML

[Q50] 批量更新
来源：http://baike.vehdjk.com/Article/details/gcvpguton.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/gkzceicdg.sHtML

[Q51] 用子查询更新
来源：http://3g.fktsv.cn/Article/details/gyumiulmj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/gmfezpvoi.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/ggthptnkl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gkvxlbiqh.sHtML

[Q53] 按条件删除
来源：http://wap.yfazqb.com/Article/details/gcjskzprs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gdarkvoxi.sHtML

[Q54] 清空表
来源：http://www.m.share.bbcook.cn/Article/details/giazttmbb.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.sjlbkw.cn/Article/details/gsuvsrhij.sHtML

[Q55] 排名（并列占位）
来源：http://baike.tarul.cn/Article/details/gufgdzqaf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gamtvqdhg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gblluppuw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gsnaczzuz.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gjmtiatpo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/gbrusevmm.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gkgngdncw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gicjihgge.sHtML

[Q59] 分组内累计
来源：http://www.m.share.tarul.cn/Article/details/gzbejdner.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/golnfwduk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gcyroqfsh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.tarul.cn/Article/details/geizpdkzw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gkaccwvjc.sHtML

[Q61] 移动平均
来源：http://m.share.bbcook.cn/Article/details/gmugwujdk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gfranotpw.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/gsnysvifn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyfducur.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/gdavdqkza.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gqrmtzvzb.sHtML

[Q64] 提交事务
来源：http://www.blog.sjlbkw.cn/Article/details/goknwspou.sHtML

COMMIT;
来源：http://blog.vehdjk.com/Article/details/gbsbjnfqj.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gwqktgsgd.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/galqlfets.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gnsigeuqe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.sjlbkw.cn/Article/details/ghcrzrncd.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/gecwwdoig.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/grqewvgin.sHtML

[Q68] 保存点
来源：http://mobile.epnwcf.com/Article/details/gxsmsqxhq.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/gnfkzehci.sHtML

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/gidfhygpm.sHtML

[Q69] 查看执行计划
来源：http://www.blog.epnwcf.com/Article/details/gcmnifrwa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gdjffzkqp.sHtML

[Q70] 更新统计信息
来源：http://baike.vehdjk.com/Article/details/gmyeafmtc.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.bbcook.cn/Article/details/gkimxsauh.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/gbhocrczr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gxxhmofqe.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gpcekmpka.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/goabpqzgv.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/gkurxxrub.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.yfazqb.com/Article/details/gafybtjio.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gylizcwyi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/gersghrle.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gxbhykewp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gdppotjzd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.tarul.cn/Article/details/gvlglrehn.sHtML

[Q76] 按天统计
来源：http://www.m.share.bbcook.cn/Article/details/gqxkkyayj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.sjlbkw.cn/Article/details/gmqwipzxq.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gprbopoyy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gtoudbgna.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/gilyppluc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/grzaatuwi.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/gkiohnkmz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/gzljhpdqx.sHtML

[Q80] 字符串截取
来源：http://wap.tarul.cn/Article/details/glenpsfil.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.bbcook.cn/Article/details/guxsxzyzm.sHtML

[Q81] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gkfjwfezg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gcahejncs.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/gmjjuhvfl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/ghntzkkyy.sHtML

[Q83] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/glvqalbwz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gtwtonqko.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gzqiscoyx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/grhfuopxq.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gsxgqqksm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.sjlbkw.cn/Article/details/gqdrhwlri.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fktsv.cn/Article/details/gzavhfjqs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/gdojzuwuu.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/gyjsqlvcv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gpmcafvwl.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gvfhqsmhz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/gilrgvmmh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/gxlplileg.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gsyhjiksi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gmazeulfq.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/gyvynhulx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gcvqiuupa.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggoyqbwft.sHtML

R. Bash 专题
来源：http://www.share.yfazqb.com/Article/details/grjtdftix.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gufabuqiy.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/gzxtnxaik.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/giuvcuuhp.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gnpzfyqrq.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gkmpwgldg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/gsoaazjem.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gkdgtnqzc.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/gtcbxseem.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gtzufcved.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.yfazqb.com/Article/details/geywrmvhk.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/gthzyucsz.sHtML

name="${1:-default}"
来源：http://read.share.tarul.cn/Article/details/gtaollqbk.sHtML

[R06] 判断命令是否存在
来源：http://baike.yfazqb.com/Article/details/glzocljlq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/glpqgvsfa.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/gvvwpfqon.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/genqbkozn.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/guanmtktv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.tarul.cn/Article/details/gurdbwvox.sHtML

[R09] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gfswqjkdi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.yfazqb.com/Article/details/gvoizbwlr.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gmmfhlpra.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gjbknmhab.sHtML

[R11] case 多分支
来源：http://www.share.epnwcf.com/Article/details/gemehoxdx.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/ghvbgqtuc.sHtML

start) echo "启动" ;;
来源：http://mobile.yfazqb.com/Article/details/gcvztghre.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gdjwfzpvh.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/gbqngrlpv.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gjhxagjyr.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/geivkfzlq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/gvxqtoykv.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gtuukunwq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gsbonotft.sHtML

[R14] C 风格 for
来源：http://3g.epnwcf.com/Article/details/grgehnynv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/gjwxntfzj.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gqezlsfaj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/gamzuyspq.sHtML

[R16] until 等待条件
来源：http://m.share.epnwcf.com/Article/details/gbmestlic.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.tarul.cn/Article/details/grmwvvmma.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gzithrmgz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/gxszxotwl.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gwpikqzvl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/gljisitho.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gkbqpvdcp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gctmooqji.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gshcpaemv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/gnnzbonkd.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gnyqtchtf.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gspcvqzoc.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gkvqsvmqp.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gqlfuhjss.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gbovszjle.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.sjlbkw.cn/Article/details/gqueyvyea.sHtML

[R24] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gatddogaw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/glmcwocpc.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gmkugicuw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.sjlbkw.cn/Article/details/gyrbbxtvd.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/giccnakwl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.vehdjk.com/Article/details/gctltpwob.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gticzrquj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gczzmrafl.sHtML

[R28] 浮点运算
来源：http://www.m.share.sjlbkw.cn/Article/details/givwxjzfq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.epnwcf.com/Article/details/gbgjetwpt.sHtML

[R29] 定义函数
来源：http://wap.vehdjk.com/Article/details/gofaixzwb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/gpsvblhvu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gqycknfjs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gehrojvhy.sHtML

[R31] 局部变量
来源：http://wap.yfazqb.com/Article/details/gdwcvfwma.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gbmjoviam.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/gizyhmpsf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gdhnksshs.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gcfgobaij.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/gkpiqdgvz.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvuodjgf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gegxrdmob.sHtML

[R35] 后台执行并等待
来源：http://wap.sjlbkw.cn/Article/details/gzlrcvlsy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fktsv.cn/Article/details/gyqdzdhuc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.vehdjk.com/Article/details/gsbpnfxfq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gzcjgkprs.sHtML

[R37] 把输出赋给变量
来源：http://3g.fktsv.cn/Article/details/gzssweian.sHtML

files=$(ls -1)
来源：http://mobile.vehdjk.com/Article/details/ggiwsgrfr.sHtML

[R38] 管道串联
来源：http://3g.bbcook.cn/Article/details/gohmhviua.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gfimhfqyb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.sjlbkw.cn/Article/details/gsakhomlf.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gwxovoaje.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gwgdvtezg.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/gdjhbdvnz.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gjaxiakdy.sHtML

cmd >/dev/null 2>&1
来源：http://blog.epnwcf.com/Article/details/gbxbticcw.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gieyjgvuu.sHtML

wc -l < a.txt
来源：http://www.share.bbcook.cn/Article/details/gieezkoqw.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/gxqeyzjzk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gqjjbzfrb.sHtML

[R44] 按修改时间查找
来源：http://wap.fktsv.cn/Article/details/gvqaxbcda.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/ggonhcafp.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/grkktdxpc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/giaumcpct.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gvjvdhzqp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/gzvoaoytx.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gheofickn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gxcxvypwg.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gdueiojra.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/ganccktgo.sHtML

[R49] awk 带条件
来源：http://wap.yfazqb.com/Article/details/gpbkgkyqg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.bbcook.cn/Article/details/gnxxonutf.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/ghxeenujh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.sjlbkw.cn/Article/details/ghywqnyxp.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.vehdjk.com/Article/details/ggieyzegi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.bbcook.cn/Article/details/gqfavdqgr.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/giavcicco.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gximhyhet.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fktsv.cn/Article/details/glxdcpfwq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/gezdulklu.sHtML

[R54] 比较两个文件
来源：http://www.m.share.yfazqb.com/Article/details/gfrmikngu.sHtML

diff a.txt b.txt
来源：http://www.blog.epnwcf.com/Article/details/gsspqmdwn.sHtML

[R55] 压缩与解压
来源：http://3g.sjlbkw.cn/Article/details/gvzufpcen.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.bbcook.cn/Article/details/gtbifhatj.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gdpygetqp.sHtML

scp file user@host:/path/
来源：http://mobile.epnwcf.com/Article/details/gzyjjujir.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gsswpzpul.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/glpojotyz.sHtML

[R58] 下载文件
来源：http://m.share.yfazqb.com/Article/details/gtgepnggv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.vehdjk.com/Article/details/gcbxpgcfu.sHtML

[R59] 发 POST JSON
来源：http://www.share.bbcook.cn/Article/details/geehyxkdd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.epnwcf.com/Article/details/gakeavlgh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gaxnyxioo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/gncrkwmxm.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/gvkqfgevf.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gghiroqao.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gupqmulge.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.bbcook.cn/Article/details/gvophyafj.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gowmnavke.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gnnjueqtu.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gcdsqdhnw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.sjlbkw.cn/Article/details/glszfuwno.sHtML

[R65] 查看端口占用
来源：http://read.share.fktsv.cn/Article/details/ganvlxpip.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/gjusakpaf.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gxsqnnxgl.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/gcuomfjsq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.epnwcf.com/Article/details/gtdmrgrda.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gmzbanzvw.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/gtzmxfqln.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/ggtunhbsd.sHtML

[R69] 生成随机密码
来源：http://m.share.epnwcf.com/Article/details/gjsnrpmcm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxdsvzil.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gzaxkiysq.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.vehdjk.com/Article/details/grxslipvz.sHtML

[R71] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gjsaprlpv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.yfazqb.com/Article/details/gzvjtpaes.sHtML

[R72] 等待端口就绪
来源：http://mobile.epnwcf.com/Article/details/gfoikfvtq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gyjvyfwqv.sHtML

[R73] 分割大日志
来源：http://read.share.yfazqb.com/Article/details/ggrazakfy.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gtpelacip.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/ghtdcneiz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/ghcnqypjj.sHtML

[R75] 导出环境变量
来源：http://www.share.yfazqb.com/Article/details/gnfhnnteg.sHtML


<!-- 参考信息 -->