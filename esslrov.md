代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjctchrv.sHtML

[Q24] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gecieuhmc.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gechcyiaa.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gccxcnzvm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gtaznefet.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gccgdcxue.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gwrfqijvh.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/guggomreo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.vehdjk.com/Article/details/glfyxlhgu.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/guwhbiauq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gpmjpkolk.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gvjtrirog.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gcoqbtmhr.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gulainetd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gjgygkifc.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/glgmwvfsg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.sjlbkw.cn/Article/details/gbxxadvkj.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gldowbwpp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gqxexxalh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/giufsltkv.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/gjakyikte.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gngqatgne.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gitqqklpp.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/gleosopai.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gnjydchks.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gdpvmchye.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/gwuntnjfl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gxjvasbws.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/gluynjtdf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gmfhtbwua.sHtML

[Q37] 右连接
来源：http://blog.tarul.cn/Article/details/ggdskmzmq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.sjlbkw.cn/Article/details/grjsfnwkw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.vehdjk.com/Article/details/ghfnbizkj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gnclewdex.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gnrmtkfsd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.epnwcf.com/Article/details/gjwomyoeh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/gjsacumpx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.tarul.cn/Article/details/girbbunnz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/gxonytzjb.sHtML

[Q41] 多表连接
来源：http://read.share.epnwcf.com/Article/details/gvmqusyhc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gmemsmwbi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.vehdjk.com/Article/details/gdfannvfj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gcnixfsqm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gklgqgxhu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gvoeioiou.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.tarul.cn/Article/details/gzubbmzky.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/grhgtjvbo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/gdbjkkdem.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/grqcadpyl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/gfhyexswq.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.tarul.cn/Article/details/ghterbjng.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/ggwmkxbex.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/grcvxkzei.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/ghqbvctcn.sHtML

[Q47] 与平均值比较
来源：http://m.share.vehdjk.com/Article/details/ghawjhuuq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.yfazqb.com/Article/details/gbswfarne.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.bbcook.cn/Article/details/gtyuvelpa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fktsv.cn/Article/details/gzfslkhgz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.epnwcf.com/Article/details/gwoopptal.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gxronzxcu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gmxjczfkf.sHtML

[Q50] 批量更新
来源：http://mobile.fktsv.cn/Article/details/gteotgxhw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/guivotfkx.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gvyiflvhj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/gxutjwkdm.sHtML

[Q52] 删除指定行
来源：http://www.share.sjlbkw.cn/Article/details/gtwujuqtd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gylmkzghu.sHtML

[Q53] 按条件删除
来源：http://www.blog.yfazqb.com/Article/details/gjeqhdzmq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.epnwcf.com/Article/details/gosvokphw.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/geqdjyjoy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.epnwcf.com/Article/details/gyqfgaeto.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/gtitcogai.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gnhfpmgbv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gynuhczxi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/ggvqbixow.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/glyngstzw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.yfazqb.com/Article/details/ggctzxvas.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/gxmtgbgkb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gwharzunb.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/gsutidmto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/guhzpsgqn.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.sjlbkw.cn/Article/details/gjkwwonmy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gzxkbbqsb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gdpkckfdg.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gyidnwdsg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gncodzwfi.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/gnvihuhex.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gyzyfufht.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/gvojwbcpy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gvkvduast.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/guixmbrrt.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/gdzxbkxjr.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/gsozuydlp.sHtML

ROLLBACK;
来源：http://m.share.yfazqb.com/Article/details/gtusfcbll.sHtML

[Q66] 行锁查询
来源：http://mobile.epnwcf.com/Article/details/gmbuczqfy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/gymdmkokc.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gsbprfqhg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gonawroyj.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gkwolzcrj.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gzsmnfvfi.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/gcevwspeo.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gntnqnscw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gsotaeunj.sHtML

[Q70] 更新统计信息
来源：http://blog.yfazqb.com/Article/details/gearwbpey.sHtML

ANALYZE TABLE users;
来源：http://3g.tarul.cn/Article/details/ghjqvrirk.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gtrkznwpf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/gyhhjupnj.sHtML

[Q72] 查看索引
来源：http://www.share.yfazqb.com/Article/details/gjrgpewjh.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/gpxxuzryn.sHtML

[Q73] 查看表状态
来源：http://wap.epnwcf.com/Article/details/gyqzvcyvl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.yfazqb.com/Article/details/grgtewakk.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gfebmqrii.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/gaygvgnlr.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/glkwefeei.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gpuccjnnk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.bbcook.cn/Article/details/gjfpbjhxs.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/glotsnuxq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/gvxntayjn.sHtML

