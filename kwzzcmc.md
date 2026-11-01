代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.epnwcf.com/Article/details/gmnyoksrg.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gnddxxkbv.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/givboscku.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/gnwbmzctk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.yfazqb.com/Article/details/gzmuaxnlr.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/gqdvzfzlk.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fktsv.cn/Article/details/ggrtkqgxz.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/grystrtnx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gyrbvklvt.sHtML

[Q28] 求和与平均
来源：http://mobile.epnwcf.com/Article/details/gshapbjja.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gcnrqvyac.sHtML

[Q29] 最大最小值
来源：http://wap.epnwcf.com/Article/details/gqisnmayx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/ghymglxif.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/gvsrrrbjl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/ghgdccars.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gjwwwkmao.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/garnuykjq.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gdbyuwgxs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gondllpjp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/gvvubigxh.sHtML

[Q33] 多列分组
来源：http://www.blog.bbcook.cn/Article/details/gxsffafbt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.tarul.cn/Article/details/gfikudtxs.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gctziqctr.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gxgptfvbl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gzywgovsq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gzusigsjs.sHtML

[Q35] 内连接
来源：http://blog.bbcook.cn/Article/details/gdhakerov.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/goyifjkqp.sHtML

[Q36] 左连接
来源：http://www.share.fktsv.cn/Article/details/ggjcnlgrs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gjffnyohb.sHtML

[Q37] 右连接
来源：http://3g.yfazqb.com/Article/details/gzbicaesa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.epnwcf.com/Article/details/ghbnbbbjb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.vehdjk.com/Article/details/ggljatpyd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/gnthgmjhf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/ghhucktie.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/ghzwanjzq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fktsv.cn/Article/details/gchklvgsz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/gfmzxqjbc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/gdrskbuik.sHtML

[Q41] 多表连接
来源：http://read.share.yfazqb.com/Article/details/gouiykmfz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.sjlbkw.cn/Article/details/gzlxjozrv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/gpzlbxsux.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.yfazqb.com/Article/details/gvcytbzpa.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gpqphriuf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gontuxdei.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/geuefjosz.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/grngeypmq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.tarul.cn/Article/details/gewuqopsy.sHtML

[Q44] IN 子查询
来源：http://www.blog.vehdjk.com/Article/details/ggrmvuxmq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.sjlbkw.cn/Article/details/gaeeyvjsv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gewwsmbyx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gjscdmgyf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/gxecmxxpm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gnvmujfjv.sHtML

[Q47] 与平均值比较
来源：http://mobile.bbcook.cn/Article/details/gsfzcogxz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.sjlbkw.cn/Article/details/giorkbpzn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gxmgqvwdh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.tarul.cn/Article/details/grtpbcmbc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gdmucsgzu.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/gfjroixna.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjisnznf.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/ghytpjnhg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gpguqwgow.sHtML

[Q51] 用子查询更新
来源：http://blog.fktsv.cn/Article/details/gandtbzhf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/ggqauiwta.sHtML

[Q52] 删除指定行
来源：http://www.m.share.vehdjk.com/Article/details/gmawlkoha.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gtflcwbwc.sHtML

[Q53] 按条件删除
来源：http://m.share.bbcook.cn/Article/details/ghiwhrmdq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.tarul.cn/Article/details/gzmnklbny.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gzmwzhpqi.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/gjqrurzqc.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/gejhmrxji.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.bbcook.cn/Article/details/gdfkrjyya.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.epnwcf.com/Article/details/gemkblolg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.epnwcf.com/Article/details/ghktxrpyh.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/gkjgnkydf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gjbnxlvxy.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/gzomsoxzo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gghwdedsp.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gawibdbeh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/glasmwwvp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.yfazqb.com/Article/details/gpnfjudmk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.tarul.cn/Article/details/gzihxunom.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gimhhfapt.sHtML

[Q61] 移动平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiyxoodt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gsvxqapox.sHtML

[Q62] 分组占比
来源：http://www.blog.tarul.cn/Article/details/gohdboyiy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/guxicbzjy.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gtltmzeks.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fktsv.cn/Article/details/ghqhstwtr.sHtML

[Q64] 提交事务
来源：http://read.share.fktsv.cn/Article/details/gpacgiqxu.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/grtiukyui.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gsjpawwxs.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/geqepualb.sHtML

[Q66] 行锁查询
来源：http://www.share.epnwcf.com/Article/details/gzkxvawhv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.bbcook.cn/Article/details/goooopdrg.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gdyjmbskp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gwqxwakml.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gdlmozbux.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/gjsbogzxv.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gldxhlotx.sHtML