[Q77] 时间加减
来源：http://www.share.epnwcf.com/Article/details/gablkqtoq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/gykjrxseo.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/gjxnjeqtr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/gcggqhiuw.sHtML

[Q79] 字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gngximybs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.tarul.cn/Article/details/gfblaojjj.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/gzjshxjsi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gamtiupsi.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gachrlmvj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fktsv.cn/Article/details/gaydnpwuj.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/grswjynjj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gdgpultub.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gjvmahmnl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/guwsrtphh.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/gsvoeltla.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gzfmowgcq.sHtML

[Q85] 数值取整
来源：http://m.share.vehdjk.com/Article/details/gwydwohpl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gaqsyyohc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/gwfgdxdyn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/gtthbxppb.sHtML

[Q87] JSON 字段做条件
来源：http://blog.yfazqb.com/Article/details/gsgicgpxx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/ghdslzhra.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.tarul.cn/Article/details/ghnhhqnmx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/glvcynvlk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gwjetzjnv.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gvfkrcyve.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fktsv.cn/Article/details/ggykchhry.sHtML

[Q90] 生成序号列
来源：http://blog.yfazqb.com/Article/details/gbejzqmeu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/ghqvnnlxf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gduputqeh.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gtzfghmwp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glsqqvepz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.yfazqb.com/Article/details/glhwhoptn.sHtML

#!/usr/bin/env bash
来源：http://blog.vehdjk.com/Article/details/gtjuykelk.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gchxizlmb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gesxkgkjp.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/guznlrrgu.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/gnqwlmicj.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/gpdqyzsiv.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/gfquogzql.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.tarul.cn/Article/details/ghuyfzgyd.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/gyquvdacx.sHtML

name="${1:-default}"
来源：http://baike.tarul.cn/Article/details/galloofxt.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/geikehqab.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/ghhrudryw.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/gibhdcmyo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.yfazqb.com/Article/details/gmjisguzc.sHtML

[R08] 数值比较
来源：http://3g.vehdjk.com/Article/details/gebdlzfwg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gwjseghqg.sHtML

[R09] 字符串比较
来源：http://3g.fktsv.cn/Article/details/gzrnqumhw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gfewjcawv.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gjuwkahqu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/gogubmrpn.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/gtfpqnvyv.sHtML

case "$1" in
来源：http://wap.vehdjk.com/Article/details/glbjgdnjy.sHtML

start) echo "启动" ;;
来源：http://mobile.bbcook.cn/Article/details/gzkldlxvr.sHtML

stop)  echo "停止" ;;
来源：http://m.share.epnwcf.com/Article/details/gssdnhukb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/gavshypnx.sHtML

esac
来源：http://www.m.share.epnwcf.com/Article/details/gtkxvqynf.sHtML

[R12] for 遍历文件
来源：http://blog.fktsv.cn/Article/details/gawvgmkip.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.vehdjk.com/Article/details/gjtvahvca.sHtML

[R13] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/glynpawru.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gcinkxxxe.sHtML

[R14] C 风格 for
来源：http://www.blog.bbcook.cn/Article/details/gsnqfbpeu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gyfywoike.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gbrjntfpn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/gphwoyyjf.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/gqqmediaa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gwlynwiot.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/gaoqakuyq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/grpxyqryy.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gaiafbraa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.vehdjk.com/Article/details/ghfoyzioi.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gnrsrshdf.sHtML

echo "${#arr[@]}"
来源：http://wap.yfazqb.com/Article/details/gztmhwcht.sHtML

[R20] 关联数组（字典）
来源：http://mobile.bbcook.cn/Article/details/gkzgixyle.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gtcjyeier.sHtML

[R21] 字符串长度
来源：http://3g.vehdjk.com/Article/details/gskutbqgk.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/gtcjkuqej.sHtML

[R22] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gzdgcgcsg.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gpftovqxz.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gojsgkdoe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/gfxfkhjwq.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/grplgtxvl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.epnwcf.com/Article/details/gzlveftyv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fktsv.cn/Article/details/gscgoosfj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/ghogclvqd.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/gbrbxejek.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gudfhhzhb.sHtML

[R27] 算术展开
来源：http://www.share.yfazqb.com/Article/details/gscukczbu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/guyxvnxmr.sHtML

[R28] 浮点运算
来源：http://wap.bbcook.cn/Article/details/gmitazzdy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/govigagzh.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gwzxtonhb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gktqvifkr.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gbreceuuq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.tarul.cn/Article/details/gvsaceasl.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gxzlyoeuz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.tarul.cn/Article/details/gebyrukco.sHtML

[R32] 参数个数校验
来源：http://m.share.bbcook.cn/Article/details/ggovezfjy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gxiwizvig.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gqdgnfabs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/glbkvthbe.sHtML

[R34] 退出时清理
来源：http://read.share.yfazqb.com/Article/details/gvlozniob.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gbcwitjtc.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/gtqxnljsr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.yfazqb.com/Article/details/gxlhwjuab.sHtML

[R36] 并发执行多个任务
来源：http://www.share.bbcook.cn/Article/details/gqtppbbli.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.yfazqb.com/Article/details/gkweujlya.sHtML

[R37] 把输出赋给变量
来源：http://m.share.bbcook.cn/Article/details/gtdpbyzpt.sHtML

files=$(ls -1)
来源：http://wap.yfazqb.com/Article/details/gkhwbnjdw.sHtML

[R38] 管道串联
来源：http://read.share.sjlbkw.cn/Article/details/gtwiwxott.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/gtvgztnnk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gjhxcznkt.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/gkfrrzfci.sHtML

[R40] 追加写日志
来源：http://mobile.yfazqb.com/Article/details/gkvatjzvw.sHtML

echo "log" >> out.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gznxzytlb.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gqbdnditi.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gxiupttnm.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/ggonsboxb.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gvtxubwiu.sHtML

[R43] 按名字查找文件
来源：http://m.share.tarul.cn/Article/details/glfabbyxp.sHtML

find . -name "*.log" -type f
来源：http://3g.yfazqb.com/Article/details/grgcswntk.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/gfzmenkco.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gxqxiyyqy.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxwnfzyh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/gbegcpovp.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gehfugfuz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gabsjzauf.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gpxbpbylm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gwkgntorg.sHtML

[R48] awk 取指定列
来源：http://3g.tarul.cn/Article/details/gyiwgblqd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/gdxgrgvux.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/gmaoqryxv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gccnfopze.sHtML

[R50] awk 求和
来源：http://www.share.tarul.cn/Article/details/gouynlbhi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gijjagbfq.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gbysikqyd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.sjlbkw.cn/Article/details/gcztdaspr.sHtML

[R52] 统计行数
来源：http://read.share.tarul.cn/Article/details/gydlfqydb.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gkzdwlvqo.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gtntnudnk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gogmacory.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/gijshrkps.sHtML

diff a.txt b.txt
来源：http://m.share.sjlbkw.cn/Article/details/gxlbglsvm.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/gpidjfnmh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.bbcook.cn/Article/details/gwlfajyoz.sHtML

[R56] 远程拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gortwdozh.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gzovcxpnl.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gojnxgaws.sHtML

ssh user@host 'uptime'
来源：http://m.share.vehdjk.com/Article/details/gwrzbboqy.sHtML

[R58] 下载文件
来源：http://mobile.fktsv.cn/Article/details/gzjkzcath.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.epnwcf.com/Article/details/gnauapoui.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gufsuecwi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gcwbxphpd.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gyglxpiaa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gqhhjgmjr.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gqkjybglv.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gguhwiqpt.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gcldngont.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fktsv.cn/Article/details/ggmixwkhp.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/gflfeddkm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.yfazqb.com/Article/details/gcghwksbk.sHtML

[R64] 结束进程
来源：http://mobile.tarul.cn/Article/details/glbawgout.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/ggfjqnrya.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/ghygjgueu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gjfwahgyn.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gcpyibmun.sHtML

crontab -e;  crontab -l
来源：http://www.blog.bbcook.cn/Article/details/gfjlidmhp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.tarul.cn/Article/details/gpjfybfpc.sHtML

openssl rand -hex 16
来源：http://m.share.epnwcf.com/Article/details/goqmjvzyn.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gwitkrgzs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/glnkhrsyh.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gizzcuqvv.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/ghegosctm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/gbttkuwdx.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.vehdjk.com/Article/details/gcuvvdqdr.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/goatbxzuy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/ghprdkmlq.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/gjpjfylvb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gawunsrcj.sHtML

[R73] 分割大日志
来源：http://m.share.bbcook.cn/Article/details/gssvmpizl.sHtML


<!-- 参考信息 -->