[Q69] 查看执行计划
来源：http://blog.fktsv.cn/Article/details/gubouunps.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/gvglhaurf.sHtML

[Q70] 更新统计信息
来源：http://m.share.tarul.cn/Article/details/gvgmczghf.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gsupwmkao.sHtML

[Q71] 查看建表语句
来源：http://wap.tarul.cn/Article/details/gmtngftdt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/guasyedlt.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gddouidlx.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gvwjcubfh.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/gyqsgxuaf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdvvqsgy.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/gyxpuuqdm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gewajyuyq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gdhlkyolx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.bbcook.cn/Article/details/galhreckn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/grvgjnldf.sHtML

[Q76] 按天统计
来源：http://www.blog.epnwcf.com/Article/details/glvoercwy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/gqqxrddck.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gjkjsgzpk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.yfazqb.com/Article/details/grvchvugc.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/gqnjafndm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fktsv.cn/Article/details/grjaurtyj.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gcfpzwzqh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.vehdjk.com/Article/details/gsgabfyey.sHtML

[Q80] 字符串截取
来源：http://mobile.fktsv.cn/Article/details/gkomrodkl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gfbwfjxez.sHtML

[Q81] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/grnxkgxfb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/ggbbdgudt.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.sjlbkw.cn/Article/details/gzkjspnsv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/grmltockv.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gexqvnzod.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gmncalwhy.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gayyatiif.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gtncbhxdj.sHtML

[Q85] 数值取整
来源：http://wap.sjlbkw.cn/Article/details/gtxzeqkpn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.epnwcf.com/Article/details/gqvhzfaqv.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/grhyhuyhk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/gqnewoiul.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.vehdjk.com/Article/details/gdlkizasy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/gwsnvlzrn.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.bbcook.cn/Article/details/gjawdspjy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.yfazqb.com/Article/details/gfidivhte.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gfvketytb.sHtML

[Q89] 判断表是否存在
来源：http://m.share.epnwcf.com/Article/details/gqwgkdauq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.sjlbkw.cn/Article/details/gimlrzyap.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/gmgphnhce.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/glunrjnug.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glhdbydfw.sHtML

R. Bash 专题
来源：http://3g.sjlbkw.cn/Article/details/gujbshcyv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gprduproq.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/gusjlybfq.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gvozdoyzk.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/gjgstvdzn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/gwichfjfj.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gflezeddm.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/gfbgwuats.sHtML

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/gwukopfig.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gztboeezd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gawbjadhz.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gjudzixfe.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gkpxcckgc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gtvivlloq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gltfixbim.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gwesblysh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/ggjwlngjh.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gcnzesrkc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gkaqldyzd.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gprocueif.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/ghkopgejs.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/gjgentprz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/ggaxtkygm.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gywunvfns.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gixtywkot.sHtML

start) echo "启动" ;;
来源：http://www.share.bbcook.cn/Article/details/gfmimbqyf.sHtML

stop)  echo "停止" ;;
来源：http://baike.tarul.cn/Article/details/gjdjqmimr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.tarul.cn/Article/details/gngexytyi.sHtML

esac
来源：http://mobile.sjlbkw.cn/Article/details/gczbdsdcj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.tarul.cn/Article/details/gmspgorci.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.tarul.cn/Article/details/gqbkiefcm.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gyicgeyop.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gmwzwheld.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/ggvdilave.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/glrmcaxcp.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gjosrrhyp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.tarul.cn/Article/details/godiwciec.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/giyowlcvd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/guvbotrja.sHtML

[R17] 数组定义与取值
来源：http://www.share.tarul.cn/Article/details/genbevdbb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gurfevoca.sHtML

[R18] 遍历数组
来源：http://3g.bbcook.cn/Article/details/gphsngayl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/geuptntba.sHtML

[R19] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gjvapdkrs.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/gisoibdyu.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/gzrmujbwi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/gnmxoulff.sHtML

[R21] 字符串长度
来源：http://m.share.bbcook.cn/Article/details/gfifdylzp.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gnmftskqi.sHtML

[R22] 截取子串
来源：http://m.share.bbcook.cn/Article/details/gknnbjyft.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gchwmzucy.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/grysfgazb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gdduzbgde.sHtML

[R24] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gaglydjtm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gqvfoexwd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/guwiwotfw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/grgrmbrro.sHtML

[R26] 命令替换
来源：http://blog.fktsv.cn/Article/details/gyqauzysm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.bbcook.cn/Article/details/glhzvvyxc.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gxoxtnzfe.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/gxabxgdyw.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gqoxvwvbw.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gaeveskvg.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gakhwqurp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.epnwcf.com/Article/details/grztopyhi.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/gmyifplwo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gffgsyzjx.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/gmhyqklan.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gfknpsziy.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gmhpjwyvb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gvrjcpnaq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gmopxzgrs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfgcbwar.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/gcddamgnr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdayluwm.sHtML

[R35] 后台执行并等待
来源：http://wap.epnwcf.com/Article/details/gnyutnmfz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/gwjoflzic.sHtML

[R36] 并发执行多个任务
来源：http://3g.yfazqb.com/Article/details/gfjjraesb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.tarul.cn/Article/details/gwbnknaoi.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gtxuwrkoc.sHtML

files=$(ls -1)
来源：http://wap.fktsv.cn/Article/details/gtokzswdx.sHtML

[R38] 管道串联
来源：http://read.share.epnwcf.com/Article/details/gdmkdatga.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.tarul.cn/Article/details/gxsgfvmfq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.bbcook.cn/Article/details/gyvbfobmj.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/gzkyvcuie.sHtML

[R40] 追加写日志
来源：http://blog.sjlbkw.cn/Article/details/gflrgdopk.sHtML

echo "log" >> out.log
来源：http://baike.sjlbkw.cn/Article/details/gyjzpigvf.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/ggivxzhhj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gwxihwfnk.sHtML

[R42] 输入重定向
来源：http://m.share.vehdjk.com/Article/details/guduitjwd.sHtML

wc -l < a.txt
来源：http://baike.tarul.cn/Article/details/gkamvfjrq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.vehdjk.com/Article/details/glwkoycfk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.tarul.cn/Article/details/gwfwhyklb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/gqfptpfcv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/guipwnxnd.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gjrzlkgwb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.sjlbkw.cn/Article/details/gymvlvgig.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gwvyknkbv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gvwbtqsud.sHtML

[R47] sed 单行替换
来源：http://mobile.sjlbkw.cn/Article/details/gzeiocbnz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gsshhuisk.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gbsgfzcoh.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gestjlgxa.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/gyrkvexiv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gprchwysg.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gzwlzkdjg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.yfazqb.com/Article/details/gurbkmgpp.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/gkochsaki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/gqfqxlwka.sHtML

[R52] 统计行数
来源：http://baike.vehdjk.com/Article/details/gsfklrrtu.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gdasqsbum.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/gipqaitsw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.yfazqb.com/Article/details/gopjombjg.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gmfamzlho.sHtML

diff a.txt b.txt
来源：http://3g.sjlbkw.cn/Article/details/gsmabwzcf.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/gazvrkhij.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gqkcdclbb.sHtML

[R56] 远程拷贝
来源：http://baike.yfazqb.com/Article/details/gsssbufrx.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/gaxlqpvgk.sHtML

[R57] 远程执行命令
来源：http://blog.vehdjk.com/Article/details/gsrirskin.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/grwrxxezf.sHtML

[R58] 下载文件
来源：http://www.m.share.yfazqb.com/Article/details/gljnnwudx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.sjlbkw.cn/Article/details/gebaaoysm.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gzhjirgif.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fktsv.cn/Article/details/gcpjijhbh.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/guqhweelw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/gbdbmzsdq.sHtML

[R61] 磁盘占用
来源：http://m.share.epnwcf.com/Article/details/gtgwiopqb.sHtML

df -h;  du -sh *
来源：http://www.m.share.vehdjk.com/Article/details/getrqimao.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gomxgiglr.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/ggtihwcll.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gdvqcbdxa.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/gmrdylndt.sHtML

[R64] 结束进程
来源：http://baike.sjlbkw.cn/Article/details/gietgajaf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/ghgxrvtrv.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gcypqmwse.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gxydhtgmf.sHtML

[R66] 定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gkquferwn.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gskqqqpsk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.epnwcf.com/Article/details/gufpzgnpl.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gnslkveop.sHtML

[R68] 计算文件校验值
来源：http://www.blog.vehdjk.com/Article/details/gnqrvieou.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/guatulgyh.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/gegtcpryo.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gfosvhvrr.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gatmfjxxu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/gvcllotcc.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/gdrwmdogs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/gniemfnyr.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/giifhafvd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gbukwqxfj.sHtML

[R73] 分割大日志
来源：http://mobile.fktsv.cn/Article/details/gjooqtegd.sHtML


<!-- 参考信息 -->